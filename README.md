# DemoGrpcJava

参照grpc官方依赖，实现java的client与server的grpc明文及TLS通信。

server启动需要命令参数：

 >9999 .\server.pem .\server.key .\client.crt

client启动需要的命令参数：

>127.0.0.1 9999 .\server.crt .\client.crt .\client.key

