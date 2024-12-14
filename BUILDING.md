# How to build this spec

This repository uses the [ReSpec toolchain](https://respec.org/docs/). Please find below a quick getting started cheatsheet using the [command line](https://respec.org/docs/#using-command-line) tools.

Setup `respec` for multiple use:
```
$ npm install --global respec
```
Update your environment with the following variables:
```
export PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=1
export PUPPETEER_EXECUTABLE_PATH="/usr/bin/google-chrome"
# replace "/usr/bin/google-chrome" with path to Chrome executable on your system.
# On MacOS, it's generally:
# "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
```
This spec uses the `data-include` attribute. For `respec` to work locally, the content MUST be served by a web server. One easy way to achive that is to run one from the project directory:
```
# Install a local HTTP server if not already installed (one time)
$ npm install -g http-server

# Start the server in your project directory
$ http-server
```

Note that the server starts on port 8080. Now you can run `respec` to generate the spec [`index.html`](http://localhost:8080/index.html) in the project root and test changes.
```
$ respec --src http://localhost:8080/spec/index.html --out index.html
```

