# node-server
nodejs 服务器


```
var routes = {
  '/search': function(req, res){
    res.end('username='+req.body.username+',password='+req.body.password)
  }
}
```
```
<form action="/search" method="POST">
    <input type="text" name="username" value="1">
    <input type="text" name="password" value="2">
    <input type="submit" value="search">
  </form>
```
search 获取input中的值


```
  var xhr = new XMLHttpRequest()
  xhr.open('GET', '/a.json', true)
  xhr.send()
  xhr.onload = function(){
    console.log(xhr.responseText)
  }
```
读取a.json