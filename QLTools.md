## Docker启动
# 创建QLTools目录并进入
mkdir qltools && cd qltools

# Docker版本提供架构：amd64、arm64、arm-7
docker run --restart=always -itd --name QLTools -v $PWD/config:/QLTools/config -v $PWD/plugin:/QLTools/plugin -p 15000:15000 nuanxinqing123/qltools:latest

# 更新步骤：
后台点击更新，稍等5分钟左右。手动重启容器即可完成更新（如果更新失败，请删除容器和镜像，然后重新拉取镜像启动）
# 重启命令：
docker restart QLTools
