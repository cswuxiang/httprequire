# httprequire
node中加载线上资源文件

##案例
1、同步加载：

var httprequire = require("./httprequire.js");<br>
var app = httprequire("http://lowinwu.com/www/myspa/res/js/scripts/app.js");

app.init();


2、异步加载

var httprequire = require("./httprequire.js");<br>
httprequire("http://lowinwu.com/www/myspa/res/js/scripts/app.js"，function(app){
   app.init()
});;
