KDC（Key Distribution Center）= 密钥分发中心
KDC（Key Distribution Center）：是默认安装在DC（域控制器）上Kerberos的主要服务，负责发行票据。
AS认证服务和TGS服务是被包含在KDC中的
TGS（Ticket Granting Service）= 票据发放服务
AS（Authentication Service）= 认证用户的身份，并为其发放TGT的服务
TGT（Ticket Granting Ticket）= TGT认证票据，由AS服务发放



用户->AS 提交信息
AS->用户 返回TGT票据

用户->TGS 提交TGT
TGS->用户 返回ST票据

用户->win7 提交ST票据
win7->用户 登录成功


AS服务是用来验证用户身份的，TGS服务是用来验证用户是否可以访问Win7的

# AS认证

用户从KDC拿到TGT的过程
AS_REQ 客户端请求包
AS_REP KDC响应包


