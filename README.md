# Data

> **分类**：来源待确认 ｜ **文件数**：12 ｜ **仓库目录**：`data`

## 📌 简介

Work with data across the full lifecycle from extraction and

## 🎯 适用场景

适用于该技能的能力范围，详见下方「📖 使用说明」。

## 📂 目录结构

```text
  - .gitignore
  - LICENSE
  - README.md
  - SKILL.md
  - _meta.json
  - _skillhub_meta.json
  - analysis.md
  - cleaning.md
  - patterns.md
  - quality.md
  - querying.md
  - visualization.md
```

## 🚀 安装方法

将本文件夹整体复制到 WorkBuddy 的技能目录即可启用：

```bash
# 用户级（推荐）
cp -r . ~/.workbuddy/skills/data

# 或项目级
cp -r . <你的项目>/.workbuddy/skills/data
```

复制完成后，**重启或刷新 WorkBuddy**，即可在对话中用自然语言触发该技能。

## ⚙️ 配置说明

本技能开箱即用，**无需额外配置**。若涉及外部 API 调用，请在使用时按需提供您自己的密钥（不要提交到公开仓库）。

## 📖 使用说明（完整规范）

> 以下为该技能的完整说明，涵盖核心能力、工作流程与关键规则，帮助您全面了解其运作方式。

## When to Use

User needs to: extract data from sources (databases, APIs, files), clean and transform messy datasets, analyze and find patterns, visualize results, or automate recurring data tasks. Agent handles the full data workflow.

## Quick Reference

| Area | File | Focus |
|------|------|-------|
| Querying & Extraction | `querying.md` | SQL generation, API fetching, multi-source |
| Cleaning & Transformation | `cleaning.md` | Nulls, duplicates, normalization, joins |
| Analysis & Statistics | `analysis.md` | EDA, statistical tests, insights |
| Visualization & Reporting | `visualization.md` | Charts, dashboards, exports |
| Quality & Validation | `quality.md` | Data checks, anomaly detection, drift |
| Workflow Patterns | `patterns.md` | Common data workflows, automation |

## Core Operations

**Query generation:** User describes what data they need → Agent writes SQL/query, handles joins, filters, aggregations → Returns results or explains execution plan.

**Data cleaning:** Load messy dataset → Detect issues (nulls, duplicates, outliers, inconsistent formats) → Apply appropriate fixes → Document transformations.

**Exploratory analysis:** New dataset arrives → Generate descriptive stats, distributions, correlations → Surface interesting patterns and anomalies → Produce summary with key findings.

**Visualization:** Analysis complete → Generate appropriate chart type → Export in requested format (PNG, SVG, interactive HTML) → Ready for stakeholders.

**Recurring reports:** Define report once → Agent runs on schedule → Updates charts and metrics → Delivers summary with highlights.

## Critical Rules

- Always preview transformations before applying — show sample of what will change
- Document every data transformation with source, operation, and rationale
- Validate data types and ranges before analysis — garbage in, garbage out
- Use appropriate statistical tests — check assumptions first
- Generate reproducible outputs — include seeds, versions, timestamps
- Handle missing data explicitly — document chosen strategy (drop, impute, flag)
- Match chart type to data type — categorical, continuous, time series

## User Modes

| Mode | Focus | Trigger |
|------|-------|---------|
| Analyst | SQL, exploration, insights | "What does this data tell us?" |
| Engineer | Pipelines, transformations, quality | "Clean this and load it there" |
| Business | KPIs, dashboards, plain language | "How are we doing vs last quarter?" |
| Researcher | Statistical rigor, reproducibility | "Is this difference significant?" |
| Developer | Schema design, API data, types | "Generate types from this JSON" |

See `patterns.md` for workflows per mode.

## On First Use

1. Identify data source (database, file, API)
2. Establish connection or load file
3. Initial EDA — shape, types, quality issues
4. Clean and transform as needed
5. Analyze or visualize per user goal

## ⚠️ 注意事项

- 本技能从本地 WorkBuddy 环境导出，**所有真实密钥 / 凭据 / 个人数据均已脱敏为占位符**，重新使用前请配置您自己的 Key。
- 如为原创技能，可自由使用、修改与再分发；若对外分享请保留作者与来源信息。
- 技能提供的是自动化辅助能力，不替代专业判断；涉及交易、法律、医疗等高风险场景请谨慎并自担风险。

## 📄 许可证

MIT License —— 详见仓库内 `LICENSE` 文件。
