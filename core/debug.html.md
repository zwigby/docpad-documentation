```
title: "Debugging"
```

Sometimes things go bad and you need to get into DocPad and work out what's happening. A plugin may be not working as expected, content isn't being generated or you're just curious as to how to do it. Well for that you'll need to get your debugging on.


## Debugging with Node Inspector

### What you'll need

1. Get Node Inspector by following the installation instructions [here](https://gist.github.com/balupton/3944017)
2. Get a Webkit based browser (stable channel of Google Chrome and Safari both work great)

### Debugging

1. Open Node Inspector up by running `node-inspector` in another Terminal window:

1. Open up our local DocPad instance for debugging by running:

	``` bash
	node --debug-brk ./node_modules/.bin/docpad run
	```

1. Navigate to http://127.0.0.1:8080/debug?port=5858 in your webkit based browser and start debugging (sometimes you may have to refresh or restart the node inspector or docpad instances).
