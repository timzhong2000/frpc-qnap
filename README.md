# Frpc-QNAP

使用 QDK 为威联通系统打包 frpc

## 配置

启动命令为：

```
frpc --config_dir /shared/homes/admin/frpc/
```

添加配置文件的方式有两种：

1. (命令行模式) 你需要在`/shared/homes/admin/frpc/`下按照 frpc 的配置格式创建配置文件。
2. (网页模式) 使用 admin 账户登录威联通 Web 管理页面，在 home 下创建 frpc 文件夹并且在里面创建配置文件。

注意，可以放置多个文件，这样可以连接到多个 frp 服务器。

## 编译

在当前目录执行 `qbuild` 进行打包，打包后安装包在 `build/frpc_<version>_<arch>.qpkg`

## 安装

在威联通系统中打开 App Center，点击右上角安装，选择上一步编译好的 qpkg 文件，安装完成。

## TODO
- [ ] 创建Release
- [ ] 编写详细的使用文档
- [ ] 在amd64和arm64架构上进行测试