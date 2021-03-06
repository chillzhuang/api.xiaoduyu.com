# 小度鱼（后端API篇）

### 介绍
小度鱼是一个好学人们的社区  
[https://www.xiaoduyu.com](https://www.xiaoduyu.com) 
### 技术栈
TypeScript、NodeJS、Express、GraphQL、MongoDB


### 本地开发环境部署
不保证 Windows 系统的兼容性  
线上运行版本 Node.js 是 v8.7.0，MongoDB 是 v3.4.9

1、安装 Node.js[必须] MongoDB[必须]   
2、克隆项目   
```
git clone git@github.com:54sword/api.xiaoduyu.com.git   
```
   
3、进入项目   
```
cd api.xiaoduyu.com
```
   
4、安装依赖包   
```
npm install
npm install -g typescript
```
   
5、创建默认的配置文件，并根据需要修改其中的配置   
```
cp ./src/config/index.default.ts ./src/config/index.ts
```

6、创建日志文件夹  
```
mkdir ./logs
```
   
7、运行TypeScript编译器，监控src里面的文件变化      
```
npm run watch-ts
```
   
8、启动项目  
```
npm run start
```

9、浏览器中打开 http://localhost:3000

### 服务器部署
1、打包项目  
```
npm run dist
```

2、将 dist、public、logs、package.json、package-lock.json 上传到服务器，然后执行如下命令，安装依赖包  
```
npm install
```

3、启动服务  
```
node ./dist/index.js
```


### 小度鱼相关开源项目
 + 前端：[https://github.com/54sword/xiaoduyu.com](https://github.com/54sword/xiaoduyu.com)  
 + 后端：[https://github.com/54sword/api.xiaoduyu.com](https://github.com/54sword/api.xiaoduyu.com)  
 + 移动端：[https://github.com/54sword/xiaoduyuReactNative](https://github.com/54sword/xiaoduyuReactNative)  
 + 后台管理：[https://github.com/54sword/admin.xiaoduyu.com](https://github.com/54sword/admin.xiaoduyu.com)  
 + 自制React同构脚手架：[https://github.com/54sword/react-starter](https://github.com/54sword/react-starter)  

### 开源协议
MIT
