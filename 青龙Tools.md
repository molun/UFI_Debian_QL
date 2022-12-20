青龙Tools 正式版【V2.2】
----------------------------------------
提问题的艺术：
出现解决不了的错误，第一步先查看运行日志。如果根据日志错误提示依然无法结论。那么请带上日志错误截图咨询水友。再解决不了，请在TG带上日志询问作者。仓库提交issues时不推荐携带日志文件
----------------------------------------
更新说明：

Tips：如果无法自动创建config文件，请下载config.zip解压到程序同目录
1、修复 变量上传的稳定性
2、修复 插件创建流程错误
3、新增 合并模式换行符分割
4、优化 前端描述文档修改
----------------------------------------
安装：
Tips：中国大陆服务器热更新需要配置Github代理，否则必失败
Tips：删除config目录里面的app.db文件就相当于重装青龙Tools

方式一、直接部署 & 守护

安装地址：https://github.com/nuanxinqing123/QLTools#安装教程

方式二、Docker

# 创建QLTools目录并进入
mkdir qltools && cd qltools

# Docker版本提供架构：amd64、arm64、arm-7
docker run --restart=always -itd --name QLTools -v $PWD/config:/QLTools/config -v $PWD/plugin:/QLTools/plugin -p 15000:15000 nuanxinqing123/qltools:latest

# 注意事项：Docker部署将从v1.7正式版全面支持热更新（v1.6以及以前版本需要手动升级）
# 更新步骤：后台点击更新，稍等5分钟左右。手动重启容器即可完成更新（如果更新失败，请删除容器和镜像，然后重新拉取镜像启动）
# 更新镜像：docker pull nuanxinqing123/qltools:latest
# 重启命令：docker restart QLTools
----------------------------------------
后台信息：
登录地址：IP或域名:15000/#/login
注册地址：IP或域名:15000/#/register
后台地址：IP或域名:15000/#/admin
----------------------------------------
仓库地址：https://github.com/nuanxinqing123/QLTools
开发计划：https://web.banlikanban.com/kanban/626f9b4c6ade1220282ac551
提交Bug：https://github.com/nuanxinqing123/QLTools/issues
插件库：http://plugin.6b7.org
插件开发文档：https://github.com/nuanxinqing123/QLTools/blob/master/Plugin.md
进程守护&反代：https://6b7.org/460.html
----------------------------------------
Github代理站：
https://ghproxy.com
https://toolwa.com/github
