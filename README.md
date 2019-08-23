# Dependencies

## Protobuf

It's possible install via APT using
```
$ sudo aptitude install protobuf-compiler
```

or via purist way, downloading and compiling.
Go to https://github.com/protocolbuffers/protobuf/releases and download `protobuf-all-<version>.tar.gz`.
After download it:
```
$ tar zxf protobuf-cpp-<version>.tar.gz
$ cd protobuf-<version>
$ ./autogen.sh
$ ./configure
$ make
$ make check
$ sudo make install
$ sudo ldconfig # refresh shared library cache.
$ sudo make clean
$ cd ..
$ rm -rf protobuf-<version>
```

More about protobuf instalation check [here](https://github.com/protocolbuffers/protobuf/blob/master/src/README.md)

## gRPC

```
$ go get -u google.golang.org/grpc
$ go get -u github.com/golang/protobuf/protoc-gen-go
```

# Build and run

```
$ go mod init github.com/rodrigovdb/microservices-blog
$ go get -u
```

# References

* https://ewanvalentine.io/microservices-in-golang-part-1/
