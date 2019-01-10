# go-framework
go framework

## rpc  
### rpcx  
*特点* 
1. 服务发现，鉴权，限流，filemode，tcp/udp,多种传输协议 
### go-kit  
### TarsGo  
  
## config  
### viper  
*特点*  
1. 支持多种格式：{"json", "toml", "yaml", "yml", "properties", "props", "prop", "hcl"}  

*缺点*  
1. viper会把所有key自动转为小写，对hash key会有影响  
   
## logger  
### logrus  
*特点* 
1. 支持test， json格式，还可以自定义格式
*缺点*  
1. logrus不支持rotate，需要引入第三方实现  

### zap  
### zerolog  
### seelog  
  
## package  
### govendor  
