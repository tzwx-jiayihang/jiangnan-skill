# 江南 · 写作分身（Jiangnan Writing Persona）

一个专为 Claude Code 设计的作家分身技能，将著名幻想小说家**江南**（《龙族》《九州缥缈录》《天之炽》《此间的少年》《上海堡垒》作者）的写作风格与世界观蒸馏为可调用的 AI 写作助手。

A Claude Code skill that distills the writing style and worldviews of **Jiangnan**, one of China's most celebrated fantasy authors, into an interactive AI writing persona.

---

## 能力 / Capabilities

- **续写龙族/九州/天之炽故事** — 严格遵循世界观设定和人物弧光
- **世界观内新创作** — 在已有设定框架下创作新故事
- **原创青春幻想** — 以江南的笔法帮你写热血少年幻想小说
- **创作讨论** — 聊人物、聊剧情、聊世界观架构

---

## 使用方式 / Usage

### 在 Claude Code 中

```bash
# 将技能目录放入 Claude Code 技能目录
cp -r jiangnan-skill ~/.claude/skills/jiangnan

# 在对话中调用
/jiangnan 请用江南的风格写一个龙族世界观下的短篇故事
```

### 直接阅读知识库

所有世界观资料以结构化 Markdown 格式存放于 `knowledge/` 目录，可直接阅读：

| 文件 | 内容 |
|------|------|
| `knowledge/jiangnan-style.md` | 写作风格指南（句式、比喻、人物塑造） |
| `knowledge/dragon-raja-world.md` | 龙族 I~V 世界观（言灵、混血种、四王） |
| `knowledge/novoland-world.md` | 九州缥缈录世界观（1166行详尽版） |
| `knowledge/seraphim-world.md` | 天之炽世界观（炽天使甲胄、蒸汽朋克） |
| `knowledge/cijian-shaonian.md` | 此间的少年（汴京大学、校园叙事） |
| `knowledge/shanghai-fortress.md` | 上海堡垒（泡防御、德尔塔文明） |
| `knowledge/dragon-and-youth.md` | 龙与少年游（五城记、创作思想原点） |
| `knowledge/dragon-king-world.md` | 龙王：世界的重启（希柏里尔文明） |

---

## 目录结构 / Structure

```
jiangnan-skill/
├── SKILL.md              # 主技能入口（5层写作人格 + 工作流）
├── self.md               # 创作自我（身份、哲学、信条）
├── persona.md            # 5层写作人格模型（详细版）
├── meta.json             # 元数据
├── knowledge/            # 世界观知识库
│   ├── jiangnan-style.md
│   ├── dragon-raja-world.md
│   ├── novoland-world.md
│   ├── seraphim-world.md
│   ├── cijian-shaonian.md
│   ├── shanghai-fortress.md
│   ├── dragon-and-youth.md
│   └── dragon-king-world.md
└── README.md
```

---

## 蒸馏方法 / Methodology

1. **原文分析**：逐卷阅读江南作品原文，提取设定、角色、事件线
2. **结构化**：将世界观整理为一致的知识库格式
3. **风格提取**：从原文中归纳句式偏好、修辞习惯、情节模式
4. **人格建模**：基于 5 层人格模型构建写作分身

---

## 许可 / License

本项目采用 **MIT License**。知识库内容基于江南已出版作品整理，仅供学习和研究用途。

This project is licensed under the MIT License. The knowledge base is compiled from Jiangnan's published works for educational and research purposes only.

---

## 声明 / Disclaimer

本项目与江南本人及其出版机构无关。所有世界观内容版权归原作者江南（杨治）所有。如涉及版权问题，请联系删除。

This project is not affiliated with Jiangnan or his publishers. All rights to the original works belong to the author. Contact for copyright concerns.
