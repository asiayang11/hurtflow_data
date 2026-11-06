# Hurtflow 个人数据

本仓库存放 Hurtflow 的个人台账、收集结果、用户偏好、任务输入输出和素材。工作台代码位于并列的 `../hurtflow`。

| 路径 | 内容 |
| --- | --- |
| `data/workspace.json` | 产品、研究、关注榜、素材索引、任务与用户设置 |
| `data/workspace.backup.json` | 工作台保留的上一版本本地备份 |
| `workspace/tasks/` | ChatGPT 协作任务与 Product Hunt 榜单任务 |
| `workspace/assets/` | 用户保存的素材，按需生成 |

新定时任务的计划、状态和产出均保存在本仓库所配置的数据根目录下。恢复数据时，先停止工作台，再在这里恢复台账和相关任务、素材。工作台可通过代码仓库 `.env.local` 中的 `HUNTFLOW_DATA_ROOT` 指向本目录。

按逻辑步骤独立提交业务数据。临时文件、备份副本、写锁和凭据留在本机。Git 工作约定见 `AGENTS.md`。
