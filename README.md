# deploy-tidb-on-cloud
TiDB Hackathon Project

# 团队介绍
公司内部员工组建的一个重在参与的团队 :P

# 项目介绍
提供一个可视化的平台界面，让用户可以轻松将 TiDB 实例部署上云。

# 动机&背景

  在早期的 TiDB 生态中，没有专门的包管理工具，使用者只能通过相应的配置文件和文件夹命名来手动管理，如 Prometheus 等第三方监控报表工具甚至需要额外的特殊管理，这样大大提升了运维管理难度。


  从 TiDB 4.0 版本开始，TiUP 作为新的工具，承担着包管理器的角色，管理着 TiDB 生态下众多的组件，如 TiDB、PD、TiKV 等。用户想要运行 TiDB 生态中任何组件时，只需要执行 TiUP 一行命令即可，相比以前，极大地降低了管理难度。在公有云平台，如果用户想用 TiUP 工具部署一套 TiDB环境，难免需要繁杂地操作来申请各种 IaaS 资源，为了让用户可以更轻松地在公有云环境使用虚拟机部署 TiDB, 我们提供一个可视化的集成运维平台，帮助用户轻松部署云上 TiDB.
  
# 项目设计
## 1. 账号管理
用户使用账号登陆平台，管理公有云账户

## 2. 创建 TiDB 集群
通过用户输入的 Vendor、Region、Zone, 产品规格等信息，在对应的区域申请资源并打通 TiUP 工具创建集群

## 3. 查看集群信息
在集群页面可以查看创建的 TiDB 集群列表和详情

## 4. 查看资源信息
在资源页面可以查看当前已使用的资源详情

## 5. 账单计量
统计当前已使用的公有云资源计量信息
