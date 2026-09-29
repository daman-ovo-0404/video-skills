# 外部视频技能目录

以下依据 2026-09-29 本机可读取的技能文件及当前会话技能目录整理。它们是外部依赖入口，源码未复制到本库；“存在技能文件”不代表本次完成了登录、依赖或实际生成验证。安装时按原插件或包恢复，凭据留在目标设备。

| 阶段 | 技能／插件入口 | 用途 | 获取或恢复方式 |
|---|---|---|---|
| 研究 | `douyin-video-analyzer` | 抖音视频结构、视觉与口播拆解 | 原技能包；需要 Node、FFmpeg、yt-dlp 及所选 AI 服务凭据 |
| 研究 | `douyin-search-keyword` | 关键词、作品、评论和热点线索 | 原技能包及其数据服务；运行前检查账号权限 |
| 研究 | `cn-last30days` | 中国社媒近 30 天话题研究 | [原项目](https://github.com/redfox-data/redfox-community)，按其技能说明安装 |
| 生成 | `dreamina-canvas-cli` | 即梦画布、媒体生成与交付 | 原 CLI 随附技能；先核对版本、模型列表和登录状态 |
| 生成 | `libtv-cli` | LibTV 模型与节点操作 | 两项自维护技能依赖此工具；本次扫描未找到其全局技能目录或 PATH 命令，目标环境须单独恢复 |
| 剪辑 | `mandarin-talking-head-rough-cut:rough-cut` | 中文口播去废话、多 take 处理、字幕与声音包装 | Codex 对应插件；本机缓存版本 1.1.0 |
| 剪辑 | `adobe-edit-quick-cut` | 从素材中挑选重点形成短剪 | Adobe 插件；需相应连接器和素材访问能力 |
| 包装 | `hyperframes:hyperframes` | HTML 视频、字幕、动效、转场与旁白 | HyperFrames 插件；本机缓存版本 0.1.2 |
| 包装 | `hyperframes:hyperframes-cli` | 创建、预览、检查和渲染 | 同一 HyperFrames 插件 |
| 包装 | `hyperframes:website-to-hyperframes` | 网页内容转视频 | 同一 HyperFrames 插件 |
| 包装 | `hyperframes:gsap` / `hyperframes:hyperframes-registry` | 动画实现与组件 | 同一 HyperFrames 插件，作为包装阶段辅助 |
| 转写 | `media-transcript` | 社媒视频口播转文字、查询转写任务 | `socialdatax-skills` 包及其 MCP/服务凭据 |
| 发布 | `video-account-zh` | 视频号选题、直播预热与公众号联动 | 原技能包（本机元数据：作者 ikun，MIT） |
| 复盘 | `wechat-video-channel-hot-trend` | 公开视频号页面信息与表现摘要 | 本机安装目录名 `wechat-video`，恢复时注意与技能名不同 |
| 封面 | `guizang-social-card-skill` | 社媒图卡、视频与 Live Photo 衍生视觉 | 原技能包；按具体任务加载 |

与纯视频任务无关的通用运营、图像、文档和设计技能不重复归入。剪映、Blender、DaVinci 的软件或 MCP 配置也不等同于技能文件，未随本库打包。
