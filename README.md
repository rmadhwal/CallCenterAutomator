# CallCenterAutomator

## Run

If you haven't done so already, install the [Tabris CLI](https://www.npmjs.com/package/tabris-cli) on your machine:

```
npm i tabris-cli -g
```

Then in the project directory, type:

```
npm start
```


This will start a Tabris.js code server at a free port and print its URL to the console. The app code can then be [side-loaded](https://docs.tabris.com/3.7/developer-app.html#run-your-app) in the [developer app](https://docs.tabris.com/3.7/developer-app.html) by entering that URL.

Alternatively you can also call the Tabris CLI directly:

```
tabris serve -a -w
```

This the same as running `npm start`. The `-w` switch starts the compiler in watch mode, meaning you do not have to re-start the server after each code change, and `-a` causes the app to reload automatically as well.

## Test

You can run compiler, linter and all unit tests with a single command:
```
npm test
```

Unit tests are executed with [Mocha](https://mochajs.org/) and located in the `test` directory. They can be run explicitly via:

```
npm run mocha
```

This project also includes a ESLint configuration that helps preventing common mistakes in your code. Most IDEs can display ESLint-based hints directly in the editor, but you can also run the tool explicitly via:

```
npm run lint
```

## Debugging


### Android

Tabris on Android supports any debugger that uses the V8 inspector protocol. This includes Visual Studio Code, WebStorm and the Chrome Browser. More information can be found [here](https://docs.tabris.com/3.7/debug.html#android).

### iOS

On iOS, the Safari developer tools [can be used for debugging](https://docs.tabris.com/3.7/debug.html#ios).

Tabris.js unit tests support any debugger that works with Node.js.
## Build

The app can be built using the online build service at [tabrisjs.com](https://tabrisjs.com) or locally using [Tabris.js CLI](https://www.npmjs.com/package/tabris-cli).

See [Building a Tabris.js App](https://docs.tabris.com/3.7/build.html) for more information.
