# webpack-sftp-client

## Introduction

A plugin for webpack as an sftp client

## Installation

```
npm install webpack-sftp-client
```

## Usage

```
var fs = require('fs');

var WebpackSftpClient = require('webpack-sftp-client');

var privateKey = fs.readFileSync('your_key_rsa')

new WebpackSftpClient({
    port: '22',
    host: 'example.com',
    username: 'nonroot',
    privateKey: privateKey,
    path: './build/',
    remotePath: '/data/website/demo/',
    // Show details of uploading for files
    verbose: true
})
```
Copyright (c) 2016 - 2017 zhangyuhang
Copyright (c) 2019 jefrancomix / tzkmx

MIT (http://www.opensource.org/licenses/mit-license.php)
