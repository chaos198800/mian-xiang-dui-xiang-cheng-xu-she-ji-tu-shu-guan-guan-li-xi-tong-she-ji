# 面向对象程序设计图书馆管理系统设计

## 项目概述

本项目是一个面向对象程序设计的图书馆管理系统，采用Visual Studio 2022作为开发工具，使用C#语言和WinForm框架进行开发，数据库使用MySQL。该系统旨在帮助图书馆管理员高效地管理图书、借阅证、借书、续借、还书以及罚款等操作。

## 技术栈

- **开发工具**: Visual Studio 2022
- **编程语言**: C#
- **框架**: WinForm
- **数据库**: MySQL (版本 5.7.40)

## 功能模块

### 管理员登录模块
- **功能**: 管理员通过输入用户名和密码进行登录。
- **用户名**: admin
- **密码**: 123456

### 首页管理
- **功能**: 登录成功后加载网页显示。

### 图书查询
- **功能**: 管理员可以查询图书馆中的图书信息。

### 图书管理
- **功能**: 管理员可以添加、删除、修改图书信息。

### 借阅证管理
- **功能**: 管理员可以管理借阅证信息，包括添加、删除、修改借阅证。

### 借书管理
- **功能**: 管理员可以处理借书请求，记录借书信息。

### 续借管理
- **功能**: 管理员可以处理图书的续借请求。

### 还书管理
- **功能**: 管理员可以处理图书的还书操作。

### 罚款管理
- **功能**: 管理员可以处理逾期罚款的相关操作。

### 密码重置
- **功能**: 管理员可以重置自己的登录密码。

## 数据库设计

### 数据库名称
- **名称**: `bookmanagementdb`

### 表结构

#### 管理员表 (`admin_books`)
- **字段**:
  - `id`: 管理员ID
  - `username`: 用户名
  - `pwd`: 密码

#### 借阅书籍表 (`borrowing_books`)
- **字段**:
  - `id`: 借阅记录ID
  - `bookmanagementid`: 图书管理ID
  - `borrowing_cardid`: 借阅证ID

#### 借阅证表 (`borrowing_card`)
- **字段**:
  - `id`: 借阅证ID
  - `name`: 姓名
  - `sex`: 性别
  - `cardid`: 借阅证号码
  - `address`: 地址

#### 图书管理表 (`management_books`)
- **字段**:
  - `id`: 图书ID
  - `bookbarcode`: 图书条码
  - `bookName`: 图书名称
  - `bookAuthor`: 图书作者
  - `bookPr`: 图书价格

#### 罚款管理表 (`penalty_books`)
- **字段**:
  - `id`: 罚款记录ID
  - `bookbarcode`: 图书条码
  - `bookName`: 图书名称

## 使用说明

1. **安装环境**: 确保已安装Visual Studio 2022和MySQL 5.7.40。
2. **导入数据库**: 使用提供的SQL文件导入数据库结构。
3. **配置连接字符串**: 在项目中配置MySQL数据库连接字符串。
4. **运行项目**: 打开Visual Studio 2022，加载项目并运行。

## 注意事项

- 请确保数据库连接字符串配置正确，否则系统无法正常运行。
- 管理员登录时请使用默认用户名和密码，登录后建议立即修改密码。

## 联系我们

如有任何问题或建议，请联系项目维护者。

## 下载链接

[面向对象程序设计图书馆管理系统设计](https://pan.quark.cn/s/97633b770cfb)