ffmpeg static binaries for Mac OSX and Linux (Lambda) ~~and Windows~~

## Why another package?

This package should work locally on Mac and in Vercel/Lambda linux deployments with node20
- existing packages either didn't include the binary in the repo itself (downloaded the binary upon install which didn't work with Vercel)
- and/or the binary was not working in Lambda env (amazon linux 2023 is used for node 20)



## Installation

This module is installed via npm:

``` bash
$ npm install https://github.com/AndreyMay/ffmpeg-static-lambda
```

## Example Usage

Returns the path of a statically linked ffmpeg binary on the local filesystem.

``` js
var ffmpeg = require('ffmpeg-static-lambda');
console.log(ffmpeg.path);
```

- Currently supports Mac OS X (64-bit), Linux (~~32 and~~ 64-bit) 
- Windows (32 and 64-bit) was removed
