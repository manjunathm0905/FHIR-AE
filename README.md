# Adverse Event IG

[![Build Status](https://travis-ci.org/HealthSamurai/ig-ae.svg?branch=master)](https://travis-ci.org/HealthSamurai/ig-ae)

Implementation Guide for Adverse Event.

Current version is published at https://healthsamurai.github.io/ig-ae/

## Development

In order to develop the implementation guide, do the following steps:

* clone the repo
* cd ig-ae
* execute `npm install` in a command line
* git submodule init
* git submodule update
* execute `./igpop.sh dev` in the command line to run a local server on 8899 (may be changed with `-p` param)
* navigate to `http://localhost:8899` to see results of editing
