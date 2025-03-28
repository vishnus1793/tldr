# scp

> 安全的复制文件。
> 使用 SSH 上的安全复制协议在主机之间复制文件。
> 更多信息：<https://man.openbsd.org/scp>.

- 将本地文件复制到远程主机：

`scp {{路径/到/本地文件}} {{远程主机地址}}:{{路径/到/远程文件}}`

- 连接到远程主机时使用特定端口：

`scp -P {{端口}} {{路径/到/本地文件}} {{远程主机地址}}:{{路径/到/远程文件}}`

- 将文件从远程主机复制到本地目录：

`scp {{远程主机地址}}:{{路径/到/远程文件}} {{路径/到/本地目录}}`

- 递归地将目录内容从远程主机复制到本地目录：

`scp -r {{远程主机地址}}:{{路径/到/远程目录}} {{路径/到/本地目录}}`

- 通过本地主机在两个远程主机之间复制文件：

`scp -3 {{主机地址1}}:{{路径/到/远程文件}} {{主机地址2}}:{{路径/到/远程目录}}`

- 连接到远程主机时使用特定用户名：

`scp {{路径/到/本地文件}} {{远程主机用户名}}@{{远程主机地址}}:{{路径/到/远程目录}}`

- 使用特定 SSH 私钥与远程主机进行身份验证：

`scp -i {{~/.ssh/私钥文件}} {{路径/到/本地文件}} {{远程主机地址}}:{{路径/到/远程文件}}`

- 连接到远程主机时使用特定代理：

`scp -J {{代理用户名}}@{{代理主机地址}} {{路径/到/本地文件}} {{远程主机地址}}:{{路径/到/远程文件}}`
