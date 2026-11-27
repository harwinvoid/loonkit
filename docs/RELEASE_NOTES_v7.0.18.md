# LoonKit v7.0.18

- **券商域名补全**：`HKBroker` 订阅由 23 条扩到 74 条，补齐各家 App、行情、交易与区域站点域名。
  - 富途 / moomoo：`futuhk1`、`futuhk2`、`futuhkapp`、`futufin`、`futustatic`、`futuoa`、`futubull`、`futuchain`、`futuie`、`futuniuniu`、`futuhongkong`、`futuhn`、`futuau`、`futusg`、`fututrade`、`fututrust(ee)`、`ftesop`，以及 `moomooapp`、`moomoobull`、`moomoocn`、`moomooequity`、`moomootrustee`。
  - 长桥：补 `longbridge.sg`、`longbridge.global`、`longbridge.cn`、`longbridge.cloud`、`lbkrs`、`lbctrl`、`wbrks`、`longportwhale`。
  - 老虎：补 `itigergrowtha`、`tigerbrokers.net`、`tigerbrokers.nz`、`tigerbbs`、`xiaohu8`、`skytigris`、`ftfast`、`tigr.link`。
  - 盈立：补 `usmartsecurities`、`usmart.sg`、`usmart-app`、`usmart66`。
  - 华盛：补 `vbkr.com`、`hstong.com`；耀才保留 `brightsmart.com.hk` 与 `bsgroup.com.hk`。
- **筛选**：来源为券商自有站点与社区规则集（v2fly/domain-list-community、blackmatrix7/ios_rule_script、forecho/broker-rules 等），逐项用 DoH/HTTP 复核；剔除停放页（如 `futu0-9.com`、`futuin*`、`moomoo.io`、`brightsmart.com`）、他已持有域名（`yxzq.com`、`usmartsg.com`）与共享第三方根域。
- **其余不变**：本地规则、Final 兜底、其余 44 份远程订阅与全部策略组保持原样；订阅总数仍为 45 份。
