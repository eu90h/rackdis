# rackdis
[![Build Status](https://travis-ci.org/eu90h/rackdis.svg?branch=master)](https://travis-ci.org/eu90h/rackdis)

Redis client for Racket. The documentation still needs to be written, but for now see the `tests.rkt` file to see example
usage. Currently the entire set of Redis v1 commands is implemented, along with most of v2 and some of v3. 

The api is 1-1 with Redis, except in one way: the Redis append command has been renamed to concat.

Example Usage
=============
Create a redis object: `(define redis (new redis%))`

Initialize it: `(send redis init)`

Send a command: `(send redis set "a-number" "1")`

Installation
============
Execute `raco pkg install git://github.com/eu90h/rackdis` or use DrRacket.

To uninstall, run `raco pkg remove rackdis`
