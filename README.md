# Examples

<img align="right" width="150px" src="https://iris-go.com/images/logo.svg?v=10">

<a href="https://travis-ci.org/iris-contrib/examples"><img src="https://img.shields.io/travis/iris-contrib/examples.svg?style=flat-square" alt="Build Status"></a>
<a href="https://github.com/iris-contrib/examples/blob/master/LICENSE"><img src="https://img.shields.io/badge/%20license-MIT%20%20License%20-E91E63.svg?style=flat-square" alt="License"></a>
<a href="https://github.com/kataras/iris/blob/master/HISTORY.md"><img src="https://img.shields.io/badge/version-10.x%20-blue.svg?style=flat-square" alt="CHANGELOG/HISTORY"></a>

This repository provides easy to understand code snippets on how to get started with web development with the Go programming language using the [Iris](https://github.com/kataras/iris) web framework.

It doesn't contain "best ways" neither explains all its features. It's just a simple, practical cookbook for young Gophers!
```
每个示例编译时最好用终端单独编译，或者用IDE单独打开每一个示例进行编译运行，否则会出现VIEW找不到的情况
```

## Table of Contents

* [Overview](overview)
    * [Hello world!](hello-world/main.go)
    * [Hello WebAssemply!](webassembly/basic/main.go) **NEW**
    * [Glimpse](overview/main.go)
    * [Tutorial: Online Visitors](tutorial/online-visitors/main.go)
    * [Tutorial: URL Shortener using BoltDB](tutorial/url-shortener/main.go)
    * [Tutorial: DropzoneJS + Go: How to build a file upload form](tutorial/dropzonejs/main.go)
    * [Tutorial:Iris Go Framework + MongoDB](https://medium.com/go-language/iris-go-framework-mongodb-552e349eab9c)
* [快速构建](structuring)
    * [引导||构建模板](structuring/bootstrap/bootstrap/bootstrapper.go)
    * [带有存储库和服务层概述的MVC](mvc/overview/main.go)
    * [Login (MVC with Single Responsibility package)](structuring/login-mvc-single-responsible-package/main.go)
    * [Login (MVC 使用Datamodels，Datasource，Repository和Service层)](mvc/login/main.go)
* [HTTP 服务](http-listening)
    * [启动 && 监听端口](http-listening/listen-addr/main.go)
    * [UNIX 套接字](http-listening/listen-unix/main.go)
    * [TLS](http-listening/listen-tls/main.go)
    * [Letsencrypt (Automatic 自动认证)](http-listening/listen-letsencrypt/main.go)
    * [使用自定义监听器](http-listening/custom-listener/main.go)
    * [适用于unix系统的SO_REUSEPORT](http-listening/custom-listener/unix-reuseport/main.go)
    * [省略服务器错误](http-listening/listen-addr/omit-server-errors/main.go)
    * [自定义HTTP 服务](http-listening/custom-httpserver/easy-way/main.go)
    * [自定义 HTTP Server (STD)](http-listening/custom-httpserver/std-way/main.go)
    * [多个 HTTP Servers](http-listening/custom-httpserver/multi/main.go)
    * [优雅关闭](http-listening/graceful-shutdown/default-notifier/main.go)
* [配置](configuration)
    * [函数式配置](configuration/functional/main.go)
    * [结构体式配置](configuration/from-configuration-structure/main.go)
    * [从YAML加载配置](configuration/from-yaml-file/main.go)
        * [Share Configuration between multiple instances](configuration/from-yaml-file/shared-configuration/main.go)
    * [从TOML加载配置](configuration/from-toml-file/main.go)
* [路由](routing)
    * [总体示例](routing/overview/main.go)
    * [基础示例](routing/basic/main.go)
    * [自定义 HTTP 错误](routing/http-errors/main.go)
    * [动态请求地址](routing/dynamic-path/main.go)
    * [根级别通配符](routing/dynamic-path/root-wildcard/main.go)
    * [反向路由](routing/reverse/main.go)
    * [自定义封装](routing/custom-wrapper/main.go)
    * [路由状态](routing/route-state/main.go)
* [Hero](hero)
    * [Basic](hero/basic/main.go)
    * [Overview](hero/overview/main.go)
* [MVC](mvc)
    * [Hello world](mvc/hello-world/main.go) **UPDATED**
    * [Session Controller](mvc/session-controller/main.go) **UPDATED**
    * [Overview - 加上存储库和服务层](mvc/overview/main.go) **UPDATED**
    * [Login 示例 - 加上存储库和服务层](mvc/login/web/main.go) **UPDATED**
    * [单例模式](mvc/singleton/main.go) **NEW**
    * [Websocket Controller](mvc/websocket/main.go) **NEW**
    * [Vue.js Todo MVC](tutorial/vuejs-todo-mvc/src/web/main.go) **NEW**
* [自定义 Context](routing/custom-context)
    * [重写Method](routing/custom-context/method-overriding/main.go)
    * [新实现](routing/custom-context/new-implementation/main.go)
* [转换 http.Handler](convert-handlers)
    * [From func(http.ResponseWriter, *http.Request, http.HandlerFunc)](convert-handlers/negroni-like/main.go)
    * [From http.Handler or http.HandlerFunc](convert-handlers/nethttp/main.go)
* [子域](subdomains)
    * [单个](subdomains/single/main.go)
    * [多个](subdomains/multi/main.go)
    * [通配符](subdomains/wildcard/main.go)
    * [WWW](subdomains/www/main.go)
* [视图](view)
    * [整体示例](view/overview/main.go)
    * [Hi](view/template_html_0/main.go)
    * [单个布局示例](view/template_html_1/main.go)
    * [布局: `yield` and `render` tmpl 函数](view/template_html_2/main.go)
    * [The `urlpath` tmpl 函数](view/template_html_3/main.go)
    * [The `url` tmpl 函数](view/template_html_4/main.go)
    * [在处理程序之间注入数据](view/context-view-data/main.go)
    * [将模板嵌入到App可执行文件中](view/embedding-templates-into-app/main.go)
    * [自定义一个 `io.Writer`](view/write-to/main.go)
    * [使用 (Jade)模板`](view/template_pug_0/main.go)
    * [Pug (Jade) Actions`](view/template_pug_1/main.go)
    * [Pug (Jade) Includes`](view/template_pug_2/main.go)
    * [Pug (Jade) Extends`](view/template_pug_3/main.go)
* [认证](authentication)
    * [基础认证](authentication/basicauth/main.go)
    * [OAUth2](authentication/oauth2/main.go)
    * [JWT](experimental-handlers/jwt/simple/main.go)
* [文件服务](file-server)
    * [Favicon](file-server/favicon/main.go)
    * [基础服务](file-server/basic/main.go)
    * [启动文件服务](file-server/embedding-files-into-app/main.go)
    * [在文件服务中启动GZIP ](file-server/embedding-gziped-files-into-app/main.go) **NEW**
    * [发送或下载文件](file-server/send-files/main.go)
* [单页应用](file-server/single-page-application)
    * [单页应用](file-server/single-page-application/basic/main.go)
    * [启动单页应用](file-server/single-page-application/embedded-single-page-application/main.go)
* [怎么读取 *http.Request`](http_reqest)
    * [取值：JSON](http_request/read-json/main.go)
    * [从 Form 取值](http_request/read-form/main.go)
    * [从upload中读取数据](http_request/upload-files/main.go)
* [怎么调用 http.ResponseWriter](http_responsewriter)
	* [输出到 `valyala/quicktemplate` 模板](http_responsewriter/quicktemplate/main.go)
    * [输出Text, Markdown, HTML, JSON, JSONP, XML, Binary](http_responsewriter/write-rest/main.go)
    * [输出 Stream Writer](http_responsewriter/stream-writer/main.go)
    * [输出 Transactions](http_responsewriter/transactions/main.go)
    * [输出 SSE (third-party package usage for server-side events)](http_responsewriter/sse-third-party/main.go)
* [杂项](miscellaneous)
    * [访问日志](http_request/request-logger/main.go)
	* [Log Requests to a file](http_request/request-logger/request-logger-file/main.go)
    * [本地化和国际化](miscellaneous/i18n/main.go)
    * [启用recover，防止崩溃](miscellaneous/recover/main.go)
    * [性能分析 Profiling (pprof)](miscellaneous/pprof/main.go)
    * [日志 Internal Application File Logger](miscellaneous/file-logger/main.go)
    * [测试 Testing](testing/httptest/main_test.go)
    * [缓存 Caching](cache/simple/main.go)
    * [Yaag - API Automated Docs](apidoc/yaag/main.go)
* [Sessions](sessions)
    * [Overview](sessions/overview/main.go)
    * [标准示例](sessions/standalone/main.go)
    * [安全 Cookie](sessions/securecookie/main.go)
    * [传输数据](sessions/flash-messages/main.go)
    * [基于数据库](sessions/database)
        * [Badger](sessions/database/badger/main.go)
        * [Redis](sessions/database/redis/main.go)
        * [BoltDB](sessions/database/boltdb/main.go)
* [Websockets](websocket)
    * [聊天](websocket/chat/main.go)
    * [交互 Messages](websocket/native-messages/main.go)
    * [查看所有链接](websocket/connectionlist/main.go)
    * [启动 TLS ](websocket/secure/main.go)
    * [自定义Go Client](websocket/custom-go-client/main.go)
* [实验处理程序](experimental-handlers)
    * [Casbin wrapper](experimental-handlers/casbin/wrapper/main.go)
    * [Casbin middleware](experimental-handlers/casbin/middleware/main.go)
    * [Cloudwatch](experimental-handlers/cloudwatch/simple/main.go)
    * [CORS](experimental-handlers/cors/simple/main.go)
    * [JWT](experimental-handlers/jwt/main.go)
    * [Newrelic](experimental-handlers/newrelic/simple/main.go)
    * [Prometheus](experimental-handlers/prometheus/simple/main.go)
    * [Secure](experimental-handlers/secure/simple/main.go)
    * [Tollboothic](experimental-handlers/tollboothic/limit-handler/main.go)

> Do not forget to [star or watch the project](https://github.com/kataras/iris/stargazers) in order to stay updated with the latest tech trends, it takes some seconds for the sake of go!

> Examples are tested using Windows 10, Ubuntu 16.10 with [Microsoft's Visual Studio Code](https://code.visualstudio.com/) and built using the [Go 1.9](https://golang.org/dl).

## Run

1. Install the Go Programming Language, version 1.9 from [here](https://golang.org/dl).
2. Install Iris: `go get -u github.com/kataras/iris`
3. [Download the examples](https://github.com/iris-contrib/examples/archive/master.zip) and copy-paste them to your `$GOPATH/src/github.com/iris-contrib/examples`

And run

```sh
$ cd $GOPATH/src/github.com/iris-contrib/examples/overview
$ go run main.go
```

## Any troubles with examples?

    https://github.com/iris-contrib/examples/issues

## Su, 04 June 2017

This repository is just a minor of the https://github.com/kataras/iris/master/_examples folder.
