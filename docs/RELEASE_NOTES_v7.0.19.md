# LoonKit v7.0.19

- **券商 IP 分流**：`HKBroker` 在 74 条域名之外新增 44 条 `IP-CIDR,no-resolve`，覆盖社区券商规则集中记录的海外行情/交易服务器地址（香港、新加坡、日本、美国），用于 App 直接连接原始 IP 的场景。
- **收录边界**：只保留非境内 IP 段；境内地址继续落在 `GEOIP,CN,DIRECT`，避免把本应直连的境内服务推到代理。Cogent 等纯转售骨干段不收录。`no-resolve` 保证域名请求不会被 IP 规则触发解析。
- **来源**：forecho/broker-rules `_ip.conf`、LingJingMaster `HK_Broker.list`、StricklandF `uSmart.list`，并用 ip-api 逐段核对国家与 ASN；按 ASN 归属推断为腾讯云/阿里云海外节点。
- **其余不变**：域名清单、策略组、本地规则与 Final 兜底保持原样；订阅总数仍为 45 份。
