在django1.9里，urls的配置不再支持字符串型的路由。需要先import，然后直接引用。更加清晰。比如：

在django1.9里，urls的配置不再支持字符串型的路由。需要先import，然后直接引用。更加清晰。



比如：

urlpatterns = patterns\('',

 url\(r'^test\/', 'httpServer.views.hello.test'\), \# 注意，字符串形式

\)

