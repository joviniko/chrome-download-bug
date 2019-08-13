# Google Chrome Download Bug

This is an example to recreate the "Failed - Bad certificate" download error.
Created for the chromium issue: https://bugs.chromium.org/p/chromium/issues/detail?id=993362

## Run the test
```
$ docker-compose up
```

 - go to https://localhost:8080
 - click on the download link
 - Wait 90 seconds. Do not refresh the page
 - Click on the download link again. Returns "Failed - Bad certificate"

## Tested on Ubuntu 18.04.3 

 - Google Chrome Version 76.0.3809.100 (Official Build) (64-bit) - fails
 - Firefox 68.0.1 (64-bit) - works as expected
