# 小红书爬取无水印图片

在使用之前，登录网页版小红书获取cookie

简单使用正则获取traceId：`trace_id = re.findall(r'"traceId":"[a-zA-Z0-9]+"', r.text)`

## 代理设置
如有需要可以设置代理

```Python
# set proxy if do not need, just comment this line
    proxy = 'http://127.0.0.1:7891'  # clash proxy, works for windows
    r = requests.get(url, stream=True,
                     proxies={'http': proxy, 'https': proxy}, verify=False)
```
