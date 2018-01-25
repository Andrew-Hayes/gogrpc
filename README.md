# gogrpc
A Docker container used to build golang projects using GRPC code

## Building your project
You can build your project by running the command below:

```docker run --rm -v "${PWD}":/go/src/<your app> -w /go/src/<your app> puppetlabs/myapp:latest go build -v```

This mounts the current directory to /go/src/<your app> , sets the working directory to /go/src/<your app> and runs go build.

Alternatively if you need to run a few steps such as protoc you can use make i.e.
```docker run --rm -v "${PWD}":/go/src/<your app> -w /go/src/<your app> puppetlabs/myapp:latest make all```
