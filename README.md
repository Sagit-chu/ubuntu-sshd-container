# Docker Debian/GNU Linux with OpenSSH-Server
 修改自ilemonrain/debian-sshd，更新为Debian11
- **0.更新说明**
**sagitchu/debian-sshd** Update 20220623   
 - 重新设计架构，为以后的部署做准备
 - 设置默认语言为 zh_CN.UTF8 (但实际上界面还是英文)  
 - 设置默认时区为 Asia/Shanghai (UTC+8)    

- **2. 镜像介绍**
本镜像，基于官方Debian Docker镜像制作，集成了OpenSSH-Server用于远程连接，快速部署环境

- **3. 食用说明**  
How To 拉取镜像：**docker pull sagitchu/debian-sshd:latest** 

How To 运行镜像：**docker run -d -p 22:22 --name=debian-sshd sagitchu/debian-sshd:latest**  

**参数基础格式**：docker run -d **-p 22:22** **-name=debian-sshd** sagitchu/debian-sshd:latest  

**-p 22:22**：端口映射，冒号前面的是外部端口，冒号后面的为内部端口，根据自己需要自行部署（比如要部署个Nginx，那就是“**-p 22:22 -p 80:80**”）

**--name=debian-sshd**：容器名称，自行确定，也可以省略（但不方便以后管理）

**登录用户名：root 密码：sagitpass**
**！！！部署成功后立刻改掉ROOT密码！！！**  
**！！！部署成功后立刻改掉ROOT密码！！！**  
**！！！部署成功后立刻改掉ROOT密码！！！**  
**！！！重要的事情说三遍！！！**  
**！！！因不改ROOT密码导致容器出现问题，概不负责！！！**  


