# 压缩解压
gzip：压缩.gz文件
```
gzip [file]

>> 只能压缩文件，不能压缩目录
>> 压缩后不保留原文件
```

gunzip / gzip -d：解压.gz文件
```
gunzip [zipfile]
```
tar：打包目录，压缩成.tar.gz文件
```
tar [-zcfv] [zipfile] [dirctory]

-c 打包     -v 显示详细信息     -f 指定文件名      -z 打包同时压缩
$ tar -zcf zipfile dir
```

```
解压缩
-x 解包     -v 显示详细信息     -f 指定解压文件     -z 解压缩
$ tar -zxvf zipfile.tar.gz
```
zip：压缩文件或目录，.zip格式
```
zip [-r] [zipfile] [file/dir]

-r 压缩目录

>> 唯一linux和windows都支持的压缩格式
>> 保留原文件且可以压缩目录
```
unzip：解压.zip压缩文件
```
unzip [zipfile]
```
bzip2：压缩文件，.bz2格式
```
bzip2 [-k] [file]

-k：产生压缩文件后保留原文件
```
bunzip2：解压缩
```

```
# ifconfig
查看当前网卡状态
```
ifconfig [网卡名称] [IP address]
```
# shutdown
```
shutdown [-chr] [time]

-c：取消前一个关机命令
-h：关机
-r：重启

$ shutdown -h now     # 现在关机

>> shutdown会在关机之前保存正在运行的服务
```
- 系统运行级别
  - 0 关机
  - 1 单用户
  - 3 完全多用户
  - 5 图形界面
  - 6 重启 
