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
  
## efficiently go  
### string join 
0. '+' (base):字符串越长越慢 
1. string.Builder (~5000): https://golang.org/pkg/strings/#Builder 
2. bytes.Buffer(~2000) : https://stackoverflow.com/questions/1760757/how-to-efficiently-concatenate-strings-in-go 
![beachmark](https://github.com/sniperdong/go-framework/blob/master/string_join_beach.png) 

### capacity 
1. map ,slice 在能预知容量的情况下指定cap，可以有效减少动态伸缩和GC
