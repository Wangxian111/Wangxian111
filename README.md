### Hi there 👋

I build **[xaudaily.com](https://xaudaily.com/gh)** — a free, static, cookie-free dashboard for gold and macro data.
我做 **[黄金读数 xaudaily.com](https://xaudaily.com/gh)**：免费、纯静态、无 Cookie 的黄金与宏观数据站。

**站上有什么 / What is on it**
- 金价：COMEX GC 连续、上期所 Au99.99（每 30 分钟实时 tick）
- 宏观：CPI / 核心 PCE / 非农 / PPI / 美元指数 / 美债 10Y·30Y / 布伦特·WTI / VIX / SPDR 持仓
- 政策与资金：联邦基金利率与下次 FOMC、Polymarket 决议定价、央行净购金（IMF 报告国口径）
- 读法：金价驱动因子打分（-100 利空 ~ +100 利多）、事件预判

**怎么做的 / How it works**
- 纯标准库 Python 数据管道（十几个来源）；每天 06:30 / 22:40（JST）两次全量更新 + 每 30 分钟行情 tick
- 每个数字都标注来源与截止日，并过一道 **ground check**：正文里的数字必须能溯源到数据快照，编造的直接弃稿
- 纯静态 HTML、无 Cookie（统计走自建 Umami，不跨站追踪）

**给程序看的入口 / For agents and scripts**
- 机器可读读数（JSON，字段稳定、带 source/asOf）：<https://xaudaily.com/readings.json>
- 每日简报（Markdown）：<https://xaudaily.com/brief.md> · 站点说明：<https://xaudaily.com/llms.txt>
- 存档 </d/>（每日一个稳定 URL）· 专题 </topic/>（如 FOMC 复盘）· 英文页 </en/>

<sub>数据事实梳理，不构成投资建议 / Data notes, not investment advice.</sub>
