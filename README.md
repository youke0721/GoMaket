# 项目简介

## 简介
本项目实现了一个电商项目的核心功能，内容包括：用户登录、用户注册、jwt鉴权、商品分类管理、商品管理、订单管理、购物车管理。

## 技术栈
go + mysql + gorm + gin + jwt + viper + swagger api + air + 分页技术

## 架构
本电商项目采用mvc设计模式，及Model-View-Controller设计模式，有五大模块：

用户模块user
商品分类模块category
商品模块product
订单模块order
购物车模块cart

## 目录结构
![image](https://github.com/youke0721/GoMaket/assets/118320030/b355891d-f681-40d2-89b2-5fcb198d37f1)

api ，包括controller和router路由，向客户端提供api接口。
config，系统配置文件和配置类
docs，swagger文档配置类和配置文件
domain，数据模型entity、数据逻辑repository、和业务逻辑service
utils，系统工具类，jwt、中间件、分页等

## 术语
api，appplication programming interface，api接口
config，配置
docs，文档
domain，域
utils，工具
cart，购物车
category，分类
order，订单
product，商品
user，用户

## 修改配置文件
```
Env: "dev"

DatabaseSettings:
  DatabaseURI: "root:123456@tcp(127.0.0.1:3306)/go_database?parseTime=True&loc=Local"
  DatabaseName: "go_database"
  Username: "root"
  Password: "123456"


JwtSettings:
  SecretKey: "golang-tech-stack.com"
```

## 创建数据库
```
create database go_database
```


## 编译
```
go run main.go
```

## 访问
```
http://localhost:8080/swagger/index.html\
```

## 展示
![image](https://github.com/youke0721/GoMaket/assets/118320030/2655bf0e-a406-4166-8b13-dcd2c383209d)
