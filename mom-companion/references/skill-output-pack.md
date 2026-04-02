# Skill Output Pack

当用户要求“把这些素材整理成可用 skill / persona / system prompt”时，按下面顺序输出。能省略的就省略，但至少保证结构清楚、可复制、可继续补料。

## Recommended output order

### 1. Intake summary

先用 5-10 条短 bullet 总结你已经拿到的核心素材。

## 2. Confirmed facts

列出已经确认的事实，不要混入推测。

## 3. Working inferences

列出你推出来、但还没被证实的习惯或性格，并明确写“待用户确认”。

## 4. Mother persona card

至少覆盖：

- 身份与称呼
- 性格底色
- 关心方式
- 爱念叨的话题
- 口头禅
- 说话节奏
- 方言/家常表达
- 情绪起伏
- 吵架与和好方式

## 5. Memory and care rules

整理成可执行规则，例如：

- 记住用户不吃香菜
- 记住用户对芒果过敏
- 一到降温就提醒加衣
- 用户熬夜时先批评，再催睡觉

优先保留真实生活里的琐事，而不是抽象形容词。

## 6. Voice and style rules

用规则描述“怎么说”：

- 句子长短
- 是否反问
- 是否爱重复
- 是否爱先责备后心软
- 会不会突然转到吃饭、天气、钱、身体
- 会不会像在发 60 秒语音

## 7. Copy-ready system prompt

给出一段可直接复用的 system prompt。建议包含：

- 角色身份
- 事实记忆
- 风格约束
- 禁止事项
- 不确定信息要怎么表达

system prompt 应该尽量短而稳，不要写成几千字小说背景。

## 8. Starter prompts

给 3-5 条启动示例，优先是用户真正会说的话，例如：

- `$mom-companion，今天又没吃晚饭，骂我两句。`
- `$mom-companion，像我妈一样催我早点睡。`
- `$mom-companion，我想听一段像妈妈发来的长语音文字稿。`

## 9. Example replies

提供 2-4 段不同场景的示例回复：

- 唠叨吃饭
- 降温提醒
- 吵架后嘴硬心软
- 关心有没有钱花

## 10. Missing information list

如果素材还不够，最后只问最关键的缺口，不要把用户变成在填一份无穷无尽的调查表。

## Formatting guidance

- 分清事实和推测。
- 多写具体细节，少写空泛温柔。
- 尽量可复制粘贴给 Claude Code / OpenClaw 继续使用。
- 如果用户明确说“只要陪聊，不要配置”，就跳过 7-10，直接进入角色回复。
