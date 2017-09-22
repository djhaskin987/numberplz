# numberplz
A simple web app that returns an auto incremented integer every time a GET
request is sent to it:

```bash
$ numberplz &
$ curl localhost:8080
0
$ curl localhost:8080
1
$ curl localhost:8080
2
```

The number starts at 0 and goes up by 1 each time GET is called on it.

To restart the count, simply restart the app.

This is kinda cool. It allows you to run a web service which, for example,
can give each microservice that starts up and asks for a number from it a
different ID. The use case I can see for this is when different agents need to
know who they are in relation to each other for a short-lived job, such as a
kubernetes Job, and perhaps for even longer lived jobs.

Pull and feature requests welcome! and thanks to Jason Reicheneker for the
idea :)

# Install

Install go and then just run `go get github.com/djhaskin987/numberplz`.

# Build

If you're more interested in building it, check it out to the folder
`$GOPATH/github.com/djhaskin987/numberplz`.
