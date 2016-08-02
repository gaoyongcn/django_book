# ajax

---

```py
$.getJSON('{% url 'test' %}', function(ret) {
        $.each(ret, function(i,item){
            // i 为索引，item为遍历值
            alert(i)
            alert(item)
        });
    });
```



