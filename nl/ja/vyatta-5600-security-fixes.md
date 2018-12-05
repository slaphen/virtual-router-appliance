---

copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# AT&T Vyatta 5600 vRouter のソフトウェア・パッチ

**2018 年 11 月 2 日現在**

本資料では、現在サポートされている Vyatta Network OS 5600 のバージョン用のパッチをリストします。5.2 以前のバージョンでは、S 番号を使用してパッチに名前が付けられています。17.1 以降のバージョンでは、「i」、「o」、「l」、および「x」を除く英小文字を使用してパッチに名前が付けられています。

単一のアップデートで複数の CVE 番号に対応した場合、最も高い CVSS スコアがリストされます。

## 1801t

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-44172 |ブロッカー|mss-clamp テストでエラー「interfaces [openvpn] is not valid」が報告される|
| VRVDR-43969 |軽微| Vyatta 18.x の GUI で、ステータスの誤り、メモリー使用量を確認せよと報告される|
| VRVDR-43847  | 大 |結合インターフェース上の TCP 通信でスループットが低速になる |

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-43842 | N/A | DSA-4305-1 | CVE-2018-16151、CVE-2018-16152: Debian DSA4305-1: strongswan – セキュリティー・アップデート|

## 1801s

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-44041 | 大 | SNMP ifDescr oid の応答時間が遅い|
 
**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-44074| 9.1 | DSA-4322-1 | CVE-2018-10933: Debian DSA-4322-1: libssh – セキュリティー・アップデート|
| VRVDR-44054 | 8.8 | DSA-4319-1 | CVE-2018-10873: Debian DSA-4319-1: spice – セキュリティー・アップデート|
| VRVDR-44038 | N/A | DSA-4315-1 | CVE-2018-16056、CVE-2018-16057、CVE-2018- 16058: Debian DSA-4315-1: wireshark – セキュリティー・アップデート|
| VRVDR-44033 | N/A | DSA-4314-1 | CVE-2018-18065: Debian DSA-4314-1: net-snmp – セキュリティー・アップデート| 
|VRVDR-43922 | 7.8 | DSA-4308-1 | CVE-2018-6554、CVE-2018-6555、CVE-2018-7755、CVE-2018-9363、CVE-2018-9516、CVE-2018-10902、CVE-2018-10938、CVE-2018-13099、CVE-2018- 14609、CVE-2018-14617、CVE-2018-14633、CVE- 2018-14678、CVE-2018-14734、CVE-2018-15572、CVE-2018-15594、CVE-2018-16276、CVE-2018- 16658、CVE-2018-17182: Debian DSA-4308-1: linux – セキュリティー・アップデート|
| VRVDR-43908 | 9.8 | DSA-4307-1 | CVE-2017-1000158、CVE-2018-1060、CVE-2018- 1061、CVE-2018-14647: Debian DSA-4307-1: python3.5 - セキュリティー・アップデート|
| VRVDR-43884 | 7.5 | DSA-4306-1 | CVE-2018-1000802、CVE-2018-1060、CVE-2018- 1061、CVE-2018-14647: Debian DSA-4306-1: python2.7 - セキュリティー・アップデート|

## 1801r

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-43738 | 大 |SNAT セッションを介して返される ICMP の到達不能パケットが配信されない|
| VRVDR-43538 | 大 |結合インターフェース上でサイズ超過エラーを受信する| 
| VRVDR-43519 | 大 |config が存在しないのに、Vyatta-keepalived が実行される| 
| VRVDR-43517 | 大 |VFP / ポリシー・ベースの IPsec のエンドポイントが vRouter 自体に常駐している場合、トラフィックが失敗する| 
| VRVDR-43477 | 大 |IPsec VPN 構成をコミットすると、警告「Warning: unable to [VPN toggle net.ipv4.conf.intf.disable_policy], received error code 65280」が返される|
| VRVDR-43379 |軽微| NAT の統計が正しく表示されない|
 
**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-43837 | 7.5 | DSA-4300-1 | CVE-2018-10860: Debian DSA-4300-1: libarchive-zip-perl – セキュリティー・アップデート|
| VRVDR-43693 | N/A | DSA-4291-1 | CVE-2018-16741: Debian DSA-4291-1: mgetty – セキュリティー・アップデート| 
| VRVDR-43578 | N/A | DSA-4286-1 | CVE-2018-14618: Debian DSA-4286-1: curl - セキュリティー・アップデート|
| VRVDR-43326 | N/A | DSA-4280-1 | CVE-2018-15473: Debian DSA-4280-1: openssh - セキュリティー・アップデート| 
| VRVDR-43198 | N/A | DSA-4272-1 | CVE-2018-5391: Debian DSA-4272-1: linux セキュリティー・アップデート (FragmentSmack) |
| VRVDR-43110 | N/A | DSA-4265-1 | Debian DSA-4265-1 : xml-security-c - セキュリティー・アップデート| 
| VRVDR-43057 | N/A | DSA-4260-1 | CVE-2018-14679、CVE-2018-14680、CVE-2018-14681、CVE-2018-14682: Debian DSA-4260-1 : libmspack - セキュリティー・アップデート| 
| VRVDR-43026 | 9.8 | DSA-4259-1 | Debian DSA-4259-1 : ruby2.3 - セキュリティー・アップデート VRVDR-42994N/ADSA-4257-1CVE-2018-10906: Debian DSA-4257-1 :fuse - セキュリティー・アップデート|

## 1801q

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-43531 | 大 |1801p 上でブートすると、約 40 秒でカーネル・パニックになる|
| VRVDR-43104 | 重大 | IPsec を使用可能にすると、DHCP ネットワーク上で不正な無償 ARP が発生する|
| VRVDR-41531 | 大 | VFP インターフェースのアンバインディング後も IPsec はインターフェースを使用し続けようとする|
| VRVDR-43157 |軽微|トンネルがバウンスしても、SNMP トラップが適切に生成されない|
| VRVDR-43114 | 重大 | リブート時に、HA ペアのルーターでピアよりも高優先度のルーターが自身の「preempt false」構成を無視して、ブート直後にマスターになる|
| VRVDR-42826 |軽微|remote-id 「0.0.0.0」の場合、事前共有キーの不一致によりピア・ネゴシエーションが失敗する|
| VRVDR-42774 | 重大| X710 (i40e) ドライバーがフロー制御フレームを超高速で送信する|
| VRVDR-42635 |軽微| BGP 再配布ルート・マップ・ポリシーへの変更が有効にならない|
| VRVDR-42620 |軽微| トンネルが稼働中に見えるのに、Vyatta-ike-sa-daemon がエラー「Command failed: establishing CHILD_SA passthrough-peer」をスローする|
| VRVDR-42483 |軽微| TACACS 認証が失敗する|
| VRVDR-42283 | 大 | vif インターフェースの IP を削除すると、すべてのインターフェースの VRRP 状態が FAULT に変わる|
| VRVDR-42244 |軽微| フロー・モニタリングがコレクターに 1000 サンプルのみエクスポートする|
| VRVDR-42114 | 重大 | HTTPS サービスは TLSv1 を公開してはならない|
| VRVDR-41829 | 大 |SIP ALG soak テストでシステムが無反応になるまでデータ・プレーンのコア・ダンプが発生する|
| VRVR-41683 |ブロッカー|VRF 上で確認された DNS ネーム・サーバー・アドレスが一貫して認識されない|
| VRVDR-41628 |軽微|ルーター通知のルート / プレフィックスはカーネルとデータ・プレーンでアクティブになるが、RIB では無視される|
 
**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-43288 | 5.6 | DSA-4279-1 | CVE-2018-3620、CVE-2018-3646: Debian DSA-4279- 1 – Linux セキュリティー・アップデート|
| VRVDR-43111 | N/A | DSA-4266-1 | CVE-2018-5390、CVE-2018-13405: Debian DSA- 4266-1 – Linux セキュリティー・アップデート|

## 1801n

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-42588 |軽微| 機密性の高いルーティング・プロトコル構成がシステム・ログで誤ってリークされる|
| VRVDR-42566 | 重大 | 17.2.0h から 1801m にアップグレードした 1 日後、両方の HA メンバーでリブートが複数回発生した|
| VRVDR-42490 | 大 |VRRP の移行の約 1 分後、VTI-IPSEC IKE SA が失敗する|
| VRVDR-42335 | 大 | IPSEC: remote-id "hostname" の動作が 5400 と 5600 の間で異なる|
| VRVDR-42264 | 重大 | SIT トンネル上で接続性がない – "kernel: sit: non-ECT from 0.0.0.0 with TOS=0xd"|
| VRVDR-41957 |軽微|NAT 済みの双方向パケットが GRE に大きすぎて ICMP Type 3 Code 4 を返さない|
| VRVDR-40283 | 大 |構成変更によって大量のログ・メッセージが生成される|
| VRVDR-39773 | 大 |BGP vrrp-failover コマンドでルート・マップを使用すると、すべてのプレフィックスが撤回される場合がある|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-42505 | N/A | DSA-4236-1 | CVE-2018-12891、CVE-2018-12892、CVE-2018-12893: Debian DSA-4236-1: xen - セキュリティー・アップデート|
| VRVDR-42427 | N/A | DSA-4232-1 | CVE-2018-3665: Debian DSA 4232-1: xen - セキュリティー・アップデート|
| VRVDR-42383 | N/A | DSA-4231-1 | CVE-2018-0495: Debian DSA-4231-1: libgcrypt20 - セキュリティー・アップデート|
| VRVDR-42088 | 5.5 | DSA-4210-1 | CVE-2018-3639: Debian DSA-4210-1: xen – セキュリティー・アップデート|
| VRVDR-41924 | 8.8 | DSA-4201-1 | CVE-2018-8897、CVE-2018-10471、CVE-2018-10472、CVE-2018-10981、CVE-2018-10982: Debian DSA-4201- 1: xen – セキュリティー・アップデート|

## 5.2R6S12

2018 年 6 月 21 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-42084 |ブロッカー|nat/ipsec config を再度適用すると、「show dataplane route」で Vfp インターフェースが「non-dataplane interface」としてマークされる|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-42317 | 5.4 | DSA-4226-1 | CVE-2018-12015: Debian DSA-4226-1: perl – セキュリティー・アップデート|
| VRVDR-42284 | 7.5 | DSA-4222-1 | CVE-2018-12020: Debian DSA-4222-1: gnupg2 – セキュリティー・アップデート|
| VRVDR-41797 | 8 | DSA-4196-1 | CVE-2018-1087、CVE-2018-8897: Debian DSA-4196-1: linux – セキュリティー・アップデート|
| VRVDR-41680 | 7.8 | DSA-4188-1 | Debian DSA-4188-1: linux – セキュリティー・アップデート (Spectre) |

## 1801m

2018 年 6 月 15 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-42256 | 重大 |最後に確立された CHILD_SA が削除されるとアウトバウンド・トラフィックがなくなる|
| VRVDR-42084 |ブロッカー|ルーターが構成されているのに、ルーターに到着したパケットに対して、PB IPsec トンネルの VFP インターフェースにリンクされた NAT セッションが作成されない|
| VRVDR-42018 |軽微| 「restart vpn」を実行すると、「IKE SA daemon: org.freedesktop.DBus.Error.Service.Unknown」エラーがスローされる|
| VRVDR-42017 |軽微| VRRP バックアップで、「show vpn ipsec sa」を実行中に、vyatta-op-vpn- ipsec-vici 563 行に関連して「ConnectionRefusedError」エラーがスローされる|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 42317 | 5.4 | DSA-4226-1 | CVE-2018-12015: Debian DSA-4226-1: perl – セキュリティー・アップデート|
| VRVDR- 42284 | 7.5 | DSA-4222-1 | CVE-2018-12020: Debian DSA-4222-1: gnupg2 – セキュリティー・アップデート|

## 5.2R6S11

2018 年 6 月 11 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-42109 | 重大 |5.2R6S7 の SNAT+FW で、1 ICMP 応答パケットのみ受信される|
| VRVDR-42084 |ブロッカー|ルーターが構成されているのに、ルーターに到着したパケットに対して、PB IPsec トンネルの VFP インターフェースにリンクされた NAT セッションが作成されない|
| VRVDR-42027 | 大 | SFLOW が誤った入力 ifIndex を使用する|
| VRVDR-41558 | 大 |パケット・トレースで報告されるタイム・スタンプが実際の時刻およびシステム・クロックと一致していない|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 42207 | 7.5 | DSA-4217-1 | CVE-2018-11358、CVE-2018-11360、CVE-2018-11362、CVE- 2018-7320、CVE-2018-7334、CVE-2018-7335、CVE-2018- 7419、 CVE-2018-9261、CVE-2018-9264、CVE-2018-9273: Debian DSA-4217-1: wireshark – セキュリティー・アップデート|
| VRVDR- 42013 | N/A | DSA-4210-1 | CVE-2018-3639: 推測的な実行、バリアント 4: 推測的なストア・バイパス / Spectre v4 / Spectre-NG |
| VRVDR- 42006 | 9.8 | DSA-4208-1 | CVE-2018-1122、CVE-2018-1123、CVE-2018-1124、CVE-2018- 1125、CVE-2018-1126: Debian DSA-4208-1: procps – セキュリティー・アップデート|
| VRVDR- 41946 | N/A | DSA-4202-1 | CVE-2018-1000301: Debian DSA-4202-1: curl – セキュリティー・アップデート|
| VRVDR- 41795 | 6.5 | DSA-4195-1 | CVE-2018-0494: Debian DSA-4195-1: wget – セキュリティー・アップデート|

## 1801k

2018 年 6 月 8 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-42084 |ブロッカー|ルーターが構成されているのに、ルーターに到着したパケットに対して、PB IPsec トンネルの VFP インターフェースにリンクされた NAT セッションが作成されない|
| VRVDR-41944 | 大 |VRRP フェイルオーバーの後、一部の VTI トンネルは、「vpn restart」またはピア・リセットを発行するまで再確立されない |
| VRVDR-41906 | 大 |ICMP Type 3 Code 4 メッセージが誤ったソース IP から送信されるため、PMTU ディスカバリーが失敗する|
| VRVDR-41558 | 大 |パケット・トレースで報告されるタイム・スタンプが実際の時刻およびシステム・クロックと一致していない|
| VRVDR-41469 | 大 |1 つのインターフェース link down – bond がトラフィックを通していない|
| VRVDR-41420 | 大 |LACP モードをアクティブからバックアップに変更すると、LACP 結合状態/リンクが「u/D」になる|
| VRVDR-41313 | 重大 | IPsec – VTI インターフェースが不安定|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 42207 | 7.5 | DSA-4217-1 | CVE-2018-11358、CVE-2018-11360、CVE-2018-11362、CVE- 2018-7320、CVE-2018-7334、CVE-2018-7335、CVE02018- 7419、CVE-2018-9261、CVE-2018-9264、CVE-2018-9273: Debian DSA-4217-1: wireshark – セキュリティー・アップデート|
| VRVDR- 42013 | N/A | DSA-4210-1 | CVE-2018-3639: 推測的な実行、バリアント 4: 推測的なストア・バイパス / Spectre v4 / Spectre-NG |
| VRVDR- 42006 | 9.8 | DSA-4208-1 | CVE-2018-1122、CVE-2018-1123、CVE-2018-1124、CVE-2018- 1125、CVE-2018-1126: Debian DSA-4208-1: procps – セキュリティー・アップデート|
| VRVDR- 41946 | N/A | DSA-4202-1 | CVE-2018-1000301: Debian DSA-4202-1: curl – セキュリティー・アップデート|
| VRVDR- 41795 | 6.5 | DSA-4195-1 | CVE-2018-0494: Debian DSA-4195-1: wget – セキュリティー・アップデート|

## 1801j

2018 年 5 月 18 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41481 |軽微|結合インターフェース上の VRRP が VRRP 通知を送信しない|
| VRVDR-39863 | 大 |GRE が関連付けられ、トンネルのローカル・アドレスが VRRP の一部であるルーティング・インスタンスをお客様が削除すると、VRRP がフェイルオーバーする|
| VRVDR-27018 | 重大 | 実行中の構成ファイルがグローバルで読み取り可能になる|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR-41680 | 7.8 | DSA-4188-1 | Debian DSA-4188-1: linux – セキュリティー・アップデート|

## 5.2R6S10

2018 年 5 月 17 日にリリース

**解決された問題**
|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41543 | 大 |構成記述で「￥」(バックスラッシュ) を使用すると、「update config-sync」でエラーが報告される
| VRVDR-27018 | 重大 | 実行中の構成ファイルがグローバルで読み取り可能になる|

## 1801h

2018 年 5 月 11 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41664 | 重大 |データ・プレーンが MTU サイズの ESP パケットをドロップする|
| VRVDR-41536 |軽微|DNS 転送を使用可能にした場合、4 を超える静的ホスト・エントリーを追加すると、Dnsmasq service start-init の制限に到達する|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 41797 | 7.8 | DSA-4196-1 | CVE-2018-1087、CVE-2018-8897: Debian DSA-4196-1: linux セキュリティー・アップデート|

## 5.2R6S

2018 年 5 月 8 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40803 |軽微|リブート後、「show vrrp」の出力に VIF インターフェースが表示されない|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 41512 | 9.8 | DSA-4172-1 | CVE-2018-6797、CVE-2018-6798、CVE-2018-6913: Debian DSA-4172-1: perl – セキュリティー・アップデート|

## 1801g

2018 年 5 月 4 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41620 | 大 |新しい vIF を追加した後、vTI インターフェースがトラフィックの送信を停止する|
| VRVDR-40965 | 大 |データ・プレーンがクラッシュした後、結合が回復しない|

## 1801f

2018 年 4 月 23 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41537 |軽微|1801d では、IPsec トンネル上で ping が動作しない|
| VRVDR-41283 |軽微|構成で静的ルートが使用不可になっている場合、ブート中に configd が静的ルートの処理を停止する|
| VRVDR-41266 | 大 |VRF への静的ルートのリークにより、リブート後 mGRE トンネルを通してトラフィックが転送されない|
| VRVDR-41255 | 大 |スレーブがダウンした場合、マスター・リンク状態にそれが反映されるまで 60 秒以上かかる|
| VRVDR-41252 | 大 |ゾーン・ポリシーのアンバインド済み VTI で、ゾーン・ルールのコミット順序によってはドロップ・ルールがバイパスされる|
| VRVDR-41221 | 重大 |vRouter を 1801b から 1801c へ、さらに 1801d へアップグレードすると、故障率が 10% になる|
| VRVDR-40967 | 大 |IPv6 転送を使用不可化すると、ソースが VTI である IPv4 パケットはルーティングされない|
| VRVDR-40858 | 大 |MTU 1428 と示される VTI インターフェースで TCP PMTU 問題が発生する|
| VRVDR-40857 | 重大 |インターフェース名が一定の長さであるタグ付き VLAN で Vhost-bridge が稼働しない|
| VRVDR-40803 |軽微|リブート後、「show vrrp」の出力に VIF インターフェースが表示されない|
| VRVDR-40644 | 大 | IKEv1: QUICK_MODE 再転送が正しく処理されない|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 41512 | 9.8 | DSA-4172-1 | CVE-2018-6797、CVE-2018-6798、CVE-2018-6913: Debian DSA-4172-1: perl – セキュリティー・アップデート|
| VRVDR- 41331 | 6.5 | DSA-4158-1 |CVE-2018-0739: Debian DSA-4158-1: openssl1.0 – セキュリティー・アップデート
| VRVDR- 41330 | 6.5 | DSA-4157-1 | CVE-2017-3738、CVE-2018-0739: Debian DSA-4157-1: openssl – セキュリティー・アップデート|
| VRVDR- 41215 | 6.1 |CVE-2018-1059 | CVE-2018-1059 – DPDK vhost で、VM ゲストからの境界を越えたホスト・メモリー・アクセス|

##5.2R6S8
2018 年 4 月 16 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-41283 |軽微|構成で静的ルートが使用不可になっている場合、ブート中に configd が静的ルートの処理を停止する|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 41330 | 6.5 | DSA-4157-1 | CVE-2017-3738、CVE-2018-0739: Debian DSA-4157-1: openssl – セキュリティー・アップデート

##1801e
2018 年 3 月 28 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-39985 |軽微|GRE トンネルの MTU より大きい TCP DF パケットが「ICMP 断片化要」を返すことなくドロップされる | 
| VRVDR-41088 | 重大 |拡張 (4 バイト) ASN が符号なしタイプとして内部で表されない|
| VRVDR-40988 | 重大 |一定数のインターフェースで使用した場合、Vhost が開始しない|
| VRVDR-40927 | 重大 | DNAT: 183 応答の後の SIP 200 OK 内の SDP が変換されない|
| VRVDR-40920 | 大 |127.0.0.1 をリッスン・アドレスにした場合、snmpd が開始しない|
| VRVDR-40920 | 重大 |結合された SR-10V インターフェース上で ARP が動作しない|
| VRVDR-40294 | 大 |結合グループからスレーブを取り除いた後、データ・プレーンが前のキューを復元しない|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 41172 | N/A | DSA-4140-1 | DSA 4140-1: libvorbis セキュリティー・アップデート|

##5.2R6S7
2018 年 3 月 15 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-38801 | 大 |複数セグメントのパケットが IPsec VTI を介して受信されると、結合インターフェースがダウンする

##5.2R6S6
2018 年 3 月 12 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40281 | 大 |5.2 からより新しいバージョンにアップグレードした後、操作モードでエラー「vbash: show: command not found」が発生する|
| VRVDR-40135 | 大 |スパンニング・ツリー・パケットが VIF インターフェースのブリッジ・ポートで受信されない|
| VRVDR-39991 | 大 |ステートフル・ファイアウォールが、同じインターフェース上の 2 つのサブネット間のパケットをドロップする| 
| VRVDR-36481 | 大 |5.2R4 から 17.1.0 または 5.2R3 にアップグレードまたはダウングレードすると、「/opt/vyatta/sbin/vyatta-install-image.functions: line 372: is_onie_boot: command not found」が表示される|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 40019 | 8.8 | DSA-4086-1 | CVE-2017-15412: Debian DSA-4086-1: libxml2 – セキュリティー・アップデート|
| VRVDR- 39907 | 7.8 | CVE-2017-5717 |ブランチ・ターゲット・インジェクション / CVE-2017-5717 / Spectre, aka. バリアント #2 |

##1801d
2018 年 3 月 8 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40940 | 大 |NAT/ファイアウォールに関連するデータ・プレーンのクラッシュ|
| VRVDR-40886 | 大 |「icmp name <value>」をルールのその他いくつかの構成と組み合わせると、ファイアウォールがロードされない|
| VRVDR-39879 | 大 |ジャンボ・フレーム用に結合を構成すると失敗する|

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 40327 | 9.8 | | DSA-4098-1
CVE-2018-1000005、CVE-20178-1000007: Debian DSA- 4098-1: curl – セキュリティー・アップデート|
| VRVDR- 39907 | 7.8 | CVE-2017-5717 | ブランチ・ターゲット・インジェクション / CVE-2017-5715 / Spectre、またはバリアント #2 |

##1801c
2018 年 3 月 7 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40281 | 大 |5.2 からより新しいバージョンにアップグレードした後、操作モードでエラー「-vbash: show: command not found」が発生する|

##1801b
2018 年 2 月 21 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40622 | 大 |IP アドレスが DHCP サーバーから取得された場合、Cloud-init イメージが正しく検出されない|
| VRVDR-40613 | 重大 |いずれかの物理リンクがダウンの場合、結合インターフェースが稼働しない|
| VRVDR-40328 | 大 |Cloud-init イメージのブートに長い時間がかかる|

##1801a
2018 年 2 月 7 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-40324 | 大 |結合インターフェースのあるルーターに負荷がないのに平均負荷が 1.0 を超える|

##5.2R6S5
2018 年 1 月 19 日にリリース

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 39891 | 5.6 | DSA-4078-1 | CVE-2017-5754: Debian DSA-4078-1: linux – セキュリティー・アップデート (メルトダウン) |
| VRVDR- 38265 | 8.8 | DSA-3970-1 | CVE-2017-1 |

##5.2R6S4
2017 年 12 月 15 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-39529 | 大 |DHCP サーバーのフェイルオーバーでデータベースが同期されない|
| VRVDR-39399 | 重大 |show vrrp/multiple interfaces flap/seg fault で Vyatta のドロップ・オフ・ネットワーク状態が FAULT になる|
| VRVDR-39112 | 大 |ZBF に一致する DNAT トラフィックがフロー内の最初のパケットのみドロップする|
| VRVDR-38075 |軽微|応答側から「restart vpn」が発行された場合、起動側が接続を再確立しない|
| VRVDR-37934 | 重大 |aggregate-address summary-only を構成し、静的ルートが無い場合、BGPd がクラッシュする|
| VRVDR-37717 |軽微|バージョンの出力で、hard-enf の「説明」フィールドと「ライセンス」フィールドの名前を変更する|
| VRVDR-37689 | 大 |高速な NIC PF 割り込み|
| VRVDR-37633 | 重大 |Keepalived がハングする|

## 5.2R6S3
2017 年 12 月 4 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-39207 | 重大 |結合 VIF インターフェース上で ARP が失敗する|


##5.2R6S2
2017 年 11 月 2 日にリリース

**解決された問題**

|発行番号|優先度|概要|
| --- | --- | --- |
| VRVDR-39177 | 大 |–push dhcp-option で OpenVPN サーバーのドメイン・ネーム・オプションが適用されない|
| VRVDR-39129 | 重大 |OpenVPN サーバーの push-route パラメーターにより OpenVPN が開始しない|

##5.2R6S1
2017 年 10 月 12 日にリリース

**解決されたセキュリティーの脆弱性**

|発行番号|CVSS スコア|アドバイザリー|概要|
| --- | --- | --- | --- |
| VRVDR- 38819 | 9.8 | DSA-3989-1 | CVE-2017-14491、CVE-2017-14492、CVE-2017-14493、CVE- 2017-14494、CVE-2017-14495、CVE-2017-14496: DSA- 3989-1 dnsmasq -- セキュリティー・アップデート|

本書に記載されている情報は、AT&T によるオファー、コミットメント、表明、または保証を意味するものではなく、また変更される場合があります。書面による合意がある場合を除き、AT&T 企業の外部での使用および開示を禁じます。

© 2018 AT&T Intellectual Property. All rights reserved. その他のマークは、各社の商標である場合があります。