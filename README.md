# DemoGrpcJava

参照grpc官方依赖，实现java的client与server的grpc明文及TLS通信。

server启动需要命令参数：

1.启动端口号

2.服务端证书公钥

3.服务端证书私钥

4.指定的客户端证书公钥（可选，指定后只能与对应的客户端进行TLS通信）


 >示例：9999 .\server.pem .\server.key .\client.crt

client启动需要的命令参数：

1.服务端ip

2.服务端端口

3.服务端证书公钥

4.客户端证书公钥（可选，若服务端指定了客户端证书公钥，则必填）

5.客户端证书私钥（可选，若服务端指定了客户端证书公钥，则必填）

>示例：127.0.0.1 9999 .\server.crt .\client.crt .\client.key

