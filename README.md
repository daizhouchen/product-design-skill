# Product Design Skill

产品设计全流程 Claude Code Skill，从头脑风暴到 PRD 产出。

## 它能做什么

通过引导式对话，帮你走完完整的产品设计流程：

```
阶段一：洞察 → 市场调研 + 用户画像 + JTBD定义
阶段二：构建 → 创意发散 + 方案收敛 + 产品架构 + 用户流程
阶段三：验证产出 → 四维设计审查 + 一次性生成PRD
```

**核心机制：**
- **ID追踪**：JTBD → 功能 → 模块 → 流程，全链路可追溯
- **覆盖检查**：每次增删改自动验证上下游完整性，防止逻辑断层
- **按需调研**：各阶段自动触发网络搜索（竞品、市场、UX最佳实践）

**内置7种方法论：** JTBD / 价值主张画布 / HMW / SCAMPER / Kano / RICE / Nielsen十原则

## 安装

将 `product-design` 目录复制到 Claude Code 的 skills 目录下：

```bash
# macOS / Linux
cp -r product-design ~/.claude/skills/product-design

# Windows (Git Bash)
cp -r product-design "$HOME/.claude/skills/product-design"

# Windows (PowerShell)
Copy-Item -Recurse product-design "$env:USERPROFILE\.claude\skills\product-design"
```

或者直接克隆：

```bash
git clone https://github.com/daizhouchen/product-design-skill.git ~/.claude/skills/product-design
```

安装后重启 Claude Code 即可生效。

## 使用

直接对 Claude Code 说产品相关的话就会自动触发，比如：

- "我想做一个XX产品"
- "帮我写个PRD"
- "我有个产品想法，想做一个……"
- "帮我分析一下这个市场，看看有没有机会做个产品"

## 文件结构

```
product-design/
├── SKILL.md                     # 主文件：流程引导 + 耦合机制 + 对话控制
└── references/
    ├── methodologies.md         # 7种方法论的详细操作指南
    ├── prd-template.md          # 13章完整PRD模板
    └── research-guide.md        # 各阶段搜索策略与输出格式
```

## License

MIT
