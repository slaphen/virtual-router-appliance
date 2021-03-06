---
copyright:
  years: 1994, 2017
lastupdated: "2017-07-26"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 如何在门户网站中查看 Vyatta

在圣何塞数据中心部署了单个 1 Gbps 网关；它针对公共和专用基础架构提供冗余访问。使用**网络 > 网关设备**菜单下的**设置**选项卡以查看已部署的硬件的实际配置。

请记录 **2546 公共 VLAN**、**2576 专用 VLAN** 和**网络硬件显示详细信息**链接。网络为专用且仅包含网关设备。它们受供应平台控制（您无法通过此选项卡供应标准服务器）。

要查看联网关联，请单击 Web 门户网站中的**网络 > 网关设备**菜单。

SoftLayer 将 Brocade 5400 vRouter (Vyatta) 上的网络交换机端口和以太网适配器全都配置为中继。我们的关联仅更新端口配置以允许选中的其他虚拟 LAN (VLAN)。<sup>1</sup>

**关联 VLAN** 下拉菜单允许您选择特定 VLAN 以使其对于数据中心中的 Brocade 5400 vRouter 设备成为已知的或与之“关联”。您**无法**关联受硬件防火墙或 FortiGate 设备保护的 VLAN，因为这会打破 VLAN 的控制。如果未在下拉菜单中列出其他 VLAN，那么可通过向 Softlayer 提交凭单来订购更多。

您可以在图 4 中的“关联的 VLAN”下查看与 Brocade 5400 vRouter 设备相关联的 VLAN。缺省状态为“已绕过”（SoftLayer 已在幕后确定中继交换机端口以包含 1894 和 2254（专用）以及 2007 和 1280（公共））。<sup>2</sup>

在**详细信息**屏幕（**网络 > 网关设备**）的**关联的 VLAN > 操作**下拉菜单中，存在一个**路由 VLAN** 选项。如果选择此选项，您实际上是要求 SoftLayer FCR 和 BCR 除去缺省网关，并改为向 Brocade 5400 vRouter 设备添加使用传输 VLAN 的子网的路由。

Brocade vRouter 设备现在是进出 VLAN 的唯一有效路由。请务必记住，这不仅针对应用程序流量，还包括现在需要流经您的设备的任何其他 SoftLayer 服务。<sup>4</sup>

Brocade 5400 vRouter 端的配置尚未执行，然而包含子网的 VLAN 上的任何内容都已不再可访问。这也意味着作为 Web 门户网站供应的新服务器也无法访问 VLAN。

**注：**

<sup>1</sup>VLAN 关联是将有资格的 VLAN 链接到网关（以便未来可将其路由到该网关）的过程。关联过程不会自动将 VLAN 路由到网关；VLAN 继续使用前端和后端客户路由器，直至手动将其路由到网关为止。VLAN 只能一次关联到一个网关，并且不得有防火墙，才能被视为有资格进行关联。

<sup>2</sup>可随时绕过网关，从而将流量返回至前端和后端客户路由器（FCR 和 BCR）。绕过 VLAN 将允许 VLAN 保持与网关的关联。

<sup>3</sup>可移植子网无法购买并添加到主网关。

<sup>4</sup>供应 Brocade 5400 vRouter 设备时通常预定义了 SoftLayer 服务 IP 地址。
