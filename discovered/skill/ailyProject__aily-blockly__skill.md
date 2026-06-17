---
name: ailyProject__aily-blockly__skill
source: https://github.com/ailyProject/aily-blockly/blob/a105e1b8fae08f4d72623899fc9ddac74eb7bfc3/public/skills/library-migration-guide/SKILL.md
repo: ailyProject/aily-blockly
kind: skill
stars: 2162
last_pushed: 2026-06-15T07:33:16Z
license: gpl-3.0
score: 9
domains: [hardware-automation, dsl-design, low-code]
tags: [arduino, blockly, library-migration, embedded]
curated: 2026-06-15
curated_by: config-scout
---

# ailyProject/aily-blockly — skill

**Why it's worth keeping:** The guide provides highly specific mapping rules between API types (Statement vs. Value) and defines a structured lifecycle for code injection (e.g., setupBegin vs. setup). The distinction between input/variable field types is an essential detail for automated tool generation.

**Summary:** A rigorous technical specification for converting C++ hardware libraries into a Blockly-based visual programming DSL. It covers block schema design, generator injection sequences, and board-specific parameter mapping.

**Source credibility:** High; part of the well-maintained Aily hardware project with significant community validation.

**Recency:** Current; actively maintained with very recent push activity.

**Source:** [ailyProject/aily-blockly/public/skills/library-migration-guide/SKILL.md](https://github.com/ailyProject/aily-blockly/blob/a105e1b8fae08f4d72623899fc9ddac74eb7bfc3/public/skills/library-migration-guide/SKILL.md) · 2162★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: library-migration-guide
description: "Blockly 库转换规范：将 Arduino/ESP32 硬件库转换为 Aily Blockly 兼容格式的完整流程、block.json 设计、generator.js 实现与 toolbox.json 配置。包含串口/I2C/SPI 总线初始化、代码注入顺序、开发板适配等专业规范。触发词：库转换、迁移、migration、block.json、generator、ensureSerialBegin、Wire.begin、SPI"
metadata:
  version: "3.0.0"
  author: aily-team
  scope: global
  agents: mainAgent
  auto-activate: false
  tags: library,migration,conversion,block-json,generator,serial,i2c,spi,board-config
---

# Blockly 库转换规范

基于真实转换案例（ArduinoJson、OneButton、MQTT/PubSubClient、DHT、INA219、VL53L0X 等）的系统性指南，帮助将 Arduino 库转换为 Blockly 库。

## 核心原则

1. **用户体验优先**：简化复杂 API，提供直观操作
2. **功能完整**：覆盖原始库核心功能，保持语义一致
3. **智能自动化**：自动处理初始化、变量管理、错误检查
4. **类型安全**：通过约束防止连接错误
5. **开发板适配**：智能适配不同 Arduino 开发板
6. **总线复用**：Serial/I2C/SPI 初始化必须使用平台统一方法，确保与其他库共存

## 转换流程

```
源码分析 → 块设计 → block.json → generator.js → toolbox.json → 测试
```

## 库目录结构

```
library-name/
├─ block.json        // 块定义
├─ generator.js      // 代码生成器
├─ toolbox.json      // 工具箱配置
├─ README.md         // 人类可读文档
├─ README_AI.md      // LLM 可读文档
└─ src/              // Arduino 库源码
```

---

## 一、源码分析

### 1.1 API 识别

分析头文件，识别公共 API，按操作类型分类：

| 操作类型 | 说明 | 示例 |
|---------|------|------|
| 初始化
```

</details>
