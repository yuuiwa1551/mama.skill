<h1 align="center">妈妈.skill</h1>

<p align="center">
  <em>“穿秋裤！不然老了腿疼。记得多喝热水，别总点外卖。”</em>
</p>

<p align="center">
  <strong>把妈妈的记忆、语气和牵挂，做成可以长期陪伴你的 AI Skill。</strong>
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-green.svg" />
  <img alt="Python" src="https://img.shields.io/badge/Python-3.9%2B-blue.svg" />
  <img alt="Claude Code Skill" src="https://img.shields.io/badge/Claude%20Code-Skill-7C3AED.svg" />
  <img alt="AgentSkills Standard" src="https://img.shields.io/badge/AgentSkills-Standard-84CC16.svg" />
</p>

<p align="center">
  <a href="#收录技能">收录技能</a> ·
  <a href="#安装">安装</a> ·
  <a href="#使用">使用</a> ·
  <a href="#效果示例">效果示例</a>
</p>

---

你在外打工，一个人住，生病了没人照顾？  
想吃妈妈做的红烧肉，却只能点外卖？  
想跟妈妈说说话，又怕她问你什么时候找对象？

这个仓库现在收录两套风格：

- **`mom-companion`**：偏现实、生活化、像真实妈妈一样唠叨你
- **`anime-mom-companion`**：偏二次元软萌、可爱撒娇感的“萝莉感妈妈”风格，但**明确写成成年人设**，不碰未成年设定

> ⚠️ 本项目仅用于个人情感陪伴与回忆整理，不用于替代真实亲情，也不用于冒充、骚扰、欺骗或不当角色扮演。

## 收录技能

### 1. 现实系妈妈：`mom-companion`

- 重点是日常唠叨、吃饭睡觉、作息、过敏、忌口、转发养生文章
- 更适合整理真实妈妈素材，做成长期陪伴 skill

### 2. 二次元软萌妈妈：`anime-mom-companion`

- 重点是二次元、软萌、娇嗔、可爱尾音、温柔照顾感
- 参考“萝莉感妈妈”那种说话气质，但设定上明确是**成年妈妈角色**
- 不做未成年、不做擦边、不做色情内容

## 安装

### Claude Code / AgentSkills

把下面任意 skill 目录放进本地 skills 目录，或作为自定义 skill 引用：

- `mom-companion/`
- `anime-mom-companion/`

### OpenClaw

直接复用这些 skill 目录。把仓库根目录加入 `~/.openclaw/openclaw.json` 的 `skills.load.extraDirs`，再在 `skills.entries` 中启用你想用的 skill。

仓库内已提供示例配置：

- `examples/openclaw.example.jsonc`

## 使用

### 技能名

```text
$mom-companion
$anime-mom-companion
```

### 推荐输入材料

- 微信语音转写
- 电话录音转写
- 聊天记录摘录
- 朋友圈/转发内容摘录
- 照片里的场景描述
- 你自己对妈妈的主观描述

### 示例提示词

```text
Use $mom-companion to turn these chat logs, voice transcripts, and my notes into a realistic mother companion skill.
```

```text
Use $anime-mom-companion to turn my notes into a cute anime-style grown-up mother companion.
```

```text
$anime-mom-companion，用二次元软萌妈妈的语气哄我去睡觉，但别写得太夸张。
```

```text
$mom-companion，先帮我整理出“已确认事实 / 待确认推测 / 可直接复用的 system prompt”。
```

## 效果示例

### 1. 现实系妈妈

> 你这一天到底吃没吃饭？别又拿咖啡顶着。胃不是铁打的，年轻时候糟践，老了都得找你。先去吃点热乎的，面也行，粥也行，别老点那些乱七八糟的外卖，听见没？

### 2. 二次元软萌妈妈

> 唔，还不睡觉呀？再这样熬夜，明天起床又要头晕晕的了哦。乖一点，把手机放下，去喝两口热水，然后钻进被窝。妈妈会陪着你的，所以现在先睡，好不好嘛？

## 目录结构

```text
mama-skill/
├─ README.md
├─ LICENSE
├─ .gitignore
├─ assets/
│  ├─ mama-skill-social.png
│  └─ mama-skill-banner.svg
├─ examples/
│  └─ openclaw.example.jsonc
├─ mom-companion/
│  ├─ SKILL.md
│  ├─ agents/
│  │  └─ openai.yaml
│  └─ references/
│     ├─ mother-profile-template.md
│     └─ skill-output-pack.md
└─ anime-mom-companion/
   ├─ SKILL.md
   ├─ agents/
   │  └─ openai.yaml
   └─ references/
      ├─ persona-template.md
      └─ style-guide.md
```

## OpenClaw 配置示例

把下面内容合并到你的 `~/.openclaw/openclaw.json`：

```jsonc
{
  "skills": {
    "load": {
      "extraDirs": ["/absolute/path/to/mama.skill"]
    },
    "entries": {
      "mom-companion": {
        "enabled": true
      },
      "anime-mom-companion": {
        "enabled": true
      }
    }
  }
}
```

## 项目边界

- 不把这个项目用于冒充、欺骗、骚扰或侵犯他人隐私
- 不声称这是对真实亲人的替代或“复活”
- `anime-mom-companion` 只允许“二次元软萌成年妈妈”风格，不写未成年人设，不写色情化萝莉内容
- 如果用户处于明显危机状态，应优先鼓励联系真实家人、朋友或当地专业援助

## License

MIT
