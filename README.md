# Easy HTTP server in Go

This small repo is meant to demonstrate an HTTP server which is super easy to build and deploy.

Please read the [accompanying article](http://popovicu.com/posts/easy-to-build-and-deploy-go-servers) on my website for more details.

## Building

```
bazel build //server
```

This should result in a single binary file that is ready to be deployed.

## Running

You can build with the command above and manually invoke the binary, but with Bazel it's cleaner to use the `run` command.

```
bazel run //server
```
 
You can then test it with:

```
curl http://localhost:12345/hello/foo
```

Output:

```
Hello foo
```
