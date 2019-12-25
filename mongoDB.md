# MongoDB 学习
```shell
# mongoDB社区版下载链接
#https://www.mongodb.com/download-center/community
# 创建持久化数据存储目录
mkdir -p /data/{db,log}
cd /data
# 下载 mongoDB
wget https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-ubuntu1804-4.2.2.tgz
# 安装
tar -xzvf mongodb-linux-x86_64-ubuntu1804-4.2.2.tgz
# 配置环境变量
export PATH=$PATH:/data/mongodb-linux-x86_64-ubuntu1804-4.2.2/bin
# 启动mongod server
mongod --dbpath /data/db --port 27017 --logpath /data/log/mongod.log --fork
# 恢复mongoDB数据
mongorestore
```