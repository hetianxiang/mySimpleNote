Ajax：async javascript and xml 异步的JS和XML

->客户端JS中的方法，用来向服务器端发送请求(还可以传递给服务器端数据)，然后把服务器端返回的内容获取到(Ajax一般是运行在客户端的浏览器中的)

AJAX四步:

->创建一个AJAX对象(下面的这种写法在IE6及更低版本的浏览器中不支持)
var xhr=new XMLHttpRequest;
->发送前的基本信息配置:

配置请求方式(GET、POST、PUT、DELETE、HEAD...)
打开一个URL地址(配置向哪一个服务器地址发送请求)
同步还是异步(true代表异步 false代表同步 默认是true)
[username]向服务器提供请求的用户名
[userpass]向服务器提供请求的用户密码 这两个值一般都不写，只有服务器做了安全的限制，只允许特定的用户访问的话，我们才传递过去 xhr.open("get","/data.txt",false,[username],[userpass]);

->给onreadystatechange这个事件绑定一个方法,监听状态的改变(只要状态改变，就出触发方法执行)