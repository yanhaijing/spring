# 青丝集 [![Build Status](https://travis-ci.org/yanhaijing/spring.svg?branch=source)](https://travis-ci.org/yanhaijing/spring)
[GitBook使用笔记](http://yanhaijing.com/tool/2015/09/12/my-gitbook-note/)

## 依赖环境
- gitbook-cli@2.3.0
- gitbook@3.2.2
- calibre@2.38.0

使用如下命令安装：

    $ npm install -g gitbook-cli@2.3.0
    $ gitbook fetch 3.2.2

## 构建命令
安装插件

    $ gitbook install

本地模拟

	$ gitbook serve --port 8001

产出静态资源

	$ gitbook build . ../temp

生成pdf, epub, mobi文件，依赖[calibre](calibre)里的ebook-convert

    $ gitbook pdf . ./spring.pdf
    $ gitbook epub . ./spring.epub
	$ gitbook mobi . ./spring.mobi

生成一个markdown文件，需要node环境

    $ npm run build:markdown

生成docx格式，依赖生成的统一markdown文件，依赖[pandoc](http://pandoc.org/)环境

    $ pandoc spring.md -o spring.docx

## LICENSE
[LICENSE](./LICENSE.md)


[calibre]: http://calibre-ebook.com/
