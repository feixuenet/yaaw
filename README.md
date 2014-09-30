YAAW
====

一个在纯 HTML/CSS/Javascirpt 环境下运行的aria2 web控制端.

不需要HTTP服务器,你需要的只是一个浏览器.

<br />

使用方法
-----
1. 开启aria2 以及RPC开启,使用如下命令
> aria2c --enable-rpc --rpc-listen-all=true --rpc-allow-origin-all
>
> 警告: 开启本选项会使请求不被校验. 你需要小心保管您的地址.

2. 打开 **index.html**.

3. 如果出现服务器内部错误,请修改JSON-RPC 地址

提示
----
* 你的所有设置都被保存在浏览器缓存中. **如果aria2被重启,所有设置都会被重置.**
* 任务列表(包含未完成的任务) 将会在aria2重启后丢失. 使用 `--save-session=SOME/WHERE` 来保存|并且使用 `--continue=true --input-file=SOME/WHERE` 来恢复任务.
* 使用 `$HOME/.aria2/aria2.conf` 来保存你的设置.
* 如果你需要更多的信息, 访问 [Aria2 用户手册](http://aria2.sourceforge.net/manual/en/html/)

本项目使用了以下组件
----------
+ [Bootstrap](http://twitter.github.com/bootstrap/)
+ [mustache.js](https://github.com/janl/mustache.js)
+ [jQuery](http://jquery.com/)
+ [jQuery Storage](http://archive.plugins.jquery.com/project/html5Storage)
+ [JSON RPC 2.0 jQuery Plugin](https://github.com/datagraph/jquery-jsonrpc)

License
-------
yaaw is licensed under GNU Lesser General Public License.
You may get a copy of the GNU Lesser General Public License from http://www.gnu.org/licenses/lgpl.txt

favicon.ico by [fangke](http://fangke.im/)
