## Grunt-Impact

![Alt text](grunt-impact-logo.png)

Grunt-Impact is a [Grunt](http://gruntjs.com/) build system for all your [ImpactJS](http://impactjs.com/) games. It aims to streamline baking and deployment to a few keystrokes.

Before you do anything else, you must have [nodejs](http://nodejs.org/) installed.

Once nodejs is installed, copy Gruntfile.js, excludes and package.json to your ImpactJS directory, and then go to the root of your ImpactJS game directory and run the following commands:

```Shell
npm install -g grunt-cli
npm install
```

This will install grunt and then install all devDependencies specified in the package.json.

After running the commands you need to take a look at the [package.json](package.json) file and update the commented items to your local configuration.

And that's it!

Now you will have all the available commands listed below that can be run from the root of your ImpactJS game directory.

## Commands

- grunt bake - bakes your game
- grunt build - bakes and uglifies your game
- grunt cocoon - deploys a zip to a connected android phone for use with [CocoonJS](http://www.ludei.com/tech/cocoonjs)
- grunt deploy - deploys your game to a remote server (settings in package.json)
- grunt expose - replace all occurrences of ig with window.ig to expose ig globally for compilation purposes
- grunt inject - injects minified script tags into your html files (specified in package.json) and removes the impact dev script tags
- grunt prepare - bakes, uglifies and injects
- grunt publish - bakes, uglifies, injects, deploys and reverts
- grunt revert - removes the minified script tags from your html files (specified in package.json) and injects the impact dev script tags
- grunt uglify - uglifies the baked file

If you run '''grunt''' by itself, it'll do the same as ```grunt build```.

## What's Next?

That's up to you! This Grunt configuration is by no means exhaustive to the ImpactJS community needs. Please feel free to offer up suggestions and pull requests to make Grunt-Impact better!
