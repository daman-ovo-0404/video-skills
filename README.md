# 视频制作技能库

达蒙与岑在视频工作中使用的技能入口与可复用方法。自维护技能保存完整源码，第三方能力按原安装方式维护。

## 从任务进入

| 现在要做什么 | 入口 |
|---|---|
| 学习 LibTV 案例、查看节点和真实输入、提炼方法 | [LibTV 画布研究](skills/libtv-canvas-study/SKILL.md) |
| 生成或修改角色、车辆、场景、分镜静帧 | [图片工作流](skills/libtv-shot-workflow/references/reference-image-prompts.md) |
| 制作视频、接续前镜、处理对白、补句或局部重拍 | [视频工作流](skills/libtv-shot-workflow/references/prompt-patterns.md) |
| 安排景别、运镜、表演和剪辑切点 | [摄影与剪辑](skills/libtv-shot-workflow/references/cinematography-and-editing.md) |
| 提交前明确输入、时序与验收 | [视频工作单](skills/libtv-shot-workflow/references/video-workcard.md) |
| 查原文提示与案例依据 | [52 条原文索引](skills/libtv-shot-workflow/references/verbatim-library.md) |
| 查口播剪辑、动态包装、转写、发布与复盘工具 | [外部技能目录](docs/external-skills.md) |

保留一个制作技能 `libtv-shot-workflow`，图片与视频分模块读取。`libtv-canvas-study` 单独承担案例研究。

## 安装与依赖

把 `skills/libtv-shot-workflow` 与 `skills/libtv-canvas-study` 两个完整文件夹放到目标宿主的技能目录。Codex 通常使用 `$CODEX_HOME/skills`，未设置时使用 `~/.codex/skills`。若同名目录已存在，先比较内容并保留本机修改。

安装技能文件只提供方法与模板。实际生成需要目标环境可用的图片工具、LibTV CLI 与账号；素材检查可能需要 FFmpeg/ffprobe。技能中提及的 `libtv-cli` 需另行安装或由当前工具文档替代，实际命令与模型参数以运行时帮助为准。九号正式品牌视觉另需工作区的 `apply-ninebot-vi` 技能及确认资产，本库未打包品牌素材。

## 同步与维护

本次快照日期：2026-09-29。两项技能来自九号工作区源码，已移除说明文字中的机器绝对路径；原文 `.txt` 逐字节保留。研究档案只记录工作区相对位置，不随技能包上传；案例页面与节点来源保留。后续修改以本库中的对应文件为单位比较、提交，避免整包覆盖本机调整。

[文件清单](manifest.json) 保存每个技能文件的 SHA-256；[验证记录](docs/validation.json) 记录结构、内部链接与原文完整性检查。本次未调用付费生成、剪辑或视频导出，不将文件同步等同于能力实测。

## 来源与分工

达蒙：提出视频创作需求、提供素材与反馈，确定整理方向及独立私有仓库。

岑：在既有制作实践基础上整理技能、归类入口、检查文件与引用、执行 GitHub 同步（运行于 Codex）。

案例作者、第三方技能与工具保留各自署名和权利。原文索引记录公开案例或用户提供文本的来源与观察状态；本库用于私有工作研究，未给这些材料另加开源许可证。
