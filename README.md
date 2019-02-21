# 问题描述
sublime package control 无法安装

# 出现原因
`packagecontrol.io` 地址被墙

# 安装package control
> 使用浏览器打开[package control](https://github.com/wbond/package_control/releases) <br />
> 选择一个版本[下载](https://github.com/wbond/package_control/archive/3.3.0.zip) <br />
> 打开sublime，选择`Preferences` --> `Browse Packages..` <br />
> 将下载的压缩包解压到当前目录，修改文件目录为`Package Control` <br />
> 重新打开sublime可以看到package control已安装

# 无法下载插件
> 打开`sublime`，选择`Preferences` --> `Package Settings` --> `Package Control` --> `Settings - User` <br />
> 修改`channels`数组，增加镜像json
```
"channels":
	[
		"http://cst.stu.126.net/u/json/cms/channel_v3.json",
		"https://gist.githubusercontent.com/nick1m/660ed046a096dae0b0ab/raw/e6e9e23a0bb48b44537f61025fbc359f8d586eb4/channel_v3.json",
		"https://packagecontrol.io/channel_v3.json"
	],
```
> 重新打开`sublime`可以正常搜索插件，正常下载

# 建议
如可以登陆`packagecontrol.io`建议提前下载一份官方json，存放到本地或网络，需要时设置成自己的文件路径即可。防止别人的json也被墙
