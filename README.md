##Hexo-blog-base是什么?
基于hexo的个人博客配置工程，包含基本的配置

向hexo作者致敬

##如何使用？

* 安装git
    * [Windows下安装Git](http://jingyan.baidu.com/article/90895e0fb3495f64ed6b0b50.html)
* 安装[node-js](https://nodejs.org/en/)
* 安装Hexo
    * 打开Git Bash
    * 执行如下命令: [npm install -g hexo]
    * 跳过命令: [hexo init]
* Clone本工程到指定repo目录中
    * git clone https://github.com/blogpage/hexo-blog-base.git
* 解压缩node_modules.7z文件到根目录
* 修改_config.yml文件配置
* 修改.travis.yml配置
* 修改source目录下的CNAME文件，设置为绑定的域名
* 执行生成提交命令: [heox d -g]

## Travis CI自动化部署
* 安装ruby环境，修改gem sources到ruby-china，安装travis
* Windows下打开cmd工具，使用Personal Access Tokens的方式加密提交
* 执行如下命令：
```javascript
  travis login --auto #如果返回登录失败，清理Personal Access Tokens中的记录即可
  travis encrypt 'GH_TOKEN=<Tokens>' --add #会在.travis.yml文件中添加secure值（如果文件为空，添加到env-global下，反之在dd下）
``` 
* 在[travis](https://travis-ci.org)对应的项目设置中，添加GH_TOKEN键值对


##有问题反馈
在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

* E-Mail: (638781#qq.com, 把#换成@)
* QQ: 638781
* BLOG: [@一座城池](http://isuhao.cn)

##感激
感谢以下的项目,排名不分先后

* [hexo](http://isuhao.cn/) 
* [source](http://blog.sc/)
* [sites](http://sites.so)

##关于作者

```javascript
  var isuhao = {
    Name  : "苏豪",
    site : "http://suhao.org"
  }
```
