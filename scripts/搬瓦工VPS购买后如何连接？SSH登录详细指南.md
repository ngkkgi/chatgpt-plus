# 搬瓦工VPS购买后如何连接？SSH登录详细指南

在购买搬瓦工VPS后，许多新手用户面临的首要问题是如何连接和使用这台远程服务器。本文将详细介绍通过SSH工具登录搬瓦工VPS的完整步骤。

## 一、获取SSH登录凭证

连接VPS需要以下三个关键信息：

1. **IP地址** - 服务器的唯一网络标识
2. **SSH端口** - 默认22端口，搬瓦工通常使用5位数字端口
3. **SSH密码** - 通常使用root账户密码

这些信息会在购买成功后通过邮件发送。若未收到，可通过KiwiVM控制面板重新获取。

👉 [【点击查看】2025年最新BandwagonHost搬瓦工优惠码及特价云服务器方案汇总](https://bit.ly/banwagon)

## 二、各平台SSH连接方法

### Windows系统连接方案

推荐使用以下SSH客户端：
- Xshell（功能全面）
- Git Bash（轻量级）
- Putty（经典工具）

连接步骤：
1. 打开SSH客户端
2. 输入IP地址和端口
3. 使用root账户和密码登录

### macOS系统连接方法

macOS用户可直接使用终端工具：
1. 打开终端（Command+空格搜索）
2. 输入命令：
   bash
   ssh root@ip_address -p ssh_port
   
3. 输入密码完成验证

### Linux系统连接

Linux用户可直接使用系统终端：
bash
ssh root@ip_address -p ssh_port

### 移动设备连接方案

- **Android**：推荐JuiceSSH应用
- **iOS/iPadOS**：Termius是优秀选择

## 三、常见问题解答

Q：连接时提示"Connection refused"怎么办？
A：检查IP和端口是否正确，确认VPS运行状态

Q：忘记root密码如何处理？
A：通过KiwiVM控制面板重置密码

Q：如何提高SSH安全性？
A：建议：
- 修改默认SSH端口
- 使用密钥认证替代密码
- 启用防火墙规则

通过以上步骤，您应该能够顺利连接搬瓦工VPS。如需更多帮助，可以参考官方文档或社区支持。