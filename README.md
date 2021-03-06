# analyser-common

[![Build Status](https://travis-ci.org/sidekickcode/analyser-common.svg?branch=master)](https://travis-ci.org/sidekickcode/analyser-common)

Module that provides `stdin` input in a pre-defined way to a Sidekick analyser.

Provides analysers with a `setup` object that contains:

 - config (any configuration file contents for the analyser, e.g. .eslintrc file contents)
 - contents (the contents of the file to be analysed)
 - filePath (the file path of the file to be analysed)

You can easily write your own analysers for use with [Sidekick](https://sidekickcode.com).
Sidekick analysers can be written in any language; all you need to do is accept input via `stdin` and provide output via `stdout`.

## Installation

```sh
npm install --save @sidekick/analyser-common
```

## Usage

```sh
var sidekickAnalyser = require("@sidekick/analyser-common");
sidekickAnalyser(function(setup){
  //run the analyser
});
```
