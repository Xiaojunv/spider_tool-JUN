下载地址：
蓝奏：https://wws.lanzous.com/b01hk5stg  密码:2ihv
百度云：https://pan.baidu.com/s/1wPjTR7jyM5VAxN-10yd45Q 提取码：mszl
GitHub：https://github.com/Xiaojunv/spider_tool-JUN
 

1.地址url: 字面意思，输入需要请求的接口地址，或网址必须为 http:// 或 https:// 开头 不能直接输入比如：www.baidu.com

 

2.请求方法: 目前只添加了最常用的get请求和post请求,选择哪个根据地址需要的请求方法来选，如果后期有其他请求方法需求可以再加

 

3.提交：emmm...这个就不多说了，填写好所有需要的参数后提交即可返回对应的数据，提示：如果一些必要参数没有填写会有弹框提示

 

4.全部清空：把填写的所有内容清空，包括返回的文本

 

5.IP代理：目前只支持 ip:端口这种格式 例如：192.168.0.1:0000  暂时只支持单个，后期会改进使用多个

 

6.随机ua:这个是请求头里的随机UserAgent参数，目前只支持随机谷歌chrome ua，如果请求头只想加入一个UserAgent就能访问的话，

勾选此项就不用再填写请求头文本框内的参数，这个挺方便的

7.禁止重定向：顾名思义，就是不让地址进行重定向请求，只返回请求未重定向的响应文本，多在请求登录接口上使用

8.关闭SSL验证：这个的话多用于app接口上使用，如果响应文本报错SSL，那就勾选此项吧

9.响应解码：添加了目前最常用的utf-8和gbk 对响应文本的编码设置默认utf-8

10.生成代码：返回Python对应已调试选择好的代码，需要在python环境下运行，依赖包   pip install requests    只生成到了响应数据那块，至于正则/xpath提数那块自定义比较多，暂时没做

 

 

 11.请求头request_haders: 请求地址url的请求头，目前支持两种格式，一种是直接从网页上复制下来的，另一种是在代码中使用的字典格式

本人觉得直接网站复制下的功能方便= =字典毕竟还得手动加""引号，如果只需要加个User-Agent就能访问的话建议勾选随机ua功能，不用填写此文本框

 

##第一种
Host: www.cnblogs.com
Referer: https://www.cnblogs.com/
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36
##第二种
{"Host": "www.cnblogs.com","User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36"}
 

12.cookies: 网页上的cookie对应值直接复制到文本框即可，不需要再加字典的key值

13.请求参数：这个是方便看url地址中请求的参数，也就是地址中 ?后的参数，目前此文本框只做展示，修改对请求地址url无效

 

https://xxxxx?q=js
 

14.请求体From_data：目前多用于post请求方法中的请求参数，同请求头一样支持2种格式    注：大多Get请求的参数放在url地址中，POST请求放置于请求体中

 

15.响应文本：请求地址返回的响应后台源数据，也就是响应文本，后期会加入搜索功能，现在还在开发中

16.响应头：响应回的headers参数，目前只做展示，内容同谷歌开发者中网络请求响应头的内容差不多一致

17.xpath/正则：对响应文本内容进行提取，默认xpath，输入对应的语法即可

 

特别说明下：如果请求参数不对或者地址不对，请求超时之类的，提交请求后响应文本会返回对应的Python报错内容，看不懂报错内容可直接百度搜索

使用技术：Python3.6    requests   Pyqt5  lxml  re剩下的就是功能代码

 

##以上为功能介绍和使用说，如果有好的idea可联系我，联系方式在软件中

........emmm因作者迫于生活贫穷 如果此软件有帮助到你的话可以给作者送丢丢温暖

