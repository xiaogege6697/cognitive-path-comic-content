# Core Contract

## EpisodeBrief

```yaml
topic: 一句话选题
industry: legal | ai-tools | education | workplace | business | health | other
audience: 目标用户
real_question: 用户正在经历的具体问题
stakes: 损失、风险、利益或机会
known_facts: 已确认事实
unknowns: 会改变结论的未知事实
evidence_assets: 可视化证据或现象
professional_framework: 专业判断标准
common_belief: 用户通常以为A
cognitive_reversal: 实际关键是B
action: 3—5个可执行动作
scope: 地区、时间、前提和不适用情况
compliance: 不能说满或不能越界的位置
platform: 发布平台
mode: plan | prompts | generate | publish
```

## CognitivePath

```yaml
before_belief: 看前认知
after_belief: 看后认知
steps:
  - action: stop | relate | observe | classify | reverse | act
    question: 用户此刻脑中的问题
    answer: 本步唯一需要获得的答案
    evidence: 支撑答案的事实或视觉
memory_line: 全期最值得记住的一句话
final_action: 看完立即能做的动作
```

## PagePlan

```yaml
page: 1
role: cover | scene | evidence | framework | reversal | action
cognitive_action: 本页唯一认知动作
user_question: 本页回答的问题
takeaway: 本页唯一结论
panels: 1 | 2
panel_logic: single | comparison | cause-effect | before-after | scene-explanation
visual_anchor: 唯一视觉重点
evidence: 本页呈现的事实
text_budget:
  title_chars: 18
  conclusion_chars: 30
  dialogue_bubbles: 0-2
risk_notes: 易被误读或说满的位置
```

## RenderSpec

```yaml
page: 1
aspect: 3:4
style: 统一风格
characters: 角色及不变量
scene: 环境、动作、道具
composition: 一格或二格布局
text:
  l1_title: 逐字文本
  l2_conclusion: 逐字文本
  l3_dialogue: 简短对话
  l4_decoration: 可选标签
continuity: 服装、颜色、页码、系列标识
avoid: 禁止元素和错误表达
```

## QAReport

记录每页七个Gate的通过状态、问题证据和处理结果。任何关键文字错误、结论条件丢失或箭头关系错误都视为失败页。

