# numberplz
A simple web app that returns an auto incremented integer every time a GET
request is sent to it.

To restart the count, simply restart the app.

This is kinda cool. It allows you to run a web service which, for example,
can give each microservice that starts up and asks for a number from it a
different ID. The use case I can see for this is when different agents need to
know who they are in relation to each other for a short-lived job, such as a
kubernetes Job.

Pull and feature requests welcome! and thanks to Jason Reicheneker for the
idea :)

# Install

Install go and then just run `go get github.com/djhaskin987/numberplz`.

# Build

If you're more interested in building it, check it out to the folder
`$GOPATH/github.com/djhaskin987/numberplz`.
