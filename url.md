在django1.9里，urls的配置不再支持字符串型的路由。需要先import，然后直接引用。更加清晰。

```
urlpatterns = patterns('',

    url(r'^test/', 'httpServer.views.hello.test'), # 注意，字符串形式

)
```

Ajax 测试

```
$(function(){
        $.ajax({
                type: 'getJson',//请求类型
                url: 'data_math/',
                data: '',
                timeout: 10000,//链接超时时间（毫秒）
                error: function (XMLHttpRequest, Status, errorThrown) {
                    alert('数据传递错误，请检查返回数据问题！');

                },
                success: function (data) {
                    alert(data)
                }
            })
        });
```

Json数据打包

