---
layout:     post
title:      Linux下安装nodejs环境
category: blog
description: Linux下安装nodejs环境。
---

## Linux下安装nodejs环境

<h3>摸了一早上坑,在新的一个机器上安装nodejs环境

1.利用yum安装wget<br/>
	<code>[root@lin-21-4-97 ~]# yum install wget</code><br/>
2.利用wget下载最新的node版本,[复制下载地址](https://nodejs.org/en/download/)<br/>
<code>cd /tmp<br/>
[root@lin-21-4-97 tmp]# wget https://nodejs.org/dist/v4.4.5/node-v4.4.5-linux-x64.tar.xz</code><br/>
3.解压下载下来的nodejs安装包node-v4.4.5-linux-x64.tar.xz,先下载xz,先用xz解压下载下来的.xz文件生成.tar文件,再用tar工具解压tar文件<br/>
<code>yum install xz -y<br/>
xz -d node-v4.4.5-linux-x64.tar.xz<br />
tar -xvf node-v4.4.5-linux-x64.tar
</code><br/>
4.配置环境变量<br/>
进入编辑:<code>vim /etc/profile<br/></code>
在内容的最后添加:<code>export NODE_HOME=/usr/local/node-v4.4.5-linux-x64(你的node最终解压后的地址)<br/>
export PATH=$PATH:$NODE_HOME/bin<br/>
export NODE_PATH=$NODE_HOME/lib/node_modules<br/></code>
验证配置:<code>source /etc/profile</code><br/>
安装成功:<code>[root@lin-21-4-97 tmp]# node -v
v4.4.5</code>


