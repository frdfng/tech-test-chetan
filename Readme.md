# Hands on tech lab

Welcome to the *ubank* tech lab!

## About

A simple express project with an endpoint that requires an implementation of a Basic Authentication validation for incoming HTTP calls.

The definition of the Basic Authentication scheme is that a value in the format of `Basic <credentials>` is passed as the value to the `authorization` header of a request. Where *credentials* is in the format of a base 64 encoded string using the values of the `username` and `password` joined using the `:` character. The `username` and `password` can not contain the `:` character and the header value must start with the word `Basic`.

In this exercise, implement the functionality to authorise a request based on whether a request contains a valid users credentials based on the list of users as defined in `src/userLogins.ts`. If the credentials are invalid then the response is expected to return a HTTP status with `401`.

An example header could look like:

`authorization: Basic bWF0dEBnbWFpbC5jb206dGhpcyBpcyBhIHZAbGlkIHBhc3N3b3JkIQ==`

# Getting started

* Run `npm install`
* Run `npm run test`
* Check tests that are failing and trouble shoot what needs to be fixed in the application code
