---
name: earthcake2233__cakecake
source: https://github.com/earthcake2233/cakecake/blob/d925f6b5c43dea0bbab5dd25e63b9cd8f1badf75/Skill.md
repo: earthcake2233/cakecake
kind: skill
stars: 8
last_pushed: 2026-06-09T08:04:45Z
license: unknown
score: 9
domains: [backend-api, go-programming]
tags: [sop, agent-instructions, dev-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# earthcake2233/cakecake — skill

**Why it's worth keeping:** Uses the 'Trigger-Step-Prohibited' pattern to prevent agent drift; provides specific terminal commands and error classification logic (e.g., permanent vs. temporary FFmpeg errors) that prevents common coding mistakes.

**Summary:** A rigorous Standard Operating Procedure (SOP) manual that defines precise execution steps and prohibitions for critical development tasks like compilation, database migrations, and logging.

**Source credibility:** A personal learning project with documentation quality far exceeding typical hobbyist repos.

**Recency:** Highly relevant; represents the gold standard for current AI agent/coding assistant instruction sets.

**Source:** [earthcake2233/cakecake/Skill.md](https://github.com/earthcake2233/cakecake/blob/d925f6b5c43dea0bbab5dd25e63b9cd8f1badf75/Skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Mini-Bili v1.0 技能手册（Skill）

**版本**：v1.0
**最后更新**：2026-05-11
**依赖文档**：Mini-Bili v1.0 SPEC、Mini-Bili v1.0 Rule

### 关于 Skill 的说明

本文档是项目的"标准操作手册"，告诉 AI 某些固定动作具体应该怎么执行。Skill 的存在是为了避免 AI 临场发挥、每次用不同的方式做同一件事。

Rule 说"这件事必须做"，Skill 说"这件事这样做"。

---

### S-001：编译验证

**对应 Rule**：R-DEV-1（改完代码必须可运行）

**触发条件**：每次代码修改完成后，必须执行本 Skill。

**执行步骤**：

1. 在项目根目录下依次执行：
   ```go
   go mod tidy
   go build -o ./bin/mini-bili ./cmd/
   ```
   `go mod tidy` 必须在 `go build` 之前执行，确保 `go.mod` 和 `go.sum` 与当前代码中的 import 一致。
2. 检查编译输出：
   - 若 `go build` 退出码为 0 且无任何 error 级别 stderr 输出 → 编译通过。
   - 若退出码非 0 或有 error 级别输出 → 编译失败。
3. 编译失败时：
   - 读取完整的编译错误信息。
   - 定位第一个错误（而非最后一个），修复它。
   - 修复后从步骤 1 开始重新执行。
   - 若同一错误修复 3 次仍未通过，停止并向人报告具体错误信息和已尝试的修复步骤。
4. 编译通过后，确认 `./bin/mini-bili` 文件已生成且可执行。

**禁止行为**：
- 严禁跳过 `go mod tidy` 直接执行 `go build`。
- 严禁跳过编译直接声称"代码没问题"。
- 严禁使用 `go run` 代替 `go build` 作为编译验证。
- 严禁在编译失败时修改无关代码来"碰运气"。

---

### S-002：数据库迁移

**对应 Rule**：R-DB-3（数据库结构变更必须通过迁移脚本）、R-DB-4（核心字段必须建索引）

**触发条件**：任何涉及新增表、修改表结构、新增索引的操作，必须执行本 Skill。

**执行步骤**：

1. 确认 GORM AutoMigrate 已正确配置在 `internal/data/` 目录下的数据层初始化代码中。
2. 在对应的模型结构体（Model）中定义或修改字段及标签（tag）。**定义 `play_count` 字段时，必须显式设置 `default:0` 标签**（如 `gorm:"default:0"`），防
```

</details>
