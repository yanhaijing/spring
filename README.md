# 青丝集

## 依赖环境
- gitbook-cli@0.3.6
- gitbook@2.3.3
- calibre@2.38.0

使用如下命令安装：

    $ npm install gitbook@0.3.6 -g
    $ gitbook versions:install 2.3.3

## 构建命令
安装插件

    $ gitbook install

本地模拟

	$ gitbook serve --port 8001

产出静态资源

	$ gitbook build . ../temp

生成pdf文件，依赖[calibre](calibre)里的ebook-convert

	$ gitbook pdf . ../spring.pdf

生成一个markdown文件，需要node环境

    $ npm run build:markdown

生成docx格式，依赖生成的统一markdown文件，依赖[pandoc](http://pandoc.org/)环境

    $ pandoc spring.md -o spring.docx

## LICENSE
[LICENSE](./LICENSE.md)


[calibre]: http://calibre-ebook.com/
