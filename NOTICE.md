# 来源与改动说明

## 原始项目

- 项目：xiaohongshu-ops-skill
- 作者：Xiangyu-CAS
- 地址：https://github.com/Xiangyu-CAS/xiaohongshu-ops-skill
- 说明：原仓库未附带开源许可证文件。本版本为改编分享，原框架的著作权归原作者所有；如原作者提出异议，将按要求修改或下架。
- 本仓库许可：新增与修改部分采用 MIT 许可（见 `LICENSE`），不改变原有部分的授权状态。

## 本版本主要改动

1. 去除对 OpenClaw 的绑定：新增执行后端选择（`references/xhs-execution-backends.md`），支持 Agent 自带浏览器、OpenClaw、专用小红书 CLI/Bridge 与纯方案模式（无浏览器，用户手动发布）；浏览器操作改为与后端无关的通用动作描述。
1.1 整合作者本地技能：`xiaohongshu-ops-upgrade` 的执行后端路由与授权规则并入后端文件；新增跨平台趋势研究模块（`references/xhs-trend-research.md`），可选调用 `last30days`（MIT，https://github.com/mvanhorn/last30days-skill，未随包分发）。
2. 新增强制质量链路：来源审计（`references/xhs-source-audit.md`）、价值闸门（`references/xhs-value-conversion-gate.md`）、实验复盘（`references/xhs-experiment-review.md`）。
3. 将“Viral Copy 爆款复刻”改为“高信号样本研究 + 独立原创”（`references/xhs-sample-research.md`），禁止复用原文、原图、专属口令、身份与数据。
4. 账号分析改为“曝光 → 点击 → 阅读 → 信任 → 咨询 → 履约”分层诊断，只有公开数据时不推断后台指标。
5. 人设改为默认“有工作经验的实操者”，“虾薯”仅用于轻量评论。
6. 新增工具/效率教程类案例（`examples/tool-tutorial/case.md`）与验收用例（`testcase.md`）。
7. 知识库新增 `sources/`、`experiments/` 目录；分发包不含任何个人运营记录。
8. 移除原仓库的演示图片、一键安装脚本和第三方账号样本数据。
