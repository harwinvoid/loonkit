# LoonKit v7.0.17

- **港股券商分流**：新增 `HKBroker` 策略组与 23 条固定域名后缀，覆盖富途（`futunn.com` / `futuhk.com` / `moomoo.com` / ESOP）、长桥（`longbridge` / `longport`）、老虎（`itiger` / `laohu8`）、华盛、盈立与耀才。默认走 `Proxy`，也可在组内改选 `DIRECT`。
- **规则来源**：新增 `rules/releases/v7.0.17/HKBroker.lsr`，域名于 2026-11-27 逐项核对各券商公开站点，不使用关键词规则，并固定到本 fork 的 Git 提交。
- **其余不变**：本地规则、Final 兜底、既有 44 份远程订阅与全部策略组保持原样；订阅总数为 45 份。
