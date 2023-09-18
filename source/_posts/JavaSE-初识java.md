---
title: JavaSE 初识java
date: 2023-09-18 08:56:10
tags:
  - javaSE
  - java
category: 复习
---

## 运行

1. 创建一个 Hello.text 文件,将后缀改为.java
2. 编辑文件代码如下

```java
class HelloChina{
	public static void main(String[] args){
		System.out.println("hello 中国!!!");
		System.out.print("hello 中国!!!");
		System.out.println(123+1);
	}
}
```

3. 进入文件所在目录输入编译命令 javac Hello.java
4. 运行编译文件 java HelloChina

## 注释

1. java 注释种类

   - 单行注释 //
   - 多行注释 /\* /
   - 文档注释 /\*\* /

2. 注释的作用

   1. 对程序中的代码做解释作用
   2. 对程序进行调试

3. 注意

   - 单行注释和多行注释不参与程序的编译,就是说你在代码中写再多的注释编译的时候都会去掉,但是文档注释会参加编译
   - 多行注释不能嵌套使用

4. 文档注释
   - 文档注释内容会被 jdk 提供的工具 javadoc 识别解析,生成一套以网页文件形式体现的该程序说明文档

## 总结

1. 怎么解释 java 是半编译边运行语言?
   - 解释重点在运行这一块,首先明确只有在 javac 编译完成生成了.class 的字节码文件才可以运行.所以在运行阶段 jvm 会读到整个.class 文件然后自行决定如果运行可能是一半一半的读和运行也可能是一整个读然后运行
