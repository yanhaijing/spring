# 青丝集

## 依赖环境
- gitbook-cli 0.3.6
- gitbook 2.3.3

使用如下命令安装：

    $ npm install gitbook -g
    $ gitbook versions:install 2.3.3

## 构建命令
本地模拟

	$ gitbook serve --port 8001

产出静态资源

	$ gitbook build . ../temp

生成pdf文件

	$ gitbook pdf . ../spring.pdf

## LICENSE
[LICENSE](./LICENSE.md)