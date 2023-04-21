1. NPM install at the root of this directory `npm install`. This currently fails on ARM Macs so we'll need to install chromium ourselves and tell puppeteer to skip installing it with the following environment variables
```sh
export PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true
export PUPPETEER_EXECUTABLE_PATH=`which chromium`
```

2. Build the resume with `npm run build-dev`. This will generate an `index-dev.html` file that you can then view in your browser. Feel free to print it as a PDF
