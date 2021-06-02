
## 特别声明及操作步骤: 
原脚本被举报，新建大家低调使用,可以直接下载本库文件后将自己的库.workflows里面的文件一次性替换即可。
hajiuhajiu




### 一丶Github Action 使用教程
方法一：

1.注册github账号 

2.导入新仓库
[点击导入仓库](https://github.com/new/import)

Your old repository’s clone URL 填入 https://github.com/hajiuhajiu1/jdsign1112 ，Your new repository details处填写导入后自己的repository名称，其它按默认，
点击Begin import，等待导入完成。

3.填写Cookie及互助码:导入完成后打开新导入的repository，在屏幕右上角找到
Settings的按钮并点击，然后左侧找到secrets点击，点右侧的new repository secrets，输入secrets name: JD_COOKIE，value 里填写获得的cookie
互助码自行填写在Secrets里，参考环境变量合集, 填写后先给自己填写的助力码助力，然后给脚本默认的助力码助力，可以自行将脚本内置的助力码去除， 或改变运行时间，自行手动助力完成后再运行脚本， 运行时间找.github\workflows目录下面对应的 yml后缀文件， 16：00对应北京时间零点。

[获取京东Cookies教程](https://github.com/hajiuhajiu1/code/blob/main/doc/GetJdCookie.md)

环境变量合集（Secrets）配置[点击查看](https://github.com/hajiuhajiu1/code/blob/main/doc/githubAction.md)

前面完成之后，点击一下右上角的 star（fork 左边那个），让 workflow 运行一次，后续脚本会按workflow默认的时间每天自动运行，需要定期更新cookie。
该方法需要手动替换或更新脚本，不会同步上游，但方法简单，可以自行选择需要运行的脚本，自己定义运行时间。



自动同步教程：
1. [按照这个教程进行 reposync](backup/reposync.md)
2. 再在`Settings`-`Secrets`里面添加`JD_COOKIE`
3. 多条 cookie 用`&`隔开或者分行，支持无数条 cookie，cookie格式pt_key=xxx;pt_pin=;,需要保证两个都有，
4. 前三步之后，点击一下右上角的 star（fork 左边那个），让 workflow 运行一次。
5. 互助码自行填写在Secrets里， 填写后先给自己填写的助力码助力，然后给脚本默认的助力码助力，可以自行将脚本内置的助力码去除， 或改变运行时间，自行手动助力完成后再运行脚本，
运行时间找.github\workflows目录下面对应的 yml后缀文件， 16：00对应北京时间零点。

喜马拉雅极速版专属环境变量[点击查看](backup/xmly/xmly.md)

>可以运行获取getcookie脚本的脚本，必须先配置微信推送后按github action：build里面运行提示用手机京东扫码登陆，脚本会自动获得cookie，然后推送到微信的消息，放在secrets即可。
>  如何配置,可参考 > [获取京东Cookies教程](https://github.com/hajiuhajiu/jdsign1112/blob/master/backUp/GetJdCookie2.md)
>
> 
> 
