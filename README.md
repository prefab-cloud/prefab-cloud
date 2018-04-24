# prefab-cloud
Shared protobuf definitions for https://www.prefab.cloud

See https://github.com/prefab-cloud/prefab-cloud-ruby for an example library


To build a client library, checkout this project then run something similar to 
```
protoc --proto_path=prefab-cloud \
  --php_out=prefab-cloud-php \
  --grpc_out=prefab-cloud-php \
  --plugin=protoc-gen-grpc=bins/opt/grpc_php_plugin \
  prefab.proto
```
for your language.
