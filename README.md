# GitHub
---

## 关键字查询：

  xx(python) awesome:查该标签下的xx （Python）项目
  xx(python) tutorial:查询xx（python）资料、书籍、文档
  xx(docket) sample:查询对应技术（socket）的代码样本

## GitHub三要素：

### Repository：
  
  仓库是github项目管理存储基本单位
  一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public、private

### Commit提交：

  程序员在整个开发周期，有大量的对代码资源的选代和修改，都可以通过commit的方式进行记录，便于程序员回溯代码，即使这些代码被删除
  提交便于使用者观察整个工程的开发流程以及设计流程

### Branch分支：

  在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为master/main
  \*不仅可以管理代码存储，便于多人开发协作
![图片1](https://i.postimg.cc/7PtVG2H7/1.png)

## 仓库内容

  Code，资源存储，代码资源，二进制，项目管理脚本，许可证等等

  issues，使用时遇到的bug或进行提交，等待反馈

  README，使用markdown语言编写，工程自述文件，开发进度，版本更新，使用介绍等等

  LICENSE许可证：GPL2.0，3.0.Apahce2.0，Mit，这些许可证，给使用者最大使用权限以及最少的限制

## Git软件，分布式版本控制系统

  仓库管理软件，使用git管理私人代码或企业代码
![图片2](https://i.postimg.cc/sDNsNwVX/2.png)
  
## 设备认证

1. 让网站的账户与设备绑定，后续完成代码的管理。上传下载
```bash
	git init // 创建本地仓库 \*后续对仓库的操作，都要在仓库位置（master）
```
```bash
	git config --list //查看git的配置文件
```

* 修改或添加config配置项
```bash
	git config --global user.name //用户名
	git config --global user.email //注册邮箱
```
* 生成本机设备密文
```bash
	ssh-keygen -t rsa -c "注册邮箱"
```
rsa.pub复制密文，粘贴到setting-> SSH key and GPG -> new ssh key -> 粘贴
* 测试关联是否成功
```bash 
	ssh -T git@github.com # ssh远程登录
```
2. 为目标仓库起别名，定位目标仓库，后续上传


# Markdowm,文本修饰语言，用特殊符号修饰正文效果<dr>

## 标题修饰符\#

# 标题修饰符（一级标题）
## （二级标题）
### （三级标题）
#### （四级标题）
##### （五级标题）


## 正文内容

  输入正文内容，但是如果需要换行，用\<br\>标签

## 修饰正文

  *一段测试文本*

  **一段测试文本**

  ***一段测试文本***

  ~~一段测试文本~~

  将一段文本中的，`关键字`重点突出

## 分割线
 
  用\-\-\-表示分割线
---

## 引用用\>表示
> 一级引用
>> 二级引用
>>> 三级引用
>>>> 四级引用

## 列表修饰符
### 无序列表
* 一级
  * 二级
    * 三级
* 哈哈哈
  * 哈哈
  * 哈

### 有序列表1.
1. 物理
   1. 量子
   2. 原子
2. 计算机
   1. 云计算
   2. 嵌入式

### 混合列表
1. 测试一级
   * 测试二级
   2. 测试三级

### 表格
名称|技能|排行
--|:--:|--:
蝙蝠侠|有钱|1
蜘蛛侠|有颜|2
闪电侠|体育生|3

### 代码片段

```c
	#include<stdio.h>
```
```cpp
	#include<iostream>
```
```bash
	echo "测试"
	pwd
	ps aux
	ls -al
```

### 超链接

[github](https://github.com "点击访问")

### 插入图片

![测试](C://Users//24228//Desktop//1.png)
