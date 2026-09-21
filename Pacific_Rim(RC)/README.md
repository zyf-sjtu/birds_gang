# 穿戴式外骨骼遥控器 × 双机械臂小车

设计基线（完整开发注意事项）见 `docs/00_design-baseline_v0.1_20260921.txt`。

## 目录只有 4 个

| 目录 | 放什么 |
| --- | --- |
| `docs/` | 开发注意事项、设计说明、通信协议、标定、安全、测试 |
| `hardware/` | `board/` 原理图 PCB Gerber BOM；`mechanical/` STEP DXF STL 图纸；`datasheets/` 器件手册 |
| `firmware/` | 4 个节点的固件：`l103_joint`（关节采集）、`l103_hand`（手部输入）、`h417_wearable`（穿戴主控）、`h417_receiver`（接收机） |
| `media/` | 实拍图片；视频只放链接（写在 `media/videos.md`） |

## 3 条规则

1. 文件夹和文件名用英文/数字，不用中文和空格（建模和 EDA 软件容易出问题）。
2. 视频和超大文件不进仓库，放网盘/B站，链接写进 `media/videos.md`。
3. 拿不准放哪：文档进 `docs/`，图片进 `media/`，硬件进 `hardware/`，代码进 `firmware/`。
