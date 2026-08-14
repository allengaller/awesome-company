# Awesome Company 全球扩展实施计划

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 将 Awesome Company 从 20 家中美互联网巨头扩展为覆盖全球科技行业的顶级导航清单，目标约 500 家头部公司。

**Architecture:** 单文件 README.md，层级结构：H1 项目 → H2 行业大类 → H3 行业子类 → H4 地区 → H5 公司名。每家公司包含 6 个信息维度：集团官网、核心产品、技术博客、开发者社区、GitHub Org、招聘页面。

**Tech Stack:** Markdown, Git

## Global Constraints

- 所有公司信息必须通过 WebSearch/WebFetch 验证，确保链接可访问
- 中国公司使用中文标签，国际公司使用英文标签
- 多链接用 ` | ` 分隔，单链接直接列出
- 缺失字段整体省略，不留空字段
- 每个地区内公司按字母/拼音排序
- 跨行业公司按主营业务归属，避免重复
- 提交信息使用 conventional commits 格式

---

### Task 1: 结构迁移与现有公司增强

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: 现有 20 家公司数据
- Produces: 新的层级结构框架，20 家公司迁移完成并补充 GitHub/Careers 字段

- [ ] **Step 1: 备份现有 README**

```bash
cp README.md README.md.backup
```

- [ ] **Step 2: 创建新结构框架**

在 README.md 顶部建立新结构：

```markdown
# Awesome Company

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated navigation list of global technology companies — official sites, products, tech blogs, developer communities, GitHub organizations, and careers pages.

## Contents

**互联网**
- [电商](#电商) | [社交](#社交) | [内容/媒体](#内容媒体) | [游戏](#游戏) | [搜索/工具](#搜索工具)

**软件**
- [SaaS](#saas) | [开发者工具](#开发者工具) | [AI/大模型](#ai大模型) | [安全/数据库](#安全数据库)

**硬件**
- [消费电子](#消费电子) | [芯片/半导体](#芯片半导体) | [服务器/基础设施](#服务器基础设施) | [物联网](#物联网)

**周边上下游**
- [云服务](#云服务) | [支付/金融科技](#支付金融科技) | [物流/供应链](#物流供应链) | [广告技术](#广告技术)

---

## 互联网

### 电商

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 社交

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 内容/媒体

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 游戏

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 搜索/工具

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

---

## 软件

### SaaS

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 开发者工具

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### AI/大模型

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 安全/数据库

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

---

## 硬件

### 消费电子

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 芯片/半导体

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 服务器/基础设施

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 物联网

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

---

## 周边上下游

### 云服务

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 支付/金融科技

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 物流/供应链

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚

### 广告技术

#### 中国

#### 美国

#### 欧洲

#### 日韩

#### 东南亚
```

- [ ] **Step 3: 迁移现有 20 家公司到新结构**

将现有公司按新分类迁移：

**电商 → 中国：**
- 阿里巴巴、京东、拼多多、美团

**社交 → 中国：**
- 腾讯

**内容/媒体 → 中国：**
- 字节跳动、百度、网易

**消费电子 → 中国：**
- 小米、华为

**SaaS → 美国：**
- Salesforce、Oracle

**内容/媒体 → 美国：**
- Google/Alphabet、Meta、Netflix

**电商 → 美国：**
- Amazon

**消费电子 → 美国：**
- Apple、Microsoft、Tesla/X

**芯片/半导体 → 美国：**
- NVIDIA

- [ ] **Step 4: 为现有公司补充 GitHub 和 Careers 字段**

使用 WebSearch 验证并补充每家公司的：
- GitHub Organization URL（格式：`https://github.com/<org-name>`）
- 招聘页面 URL（格式：公司官网 `/careers` 或独立招聘站）

**示例（阿里巴巴）：**
```markdown
##### 阿里巴巴

- **集团官网**: [阿里巴巴集团](https://www.alibabagroup.com/)
- **核心产品**: [淘宝](https://www.taobao.com/) | [天猫](https://www.tmall.com/) | [支付宝](https://www.alipay.com/)
- **技术博客**: [阿里技术](https://developer.aliyun.com/group/alitech/article/)
- **开发者社区**: [阿里云开发者社区](https://developer.aliyun.com/)
- **GitHub**: [alibaba](https://github.com/alibaba)
- **招聘**: [阿里巴巴集团招聘](https://www.alibabagroup.com/careers)
```

**示例（Amazon）：**
```markdown
##### Amazon

- **Official Site**: [Amazon](https://www.amazon.com/)
- **Products**: [Amazon](https://www.amazon.com/) | [Prime Video](https://www.primevideo.com/) | [AWS](https://aws.amazon.com/)
- **Tech Blog**: [AWS News Blog](https://aws.amazon.com/blogs/aws/) | [Amazon Science](https://www.amazon.science/blog)
- **Developer Community**: [AWS Developer Community](https://builder.aws.com/community)
- **GitHub**: [aws](https://github.com/aws) | [amazon](https://github.com/amazon)
- **Careers**: [Amazon Jobs](https://www.amazon.jobs/)
```

- [ ] **Step 5: 验证所有链接**

使用 WebFetch 或 WebSearch 验证每个链接的可访问性，确保：
- HTTP 状态码 200
- 页面内容与链接描述匹配
- GitHub Org 页面存在且有公开仓库

- [ ] **Step 6: 提交**

```bash
git add README.md
git commit -m "feat: migrate to industry-based structure and enhance existing 20 companies with GitHub/Careers"
```

---

### Task 2: 互联网行业扩展 — 电商与社交（~100 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: 电商（~60 家）和社交（~40 家）两个子类的完整公司列表

**目标公司数量：**
- 电商：中国 ~25 家、美国 ~20 家、欧洲 ~8 家、日韩 ~4 家、东南亚 ~3 家
- 社交：中国 ~15 家、美国 ~15 家、欧洲 ~5 家、日韩 ~3 家、东南亚 ~2 家

**代表性公司示例（实现者需自行研究补充完整名单）：**

**电商 → 中国：**
- 已有：阿里巴巴、京东、拼多多、美团
- 新增：唯品会、苏宁易购、国美、当当网、小红书（电商部分）、得物、蘑菇街、什么值得买、网易严选、小米有品等

**电商 → 美国：**
- 已有：Amazon
- 新增：eBay、Walmart、Target、Costco、Shopify、Etsy、Wayfair、Best Buy、Newegg、Wish 等

**电商 → 欧洲：**
- Zalando（德国）、ASOS（英国）、Allegro（波兰）、Otto（德国）、Cdiscount（法国）等

**电商 → 日韩：**
- 乐天（日本）、Mercari（日本）、Coupang（韩国）、Gmarket（韩国）等

**电商 → 东南亚：**
- Shopee（新加坡）、Lazada（新加坡）、Tokopedia（印尼）等

**社交 → 中国：**
- 已有：腾讯
- 新增：微博、小红书（社交部分）、知乎、豆瓣、陌陌、探探、Soul、Blued、即刻、雪球等

**社交 → 美国：**
- 已有：Meta
- 新增：Twitter/X、LinkedIn、Snapchat、Pinterest、Reddit、Discord、TikTok（字节跳动国际版）、Telegram、Signal、Clubhouse 等

**社交 → 欧洲：**
- VK（俄罗斯）、Badoo（英国）、Tuenti（西班牙）等

**社交 → 日韩：**
- LINE（日本）、KakaoTalk（韩国）、Mixi（日本）等

**社交 → 东南亚：**
- Zalo（越南）、Tantan（印尼）等

- [ ] **Step 1: 研究电商公司名单**

使用 WebSearch 搜索以下关键词，收集各地区的电商公司：
- "top e-commerce companies China 2024"
- "top e-commerce companies US 2024"
- "top e-commerce companies Europe 2024"
- "top e-commerce companies Japan Korea 2024"
- "top e-commerce companies Southeast Asia 2024"

对每家公司验证：
- 官网 URL
- 核心产品（1-5 个）
- 技术博客 URL（如有）
- 开发者社区 URL（如有）
- GitHub Org URL（如有）
- 招聘页面 URL（如有）

- [ ] **Step 2: 编写电商公司条目**

按照设计文档的格式规范，为每家电商公司编写条目。

**中国公司格式：**
```markdown
##### 公司名

- **集团官网**: [公司名](URL)
- **核心产品**: [产品1](URL) | [产品2](URL) | [产品3](URL)
- **技术博客**: [博客名](URL)
- **开发者社区**: [社区名](URL)
- **GitHub**: [org-name](https://github.com/org-name)
- **招聘**: [公司招聘](URL)
```

**国际公司格式：**
```markdown
##### Company Name

- **Official Site**: [Company](URL)
- **Products**: [Product1](URL) | [Product2](URL) | [Product3](URL)
- **Tech Blog**: [Blog Name](URL)
- **Developer Community**: [Community Name](URL)
- **GitHub**: [org-name](https://github.com/org-name)
- **Careers**: [Company Careers](URL)
```

- [ ] **Step 3: 研究社交公司名单**

使用 WebSearch 搜索以下关键词，收集各地区的社交公司：
- "top social media companies China 2024"
- "top social media companies US 2024"
- "top social media companies Europe 2024"
- "top social media companies Japan Korea 2024"
- "top social media companies Southeast Asia 2024"

验证每家公司的 6 个信息维度。

- [ ] **Step 4: 编写社交公司条目**

按照格式规范编写社交公司条目。

- [ ] **Step 5: 验证所有链接**

使用 WebFetch 验证所有新增链接的可访问性。

- [ ] **Step 6: 提交**

```bash
git add README.md
git commit -m "feat: add ~100 companies in e-commerce and social media categories"
```

---

### Task 3: 互联网行业扩展 — 内容/媒体与游戏（~80 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: 内容/媒体（~50 家）和游戏（~30 家）两个子类的完整公司列表

**目标公司数量：**
- 内容/媒体：中国 ~20 家、美国 ~20 家、欧洲 ~5 家、日韩 ~3 家、东南亚 ~2 家
- 游戏：中国 ~12 家、美国 ~10 家、欧洲 ~4 家、日韩 ~3 家、东南亚 ~1 家

**代表性公司示例：**

**内容/媒体 → 中国：**
- 已有：字节跳动、百度、网易
- 新增：腾讯视频、爱奇艺、优酷、哔哩哔哩、快手、喜马拉雅、得到、知乎（内容部分）、起点中文网、晋江文学城等

**内容/媒体 → 美国：**
- 已有：Google/Alphabet、Meta、Netflix
- 新增：YouTube（Google子公司）、Twitch、Spotify、Hulu、Disney+、HBO Max、Medium、Substack、Quora 等

**内容/媒体 → 欧洲：**
- BBC（英国）、Spotify（瑞典）、Deezer（法国）、Dailymotion（法国）等

**内容/媒体 → 日韩：**
- Niconico（日本）、AbemaTV（日本）、Naver（韩国）等

**内容/媒体 → 东南亚：**
- Viu（香港）、iflix（马来西亚）等

**游戏 → 中国：**
- 新增：腾讯游戏、网易游戏、米哈游、莉莉丝、鹰角网络、完美世界、巨人网络、盛大游戏、畅游、三七互娱等

**游戏 → 美国：**
- 新增：Activision Blizzard、Electronic Arts、Epic Games、Riot Games、Valve、Roblox、Unity、Take-Two Interactive 等

**游戏 → 欧洲：**
- Ubisoft（法国）、CD Projekt Red（波兰）、Supercell（芬兰）、King（英国）等

**游戏 → 日韩：**
- Nintendo（日本）、Sony Interactive Entertainment（日本）、Square Enix（日本）、Nexon（韩国）、NCSoft（韩国）等

**游戏 → 东南亚：**
- Garena（新加坡）等

- [ ] **Step 1: 研究内容/媒体公司名单**

使用 WebSearch 搜索各地区的内容/媒体公司，验证 6 个信息维度。

- [ ] **Step 2: 编写内容/媒体公司条目**

按照格式规范编写条目。

- [ ] **Step 3: 研究游戏公司名单**

使用 WebSearch 搜索各地区的游戏公司，验证 6 个信息维度。

- [ ] **Step 4: 编写游戏公司条目**

按照格式规范编写条目。

- [ ] **Step 5: 验证所有链接**

使用 WebFetch 验证所有新增链接。

- [ ] **Step 6: 提交**

```bash
git add README.md
git commit -m "feat: add ~80 companies in content/media and gaming categories"
```

---

### Task 4: 软件行业扩展 — SaaS 与开发者工具（~90 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: SaaS（~50 家）和开发者工具（~40 家）两个子类的完整公司列表

**目标公司数量：**
- SaaS：中国 ~15 家、美国 ~25 家、欧洲 ~6 家、日韩 ~2 家、东南亚 ~2 家
- 开发者工具：中国 ~10 家、美国 ~20 家、欧洲 ~6 家、日韩 ~2 家、东南亚 ~2 家

**代表性公司示例：**

**SaaS → 中国：**
- 新增：钉钉（阿里巴巴）、企业微信（腾讯）、飞书（字节跳动）、用友、金蝶、销售易、纷享销客、北森、Moka、石墨文档、ProcessOn 等

**SaaS → 美国：**
- 已有：Salesforce、Oracle
- 新增：Microsoft（Office 365）、Google（Workspace）、Slack、Zoom、Asana、Notion、Monday.com、Atlassian、ServiceNow、Workday、HubSpot、Zendesk 等

**SaaS → 欧洲：**
- SAP（德国）、Sage（英国）、TeamViewer（德国）、Celonis（德国）等

**SaaS → 日韩：**
- Cybozu（日本）、Sansan（日本）等

**SaaS → 东南亚：**
- Zoho（印度，但在东南亚有影响力）等

**开发者工具 → 中国：**
- 新增：阿里云、腾讯云、华为云、百度智能云、火山引擎（字节跳动）、Coding.net、Gitee、Teambition 等

**开发者工具 → 美国：**
- 新增：GitHub（Microsoft）、GitLab、Atlassian（Jira/Confluence）、JetBrains、Docker、Kubernetes（CNCF）、HashiCorp、Datadog、New Relic、PagerDuty、Twilio、Stripe（开发者工具部分）等

**开发者工具 → 欧洲：**
- JetBrains（捷克）、Sentry（德国）、Contentful（德国）等

**开发者工具 → 日韩：**
- Nulab（日本）、DeployGate（日本）等

**开发者工具 → 东南亚：**
- 较少，可省略或合并到其他地区

- [ ] **Step 1: 研究 SaaS 公司名单**

使用 WebSearch 搜索各地区的 SaaS 公司，验证 6 个信息维度。

- [ ] **Step 2: 编写 SaaS 公司条目**

按照格式规范编写条目。

- [ ] **Step 3: 研究开发者工具公司名单**

使用 WebSearch 搜索各地区的开发者工具公司，验证 6 个信息维度。

- [ ] **Step 4: 编写开发者工具公司条目**

按照格式规范编写条目。

- [ ] **Step 5: 验证所有链接**

使用 WebFetch 验证所有新增链接。

- [ ] **Step 6: 提交**

```bash
git add README.md
git commit -m "feat: add ~90 companies in SaaS and developer tools categories"
```

---

### Task 5: 软件行业扩展 — AI/大模型与安全/数据库（~60 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: AI/大模型（~40 家）和安全/数据库（~20 家）两个子类的完整公司列表

**目标公司数量：**
- AI/大模型：中国 ~15 家、美国 ~18 家、欧洲 ~4 家、日韩 ~2 家、东南亚 ~1 家
- 安全/数据库：中国 ~6 家、美国 ~10 家、欧洲 ~3 家、日韩 ~1 家

**代表性公司示例：**

**AI/大模型 → 中国：**
- 新增：百度（文心一言）、阿里巴巴（通义千问）、腾讯（混元）、字节跳动（豆包）、华为（盘古）、商汤科技、旷视科技、依图科技、云从科技、科大讯飞、智谱AI、月之暗面、MiniMax、百川智能等

**AI/大模型 → 美国：**
- 新增：OpenAI、Anthropic、Google（DeepMind/Gemini）、Meta（Llama）、Microsoft（Copilot）、NVIDIA（AI平台）、Cohere、AI21 Labs、Stability AI、Hugging Face、Scale AI、Databricks 等

**AI/大模型 → 欧洲：**
- DeepMind（英国，Google子公司）、Graphcore（英国）、Darktrace（英国）等

**AI/大模型 → 日韩：**
- Preferred Networks（日本）、Naver（韩国，AI部分）等

**AI/大模型 → 东南亚：**
- 较少，可省略或合并到其他地区

**安全/数据库 → 中国：**
- 新增：奇安信、360企业安全、深信服、绿盟科技、PingCAP（TiDB）、OceanBase（蚂蚁集团）等

**安全/数据库 → 美国：**
- 新增：CrowdStrike、Palo Alto Networks、Fortinet、Okta、MongoDB、Snowflake、Databricks、Elastic、Confluent、Redis Labs 等

**安全/数据库 → 欧洲：**
- SUSE（德国）、MariaDB（芬兰）、Elastic（荷兰，但在美国上市）等

**安全/数据库 → 日韩：**
- Trend Micro（日本）等

- [ ] **Step 1: 研究 AI/大模型公司名单**

使用 WebSearch 搜索各地区的 AI/大模型公司，验证 6 个信息维度。

- [ ] **Step 2: 编写 AI/大模型公司条目**

按照格式规范编写条目。

- [ ] **Step 3: 研究安全/数据库公司名单**

使用 WebSearch 搜索各地区的安全/数据库公司，验证 6 个信息维度。

- [ ] **Step 4: 编写安全/数据库公司条目**

按照格式规范编写条目。

- [ ] **Step 5: 验证所有链接**

使用 WebFetch 验证所有新增链接。

- [ ] **Step 6: 提交**

```bash
git add README.md
git commit -m "feat: add ~60 companies in AI/ML and security/database categories"
```

---

### Task 6: 硬件行业扩展（~80 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: 消费电子（~30 家）、芯片/半导体（~25 家）、服务器/基础设施（~15 家）、物联网（~10 家）四个子类的完整公司列表

**目标公司数量：**
- 消费电子：中国 ~12 家、美国 ~10 家、欧洲 ~3 家、日韩 ~4 家、东南亚 ~1 家
- 芯片/半导体：中国 ~8 家、美国 ~12 家、欧洲 ~2 家、日韩 ~3 家
- 服务器/基础设施：中国 ~5 家、美国 ~8 家、欧洲 ~1 家、日韩 ~1 家
- 物联网：中国 ~4 家、美国 ~4 家、欧洲 ~1 家、日韩 ~1 家

**代表性公司示例：**

**消费电子 → 中国：**
- 已有：小米、华为
- 新增：OPPO、vivo、一加、realme、荣耀、联想、大疆、Anker、石头科技、追觅科技等

**消费电子 → 美国：**
- 已有：Apple、Microsoft、Tesla/X
- 新增：Dell、HP、Logitech、Sonos、GoPro、Fitbit（Google子公司）等

**消费电子 → 欧洲：**
- Philips（荷兰）、Nokia（芬兰）等

**消费电子 → 日韩：**
- Samsung（韩国）、LG（韩国）、Sony（日本）、Panasonic（日本）等

**消费电子 → 东南亚：**
- 较少，可省略

**芯片/半导体 → 中国：**
- 新增：中芯国际、华为海思、紫光展锐、寒武纪、地平线、黑芝麻智能等

**芯片/半导体 → 美国：**
- 已有：NVIDIA
- 新增：Intel、AMD、Qualcomm、Broadcom、Texas Instruments、Micron、Applied Materials、Lam Research 等

**芯片/半导体 → 欧洲：**
- ASML（荷兰）、ARM（英国）等

**芯片/半导体 → 日韩：**
- Samsung（韩国，芯片部分）、SK Hynix（韩国）、TSMC（台湾，可归类到日韩或其他）等

**服务器/基础设施 → 中国：**
- 新增：浪潮、联想（服务器部分）、华为（服务器部分）、新华三等

**服务器/基础设施 → 美国：**
- 新增：Dell Technologies、HPE、Cisco、Juniper Networks、Arista Networks、Supermicro 等

**服务器/基础设施 → 欧洲：**
- 较少，可省略

**服务器/基础设施 → 日韩：**
- Fujitsu（日本）等

**物联网 → 中国：**
- 新增：小米（IoT部分）、华为（IoT部分）、涂鸦智能、移远通信等

**物联网 → 美国：**
- 新增：Amazon（Alexa/Ring）、Google（Nest）、Particle 等

**物联网 → 欧洲：**
- Bosch（德国）等

**物联网 → 日韩：**
- Samsung（韩国，SmartThings）等

- [ ] **Step 1: 研究消费电子公司名单**

使用 WebSearch 搜索各地区的消费电子公司，验证 6 个信息维度。

- [ ] **Step 2: 编写消费电子公司条目**

按照格式规范编写条目。

- [ ] **Step 3: 研究芯片/半导体公司名单**

使用 WebSearch 搜索各地区的芯片/半导体公司，验证 6 个信息维度。

- [ ] **Step 4: 编写芯片/半导体公司条目**

按照格式规范编写条目。

- [ ] **Step 5: 研究服务器/基础设施公司名单**

使用 WebSearch 搜索各地区的服务器/基础设施公司，验证 6 个信息维度。

- [ ] **Step 6: 编写服务器/基础设施公司条目**

按照格式规范编写条目。

- [ ] **Step 7: 研究物联网公司名单**

使用 WebSearch 搜索各地区的物联网公司，验证 6 个信息维度。

- [ ] **Step 8: 编写物联网公司条目**

按照格式规范编写条目。

- [ ] **Step 9: 验证所有链接**

使用 WebFetch 验证所有新增链接。

- [ ] **Step 10: 提交**

```bash
git add README.md
git commit -m "feat: add ~80 companies in hardware categories (consumer electronics, semiconductors, servers, IoT)"
```

---

### Task 7: 周边上下游扩展（~70 家）

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 建立的结构框架
- Produces: 云服务（~20 家）、支付/金融科技（~20 家）、物流/供应链（~15 家）、广告技术（~15 家）四个子类的完整公司列表

**目标公司数量：**
- 云服务：中国 ~6 家、美国 ~10 家、欧洲 ~2 家、日韩 ~1 家、东南亚 ~1 家
- 支付/金融科技：中国 ~6 家、美国 ~10 家、欧洲 ~2 家、日韩 ~1 家、东南亚 ~1 家
- 物流/供应链：中国 ~5 家、美国 ~6 家、欧洲 ~2 家、日韩 ~1 家、东南亚 ~1 家
- 广告技术：中国 ~4 家、美国 ~8 家、欧洲 ~2 家、日韩 ~1 家

**代表性公司示例：**

**云服务 → 中国：**
- 新增：阿里云、腾讯云、华为云、百度智能云、火山引擎、京东云等

**云服务 → 美国：**
- 新增：AWS（Amazon）、Microsoft Azure、Google Cloud、IBM Cloud、Oracle Cloud、DigitalOcean、Linode、Vultr 等

**云服务 → 欧洲：**
- OVHcloud（法国）、Hetzner（德国）等

**云服务 → 日韩：**
- Naver Cloud（韩国）等

**云服务 → 东南亚：**
- 较少，可省略

**支付/金融科技 → 中国：**
- 新增：蚂蚁集团（支付宝）、腾讯金融科技（微信支付）、京东科技、度小满金融、陆金所、众安保险等

**支付/金融科技 → 美国：**
- 新增：PayPal、Stripe、Square（Block）、Visa、Mastercard、American Express、Robinhood、Coinbase、Plaid 等

**支付/金融科技 → 欧洲：**
- Adyen（荷兰）、Klarna（瑞典）、Revolut（英国）、TransferWise（英国）等

**支付/金融科技 → 日韩：**
- Rakuten Pay（日本）、Kakao Pay（韩国）等

**支付/金融科技 → 东南亚：**
- Grab（新加坡，支付部分）、GoTo（印尼，支付部分）等

**物流/供应链 → 中国：**
- 新增：菜鸟网络、京东物流、顺丰速运、中通快递、圆通速递等

**物流/供应链 → 美国：**
- 新增：UPS、FedEx、DHL（德国，但在美国有重要业务）、Amazon Logistics、Flexport 等

**物流/供应链 → 欧洲：**
- DHL（德国）、Maersk（丹麦）等

**物流/供应链 → 日韩：**
- Yamato Transport（日本）、CJ Logistics（韩国）等

**物流/供应链 → 东南亚：**
- Ninja Van（新加坡）等

**广告技术 → 中国：**
- 新增：巨量引擎（字节跳动）、腾讯广告、阿里妈妈、百度营销等

**广告技术 → 美国：**
- 新增：Google Ads、Meta Ads、Amazon Advertising、The Trade Desk、Criteo（法国，但在美国上市）、AppLovin、Unity Ads 等

**广告技术 → 欧洲：**
- Criteo（法国）、Smaato（德国）等

**广告技术 → 日韩：**
- 较少，可省略

- [ ] **Step 1: 研究云服务公司名单**

使用 WebSearch 搜索各地区的云服务公司，验证 6 个信息维度。

- [ ] **Step 2: 编写云服务公司条目**

按照格式规范编写条目。

- [ ] **Step 3: 研究支付/金融科技公司名单**

使用 WebSearch 搜索各地区的支付/金融科技公司，验证 6 个信息维度。

- [ ] **Step 4: 编写支付/金融科技公司条目**

按照格式规范编写条目。

- [ ] **Step 5: 研究物流/供应链公司名单**

使用 WebSearch 搜索各地区的物流/供应链公司，验证 6 个信息维度。

- [ ] **Step 6: 编写物流/供应链公司条目**

按照格式规范编写条目。

- [ ] **Step 7: 研究广告技术公司名单**

使用 WebSearch 搜索各地区的广告技术公司，验证 6 个信息维度。

- [ ] **Step 8: 编写广告技术公司条目**

按照格式规范编写条目。

- [ ] **Step 9: 验证所有链接**

使用 WebFetch 验证所有新增链接。

- [ ] **Step 10: 提交**

```bash
git add README.md
git commit -m "feat: add ~70 companies in ecosystem categories (cloud, fintech, logistics, adtech)"
```

---

### Task 8: 开源社区标准元素与最终审查

**Files:**
- Create: `CONTRIBUTING.md`
- Create: `LICENSE`
- Create: `CODE_OF_CONDUCT.md`
- Modify: `README.md`

**Interfaces:**
- Consumes: 所有前序任务完成的公司列表
- Produces: 完整的开源社区标准文件，最终审查通过的 README.md

- [ ] **Step 1: 创建 CONTRIBUTING.md**

```markdown
# Contributing to Awesome Company

Thank you for your interest in contributing to Awesome Company! This document provides guidelines for contributing to this project.

## How to Contribute

### Adding a New Company

1. **Verify eligibility**: The company should be a leading player in its industry (internet, software, hardware, or ecosystem).
2. **Gather information**: Collect the following information:
   - Official website
   - Core products/services (1-5)
   - Tech blog (if available)
   - Developer community (if available)
   - GitHub organization (if available)
   - Careers page (if available)
3. **Verify links**: Ensure all links are accessible and point to official pages.
4. **Follow the format**: Use the established format for company entries.
5. **Submit a pull request**: Add the company to the appropriate category and region.

### Updating Existing Information

1. **Verify the change**: Ensure the update is accurate and from an official source.
2. **Submit a pull request**: Clearly describe what changed and why.

### Reporting Issues

If you find broken links, outdated information, or other issues, please open an issue with:
- The company name
- The problematic link or information
- Suggested correction (if available)

## Format Guidelines

### Company Entry Format

**Chinese companies:**
```markdown
##### 公司名

- **集团官网**: [公司名](URL)
- **核心产品**: [产品1](URL) | [产品2](URL)
- **技术博客**: [博客名](URL)
- **开发者社区**: [社区名](URL)
- **GitHub**: [org-name](https://github.com/org-name)
- **招聘**: [公司招聘](URL)
```

**International companies:**
```markdown
##### Company Name

- **Official Site**: [Company](URL)
- **Products**: [Product1](URL) | [Product2](URL)
- **Tech Blog**: [Blog Name](URL)
- **Developer Community**: [Community Name](URL)
- **GitHub**: [org-name](https://github.com/org-name)
- **Careers**: [Company Careers](URL)
```

### Rules

- Use Chinese labels for Chinese companies, English labels for international companies
- Separate multiple links with ` | `
- Omit fields that don't exist (don't leave them empty)
- Sort companies alphabetically within each region
- Categorize companies by their primary business

## Code of Conduct

This project adheres to the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## License

By contributing, you agree that your contributions will be licensed under the [CC0 1.0 Universal License](LICENSE).
```

- [ ] **Step 2: 创建 LICENSE**

使用 CC0 1.0 Universal 许可证：

```
CC0 1.0 Universal

The person who associated a work with this deed has dedicated the work to the public domain by waiving all of his or her rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law.

You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission.

Other Information:

- In no way are the patent or trademark rights of any person affected by CC0, nor are the rights that other persons may have in the work or in how the work is used, such as publicity or privacy rights.

- Unless expressly stated otherwise, the person who associated a work with this deed makes no warranties about the work, and disclaims liability for all uses of the work, to the fullest extent permitted by applicable law.

- When using or citing the work, you should not imply endorsement by the author or the affirmer.

Full license text: https://creativecommons.org/publicdomain/zero/1.0/legalcode
```

- [ ] **Step 3: 创建 CODE_OF_CONDUCT.md**

使用 Contributor Covenant：

```markdown
# Contributor Covenant Code of Conduct

## Our Pledge

We as members, contributors, and leaders pledge to make participation in our
community a harassment-free experience for everyone, regardless of age, body
size, visible or invisible disability, ethnicity, sex characteristics, gender
identity and expression, level of experience, education, socio-economic status,
nationality, personal appearance, race, religion, or sexual identity
and orientation.

We pledge to act and interact in ways that contribute to an open, welcoming,
diverse, inclusive, and healthy community.

## Our Standards

Examples of behavior that contributes to a positive environment for our
community include:

* Demonstrating empathy and kindness toward other people
* Being respectful of differing opinions, viewpoints, and experiences
* Giving and gracefully accepting constructive feedback
* Accepting responsibility and apologizing to those affected by our mistakes,
  and learning from the experience
* Focusing on what is best not just for us as individuals, but for the
  overall community

Examples of unacceptable behavior include:

* The use of sexualized language or imagery, and sexual attention or
  advances of any kind
* Trolling, insulting or derogatory comments, and personal or political attacks
* Public or private harassment
* Publishing others' private information, such as a physical or email
  address, without their explicit permission
* Other conduct which could reasonably be considered inappropriate in a
  professional setting

## Enforcement Responsibilities

Community leaders are responsible for clarifying and enforcing our standards of
acceptable behavior and will take appropriate and fair corrective action in
response to any behavior that they deem inappropriate, threatening, offensive,
or harmful.

Community leaders have the right and responsibility to remove, edit, or reject
comments, commits, code, wiki edits, issues, and other contributions that are
not aligned to this Code of Conduct, and will communicate reasons for moderation
decisions when appropriate.

## Scope

This Code of Conduct applies within all community spaces, and also applies when
an individual is officially representing the community in public spaces.
Examples of representing our community include using an official e-mail address,
posting via an official social media account, or acting as an appointed
representative at an online or offline event.

## Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported to the community leaders responsible for enforcement at
[INSERT CONTACT METHOD].
All complaints will be reviewed and investigated promptly and fairly.

All community leaders are obligated to respect the privacy and security of the
reporter of any incident.

## Enforcement Guidelines

Community leaders will follow these Community Impact Guidelines in determining
the consequences for any action they deem in violation of this Code of Conduct:

### 1. Correction

**Community Impact**: Use of inappropriate language or other behavior deemed
unprofessional or unwelcome in the community.

**Consequence**: A private, written warning from community leaders, providing
clarity around the nature of the violation and an explanation of why the
behavior was inappropriate. A public apology may be requested.

### 2. Warning

**Community Impact**: A violation through a single incident or series
of actions.

**Consequence**: A warning with consequences for continued behavior. No
interaction with the people involved, including unsolicited interaction with
those enforcing the Code of Conduct, for a specified period of time. This
includes avoiding interactions in community spaces as well as external channels
like social media. Violating these terms may lead to a temporary or
permanent ban.

### 3. Temporary Ban

**Community Impact**: A serious violation of community standards, including
sustained inappropriate behavior.

**Consequence**: A temporary ban from any sort of interaction or public
communication with the community for a specified period of time. No public or
private interaction with the people involved, including unsolicited interaction
with those enforcing the Code of Conduct, is allowed during this period.
Violating these terms may lead to a permanent ban.

### 4. Permanent Ban

**Community Impact**: Demonstrating a pattern of violation of community
standards, including sustained inappropriate behavior,  harassment of an
individual, or aggression toward or disparagement of classes of individuals.

**Consequence**: A permanent ban from any sort of public interaction within
the community.

## Attribution

This Code of Conduct is adapted from the [Contributor Covenant][homepage],
version 2.0, available at
https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.

Community Impact Guidelines were inspired by [Mozilla's code of conduct
enforcement ladder](https://github.com/mozilla/diversity).

[homepage]: https://www.contributor-covenant.org

For answers to common questions about this code of conduct, see the FAQ at
https://www.contributor-covenant.org/faq. Translations are available at
https://www.contributor-covenant.org/translations.
```

- [ ] **Step 4: 更新 README.md 添加 Awesome 徽章**

在 README.md 顶部添加：

```markdown
# Awesome Company

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
```

- [ ] **Step 5: 最终审查**

检查以下项目：
- [ ] 所有公司数量是否达到目标（~500 家）
- [ ] 所有链接是否可访问
- [ ] 格式是否一致
- [ ] 分类是否合理
- [ ] 排序是否正确
- [ ] 是否有重复公司
- [ ] TOC 是否完整

- [ ] **Step 6: 删除备份文件**

```bash
rm README.md.backup
```

- [ ] **Step 7: 提交**

```bash
git add CONTRIBUTING.md LICENSE CODE_OF_CONDUCT.md README.md
git commit -m "docs: add open source community standard files and final review"
```

---

## 验收标准

- [ ] README.md 包含约 500 家公司
- [ ] 所有公司按行业分类组织，结构清晰
- [ ] 每家公司包含 6 个信息维度（或省略缺失字段）
- [ ] 所有链接经过验证，可访问
- [ ] 格式一致，符合 Awesome 社区标准
- [ ] 包含 CONTRIBUTING.md、LICENSE、CODE_OF_CONDUCT.md
- [ ] 包含 Awesome 徽章
- [ ] TOC 完整且链接正确
