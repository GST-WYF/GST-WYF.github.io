# GST-WYF.github.io

本作品由格斯桐和她的男朋友共同完成。

## Table of Content

-   [目录](#Directory)
-   [环境](#Environment)
-   [教程](#Tutorial)
    -   [安装Gitbook](#安装Gitbook)
    -   [初始化](#初始化)
    -   [本地预览](#本地预览)
    -   [编译电子书](#编译电子书)
-   [问答](#F&Q)
-   [协议](#License)

## Directory

```

```



## Environment

-   npm >= 6.13.4
-   Node.js >= v12.16.0
-   git >= version 2.27.0.windows.1

## Tutorial

### 安装Gitbook

```
$ npm install gitbook-cli -g
```

安装完成之后，你可以使用下面的命令来检验是否安装成功

```
$ gitbook -V
CLI version: 2.3.2
GitBook version: 3.2.3
```

如果你看到了上面类似的版本信息，则表示你已经安装成功了。

### 初始化

```
$ gitbook init
```

在使用 `gitbook init` 之后本地会生成两个文件 `README.md` 和 `SUMMARY.md` ，这两个文件都是必须的，一个为介绍，一个为目录结构。

### 本地预览

当内容书写完毕后，可以在终端中输入如下命令，实现实时预览

```
$ gitbook serve
$ gitbook serve ./{book_name}
```

`gitbook serve` 命令实际会先调用 `gitbook build` 编译书籍，完成后打开 web 服务器，默认监听本地 4000 端口，在浏览器打开 [http://localhost:4000](http://localhost:4000/) 即可浏览电子书。

### 编译电子书

```
$ gitbook build
$ gitbook build ./{book_name} --output=./{outputFolde}
$ gitbook build ./ --log=debug --debug
```

当电子书内容制作好之后，可以使用如下命令来生成 HTML 静态网页版电子书。该命令会在当前文件夹中生成 `_book` 文件夹，这个文件夹中的内容就是静态网页版电子书。

使用 `--log=debug --debug` 可以用来调试，会打印出 stack trace。



## F&Q

暂无

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a> 本作品采用 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享 署名-相同方式共享 4.0协议</a> 进行许可。