# a2a-coder v3.0 — A2A 三层递归编码 Skill

## 这是什么

一个可复用的编码 Agent 工作流规范（单文件 markdown skill）：主 Agent 分析需求、拆子任务、
多轮评审后人工确认；各子任务由独立 Agent 并行开发、各自 ≥3 轮评审后实现；大子任务继续拆为
上下文受限的串行任务机械执行。含防幻觉纪律、装配验证验收分级、跨子任务契约管理、
重写类项目参考忠实度矩阵、长会话主控纪律。

源自 DeviceSimulator v3（Java 重写 4096 设备压测工具）项目全流程实践验证
（24 提交 / 13 子任务 / 5 轮现场迭代 / 189 测试），v3.0 的五项结构性改进全部对应真实缺陷。

## 安装（ZCode / Claude Code 类环境）

把 `SKILL.md` 放入目标环境的 skill 目录，例如：
- Windows: `C:\Users\<user>\.zcode\skills\a2a-coder\SKILL.md`
- 或项目级: `<project>/.zcode/skills/a2a-coder/SKILL.md`

重启会话后即可用 `/a2a-coder` 或在对话中引用调用。

## 其他环境适配

打开 SKILL.md 末尾的"环境要求与导出适配"节——逐条对照目标平台映射术语
（Agent 派发原语、模型档位、并行编排、会话命令）。最低运行要求：
能读写文件 + 跑 shell 命令的编码 Agent + 一种多轮对话机制 + 用户可参与一次方案确认。

## 许可证

MIT License — 详见 SKILL.md 文末 License 节。

## 文件

- SKILL.md — skill 本体（单文件自包含，含 MIT 许可证）
