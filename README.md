<div align="center">

# MedAI 日报

**MedAI Evidence Brief — 医学人工智能证据与行业简报**

[![Static HTML](https://img.shields.io/badge/Static-HTML5-E34F26?logo=html5&logoColor=white)](./index.html)
[![Evidence Aware](https://img.shields.io/badge/editorial-evidence--aware-78e6bd)](./AGENTS.md)
[![Language](https://img.shields.io/badge/language-zh--CN-70b9ff)](./index.html)

[**在线阅读最新一期**](https://cjf128.github.io/MedAI/) · [查看项目工作流](./AGENTS.md)

</div>

> 追踪人工智能与医学交叉领域的可核验进展，并清楚区分研究证据、产业信息与临床结论。

## 项目简介

MedAI 日报是一份聚焦 **AI × 医疗健康** 的中文证据简报。项目将学术研究与行业动态分开呈现，为论文保留来源机构、发表状态与证据阶段，帮助读者快速判断一项进展“研究了什么、证据到哪一步、原文在哪里”。

收录内容必须同时满足医学 / 临床属性与 AI / 计算属性。纯医学资讯、通用 AI 新闻以及无法追溯来源的内容均不进入简报。

## 简报结构

| 一级版块 | 内容 | 呈现方式 |
| --- | --- | --- |
| 论文研究 | 重点期刊论文与高相关 ArXiv 预印本 | 按研究方向分段，标注机构、发表状态和证据阶段 |
| 行业动态 | 医疗 AI 政策、合作、融资、安全事件与产品发布 | 优先采用公司、机构或监管部门的一手来源 |

论文研究重点覆盖：

- 医学图像分割
- 疾病诊断
- 医学基础模型
- 医疗 Agent 与临床智能体
- 医学或临床场景中的世界模型
- PET/CT 核医学影像 AI

当某个方向在检索窗口内没有合格研究时，该分段会被省略，不以低相关内容凑数。

## 证据与来源

论文检索窗口为执行日前最多 90 天，优先检查以下来源，并以出版社论文页、DOI 落地页或论文原文完成核验：

| 来源类型 | 重点来源 |
| --- | --- |
| 医学影像与健康信息学期刊 | IEEE TMI、MIA、IEEE JBHI |
| Nature 系列期刊 | Nature Communications、npj Digital Medicine、Nature Biomedical Engineering |
| 预印本补充 | ArXiv |
| 行业动态 | [AI HOT](https://aihot.virxact.com/) 与一手官方来源 |

每篇论文至少核验一个大学或研究机构，并区分同行评审、Online First、Early Access、Article in Press、会议论文或预印本；同时尽可能标注回顾性研究、前瞻性试验、动物实验或概念验证等证据阶段。

## 编辑原则

- **领域匹配优先**：医学与 AI 双重相关是硬门槛。
- **期刊版本优先**：同一研究存在多个版本时，优先保留可核验的正式版本并去重。
- **摘要忠实完整**：英文摘要翻译并改写为中文，不夸大疗效，不使用超出证据的结论。
- **机构必须可核验**：无法从 affiliation 或可靠一手页面确认机构的论文不收录。
- **一手来源优先**：社交媒体与二手报道仅作为发现线索。
- **宁缺毋滥**：目标数量不高于领域相关性与证据质量。

完整的检索式、去重逻辑、证据标注与页面约束见 [AGENTS.md](./AGENTS.md)。

## 阅读体验

- 暗绿色临床简报主题，研究与行业版块使用不同强调色。
- 二级研究导航、全局编号、来源标签和证据标签便于快速定位。
- 响应式卡片布局，支持桌面与移动端阅读。
- 纯静态单文件，无 CDN、外部字体或运行时依赖。
- 保留键盘焦点、跳转正文和减少动态效果等无障碍支持。

## 项目结构

```text
MedAI/
├── index.html       # 最新一期，也是 GitHub Pages 入口
├── template.html    # 只读视觉与 DOM 模板
├── AGENTS.md        # 检索、核验、编辑、生成与归档规则
├── README.md        # 项目说明
└── daily/           # 历史日报（首次换期后创建）
    └── YYYY-MM-DD.html
```

`index.html` 固定展示最新一期。更新日期变化时，旧首页按自身日期归档到 `daily/`；同日修订不会重复归档。

## 本地查看

项目不需要安装依赖。在 Windows PowerShell 中运行：

```powershell
Start-Process .\index.html
```

也可以直接双击 `index.html`，或访问 [GitHub Pages 在线版本](https://cjf128.github.io/MedAI/)。

## 医学声明

> 本简报仅用于信息汇总与学术参考，不构成医疗建议，也不能替代专业诊断或治疗。论文与产品信息按其原始证据状态呈现，不据此推断临床疗效。
