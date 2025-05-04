# 安装软件问题
下载之后直接安装即可，此时打开会报错：Picgo.app 文件已损坏，您应该将它移到废纸篓。

这是因为 macOS 为了保护用户不受恶意软件的攻击，macOS 会阻止安装未经过苹果认证的应用程

此时只需要在命令行中执行一个命令即可：
```
sudo xattr -d com.apple.quarantine "/Applications/PicGo.app"
```
执行完成后，再打开 Picgo.app 就可以正常使用了。