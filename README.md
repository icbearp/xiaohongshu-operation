# xiaohongshu-ops：小红书运营技能

让 AI Agent 按“先核验、再判断、后创作”的流程做小红书运营：账号体检、推荐流分析、选题、原创图文、发布前演练、评论回复和数据复盘。

## 适合谁

- 想稳定输出、但不想靠搬运和标题党的个人创作者
- 做工具教程、知识分享、服务型账号的运营者
- 已在用 Claude Code、OpenClaw、Codex 等 Agent 的用户

## 两种运行模式

- **浏览器模式**：Agent 有浏览器工具时（Claude Code / Codex 自带浏览器、OpenClaw、小红书 CLI 等），可自己打开小红书采样推荐流、搜索、填写发布页和回复评论，始终停在「发布」按钮前等你确认。
- **纯方案模式**：没有浏览器工具也能用。把截图、笔记正文或后台数据发给 Agent，它输出分析、选题、成稿和实验卡，由你手动发布。

## 能做什么

| 功能 | 你可以这样说 |
|---|---|
| 账号体检 | 帮我分析这个账号最近 10 篇笔记，问题出在哪一层 |
| 推荐流分析 | 我首页这些高赞笔记为什么会推给我 |
| 趋势研究 | 最近 30 天大家在聊 ___ 的什么问题 |
| 选题灵感 | 结合我的定位，给我 3-5 条值得做的选题 |
| 高信号样本研究 | 研究这条笔记为什么被收藏，用我的案例独立做一篇 |
| 发布前演练 | 把这篇填到发布页，停在发布按钮前 |
| 评论回复 | 检查最新评论并逐条回复 |
| 实验复盘 | 这篇发了 24 小时，帮我按实验卡复盘 |

## 设计原则

- 高互动、高收藏、GitHub Stars 只是线索，不是证据
- 证据不足时给补证据计划，价值不足时直接拒绝生产
- 不复刻原文原图、不做收入流量承诺、不教规避平台治理
- 每次任务把结论、证据和下一步沉淀到本地 `knowledge-base/`

## 目录

- `SKILL.md`：主流程
- `persona.md`：语气与人设
- `references/`：各环节 SOP（执行后端、趋势研究、来源审计、价值闸门、选题、发布、评论、复盘等）
- `examples/`：垂直案例（看剧讨论、工具教程）与回复样例
- `knowledge-base/`：本地知识库入口，使用中自动积累
- `testcase.md`：验收用例
- `NOTICE.md`：来源与改动说明
- `LICENSE`：MIT（适用于本仓库新增与修改部分）

## 致谢

- 感谢 [Xiangyu-CAS](https://github.com/Xiangyu-CAS) 的原项目 [xiaohongshu-ops-skill](https://github.com/Xiangyu-CAS/xiaohongshu-ops-skill)。本仓库在其浏览器自动化、发布、评论回复、知识库与“虾薯”人设的框架上改编而来，没有原作者的开源分享就没有这个版本。原有部分的著作权归原作者所有。
- 感谢 [mvanhorn](https://github.com/mvanhorn) 的 [last30days](https://github.com/mvanhorn/last30days-skill)，趋势研究模块可选调用它（需单独安装，未随本仓库分发）。
- 感谢 [chang-zy/xiaohongshu-skill](https://github.com/chang-zy/xiaohongshu-skill) 提供的小红书 Bridge 思路，执行后端文件将其列为可选后端。

## 许可

本仓库新增与修改部分采用 [MIT](LICENSE) 许可；原项目部分的授权状态不变，详见 [NOTICE.md](NOTICE.md)。
