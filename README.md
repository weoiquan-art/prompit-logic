# prompit-logic

JIN 的 Seedance 视频提示词总逻辑（软锁）。每次写、改、审 Seedance 2.0／2.5 视频提示词前先读 `SKILL.md`，逐条对照；对话压缩后如果这些内容不在上下文里，重新读一遍。

内容：共用写法核心 17 条、2.0 卡、2.5 卡（分开记）、交付前自检、写完交官方 skill 调试（待测）、官方写法和 JIN 原有写法的冲突与 2026-10-12 的决定。

## 这是公开仓库

- 不收录火山引擎官方 PDF 和官方 skill（sd2-pe、sd25-pe）的原文。官方来源的内容一律用自己的话转述，并在每条后面标出处（〔官方 2.0〕〔官方 2.5〕〔JIN 规定〕〔JIN 实测〕〔JIN skill〕）。
- 官方 skill 的原版另存在 JIN 的 claude.ai 里，两个版本各一个：sd2-pe（2.0）、sd25-pe（2.5）。
- 私有仓库 video-exp 里的案例原文不搬进来，只留结论和指向。

## 来源指纹（只记指纹，不存原文）

用来判断官方 skill 有没有更新过：

| 来源 | 说明 | sha256 |
|---|---|---|
| sd25-pe 0.1.1（owner seedance） | SKILL.md，996 行、69,727 字节 | `ee04557ba9a1c9f5517b574e24fc73d0022b22254373074db4c11f3d0635ea57` |
| sd25-pe 安装锁文件 computedHash | 等于 sha256("SKILL.md" 加上文件正文) | `5754d8172aaf1e4c9f4ca5a27182fc6293db1dddd5b868b791dca5c93b2623ef` |
| sd2-pe（文件头没有版本号） | SKILL.md，225 行、21,854 字节 | `8836cdb2bc4f7d8a329c4ecd33cca19efdcfc71afdd927e8defe6e1f9a2e2b3c` |

另参考 JIN 提供的五份火山引擎官方 PDF（2.5 教程、2.5 提示词指南、2.0 系列提示词指南、2.0 系列教程、视频生成教程）。

## 与其他仓库的关系

- 通用提示词 Skill `-prompit-for-ai-video-generator`、Chibi `chibi-`、真人 `video-prompit-for-realism`、短剧筹备 `short-drama-prep`：本仓库从它们和 video-exp 的已验证经验里合并出共用写法，不替代它们；分支格式和本文件冲突时，格式听分支，写法检查仍按本文件。
- 2026-10-12 起通用仓库先不改；以后要合并，另行商量。
