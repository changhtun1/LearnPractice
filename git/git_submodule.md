


## 1 在一个已存在的git仓库添加子模块。
```
git submodule add url地址 [其他路径或者名称]
```
执行此命令后会增加一个.gitmoduls文件和子项目文件夹。

## 2 克隆含有子模块的项目
克隆项目：
```
git clone pro_url
```
默认包含子模块目录，但是没有任何文件。
初始化本地配置文件：
```
git submodule init
```

从该项目中抓取所有数据并检出父项目中列出的合适的提交：
更新项目内子模块到最新版本
```
git submodule update
```



# 问题：
```bash
zhangxin@zhangxin-ThinkPad-L480:/media/zhangxin/Data/github/slambook2$ git submodule init
error: chmod on /media/zhangxin/Data/github/slambook2/.git/config.lock failed: Operation not permitted
Failed to register url for submodule path '3rdparty/DBoW3'
```

解决方法：
挂载磁盘权限问题

