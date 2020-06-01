# Gateway

This repo contains a JSON marshaler suitable for use with the gRPC-Gateway
when using `gogo/protobuf` types.

This fork includes an option to disable HTML escaping, as this isn't easy to
workaround with the upstream packages:

- https://github.com/gogo/protobuf/issues/484
- https://github.com/golang/protobuf/issues/407
- https://github.com/grpc-ecosystem/grpc-gateway/issues/566

## Original License

95% of the code is copied from the gRPC-Gateway project, so their license applies.

## Modified License

Apart from the above, the `gogojsonpb/` package includes
https://github.com/golang/protobuf/pull/409 merged into
https://github.com/gogo/protobuf/tree/master/jsonpb

Their licenses and authorship applies, I just copy-pasted the code here as
needed. Special thanks to Paul Nichols (@pauln) who authored the original
https://github.com/golang/protobuf/pull/409 patch.

A separate PR has been sent into the `gogo` project so perhaps this fork of
https://github.com/gogo/gateway won't be needed, if it gets merged. PR at:
https://github.com/gogo/protobuf/pull/694
