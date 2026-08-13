# Awesome Company Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a comprehensive Awesome-style navigation list of 20 major Chinese and US internet companies with their official sites, product pages, social media accounts, tech blogs, and developer communities.

**Architecture:** Single README.md file using hierarchical list format with inline labels. Chinese companies use Chinese labels, US companies use English labels. Each company is a `###` section with nested bullet points for different link categories.

**Tech Stack:** Markdown, Git

## Global Constraints

- File: `README.md` in repository root
- Format: Hierarchical list (方案 B), not tables
- Chinese companies: Chinese labels (集团官网, 子公司, 产品, 自媒体, 技术博客, 开发者社区)
- US companies: English labels (Official Site, Products, Tech Blog, Developer Community)
- Social media format: `微信公众号: 名称` / `微博: @名称` (plain text, no links)
- Missing fields: omit entirely, no empty placeholders
- Multiple links on same line: separated by ` | `
- All links must be verified via web search before inclusion

---

### Task 1: Chinese Companies — Batch 1 (Alibaba, Tencent, ByteDance, Baidu, JD)

**Files:**
- Modify: `README.md`

**Interfaces:**
- Produces: README.md with 5 Chinese company sections

- [ ] **Step 1: Research and verify links for Alibaba**

Search for and verify:
- 阿里巴巴集团官网
- 子公司: 蚂蚁集团, 阿里云, 菜鸟
- 产品: 淘宝, 天猫, 支付宝, 钉钉
- 技术博客: 阿里技术
- 开发者社区: 阿里云开发者社区
- 微信公众号/微博账号名

- [ ] **Step 2: Research and verify links for Tencent**

Search for and verify:
- 腾讯官网
- 子公司: 腾讯云, 腾讯游戏
- 产品: 微信, QQ, 腾讯视频
- 技术博客: 腾讯技术工程
- 开发者社区: 腾讯云开发者社区
- 微信公众号/微博账号名

- [ ] **Step 3: Research and verify links for ByteDance**

Search for and verify:
- 字节跳动官网
- 产品: 抖音, TikTok, 今日头条, 飞书, 剪映
- 技术博客: 字节跳动技术团队
- 开发者社区: 字节跳动开发者社区
- 微信公众号/微博账号名

- [ ] **Step 4: Research and verify links for Baidu**

Search for and verify:
- 百度官网
- 产品: 百度搜索, 百度地图, Apollo, 文心一言
- 技术博客: 百度技术
- 开发者社区: 百度开发者中心
- 微信公众号/微博账号名

- [ ] **Step 5: Research and verify links for JD**

Search for and verify:
- 京东官网
- 子公司: 京东物流, 京东云
- 产品: 京东商城
- 技术博客: 京东技术
- 开发者社区: 京东云开发者社区
- 微信公众号/微博账号名

- [ ] **Step 6: Write Alibaba section to README.md**

- [ ] **Step 7: Write Tencent section to README.md**

- [ ] **Step 8: Write ByteDance section to README.md**

- [ ] **Step 9: Write Baidu section to README.md**

- [ ] **Step 10: Write JD section to README.md**

- [ ] **Step 11: Commit**

```bash
git add README.md
git commit -m "feat: add Chinese companies batch 1 (Alibaba, Tencent, ByteDance, Baidu, JD)"
```

---

### Task 2: Chinese Companies — Batch 2 (Meituan, Pinduoduo, NetEase, Xiaomi, Huawei)

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: README.md from Task 1
- Produces: README.md with all 10 Chinese company sections

- [ ] **Step 1: Research and verify links for Meituan**

Search for and verify:
- 美团官网
- 产品: 美团外卖, 大众点评
- 技术博客: 美团技术团队
- 开发者社区: 美团开发者社区
- 微信公众号/微博账号名

- [ ] **Step 2: Research and verify links for Pinduoduo**

Search for and verify:
- 拼多多官网
- 产品: 拼多多, Temu
- 技术博客: 拼多多技术
- 微信公众号/微博账号名

- [ ] **Step 3: Research and verify links for NetEase**

Search for and verify:
- 网易官网
- 子公司: 网易游戏
- 产品: 网易云音乐, 网易有道
- 技术博客: 网易技术
- 开发者社区: 网易云开发者社区
- 微信公众号/微博账号名

- [ ] **Step 4: Research and verify links for Xiaomi**

Search for and verify:
- 小米官网
- 产品: MIUI, 小米IoT
- 技术博客: 小米技术
- 开发者社区: 小米开发者社区
- 微信公众号/微博账号名

- [ ] **Step 5: Research and verify links for Huawei**

Search for and verify:
- 华为官网
- 子公司: 华为云
- 产品: 鸿蒙(HarmonyOS), 华为消费者业务
- 技术博客: 华为技术
- 开发者社区: 华为开发者联盟
- 微信公众号/微博账号名

- [ ] **Step 6: Write Meituan section to README.md**

- [ ] **Step 7: Write Pinduoduo section to README.md**

- [ ] **Step 8: Write NetEase section to README.md**

- [ ] **Step 9: Write Xiaomi section to README.md**

- [ ] **Step 10: Write Huawei section to README.md**

- [ ] **Step 11: Commit**

```bash
git add README.md
git commit -m "feat: add Chinese companies batch 2 (Meituan, Pinduoduo, NetEase, Xiaomi, Huawei)"
```

---

### Task 3: US Companies — Batch 1 (Google, Meta, Amazon, Apple, Microsoft)

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: README.md from Task 2
- Produces: README.md with 5 US company sections

- [ ] **Step 1: Research and verify links for Google/Alphabet**

Search for and verify:
- Alphabet官网, Google官网
- Products: Google Search, YouTube, Android, Google Cloud, DeepMind
- Tech Blog: Google AI Blog, Google Developers Blog
- Developer Community: Google Developers

- [ ] **Step 2: Research and verify links for Meta**

Search for and verify:
- Meta官网
- Products: Facebook, Instagram, WhatsApp, Messenger
- Tech Blog: Meta Engineering, Meta AI Blog
- Developer Community: Meta for Developers

- [ ] **Step 3: Research and verify links for Amazon**

Search for and verify:
- Amazon官网
- Subsidiaries: AWS
- Products: Amazon电商, Prime Video
- Tech Blog: AWS News Blog, Amazon Science
- Developer Community: AWS Developer Community

- [ ] **Step 4: Research and verify links for Apple**

Search for and verify:
- Apple官网
- Products: iPhone, App Store, iCloud, Apple Music
- Tech Blog: Apple Machine Learning Research
- Developer Community: Apple Developer

- [ ] **Step 5: Research and verify links for Microsoft**

Search for and verify:
- Microsoft官网
- Subsidiaries: GitHub, LinkedIn
- Products: Azure, Office 365, Xbox
- Tech Blog: Microsoft Dev Blogs, Microsoft Research Blog
- Developer Community: Microsoft Developer Community

- [ ] **Step 6: Write Google/Alphabet section to README.md**

- [ ] **Step 7: Write Meta section to README.md**

- [ ] **Step 8: Write Amazon section to README.md**

- [ ] **Step 9: Write Apple section to README.md**

- [ ] **Step 10: Write Microsoft section to README.md**

- [ ] **Step 11: Commit**

```bash
git add README.md
git commit -m "feat: add US companies batch 1 (Google, Meta, Amazon, Apple, Microsoft)"
```

---

### Task 4: US Companies — Batch 2 (Netflix, Tesla/X, NVIDIA, Salesforce, Oracle)

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: README.md from Task 3
- Produces: README.md with all 20 company sections complete

- [ ] **Step 1: Research and verify links for Netflix**

Search for and verify:
- Netflix官网
- Tech Blog: Netflix TechBlog
- Developer Community: Netflix Open Source

- [ ] **Step 2: Research and verify links for Tesla/X**

Search for and verify:
- Tesla官网, X(Twitter)官网
- Tech Blog: Tesla AI, X Engineering
- Developer Community: X Developer Platform

- [ ] **Step 3: Research and verify links for NVIDIA**

Search for and verify:
- NVIDIA官网
- Products: GeForce, CUDA, Omniverse
- Tech Blog: NVIDIA Technical Blog
- Developer Community: NVIDIA Developer

- [ ] **Step 4: Research and verify links for Salesforce**

Search for and verify:
- Salesforce官网
- Products: Sales Cloud, Service Cloud, Slack
- Tech Blog: Salesforce Engineering
- Developer Community: Salesforce Developers

- [ ] **Step 5: Research and verify links for Oracle**

Search for and verify:
- Oracle官网
- Products: Oracle Cloud, Oracle Database, Java
- Tech Blog: Oracle Blogs
- Developer Community: Oracle Developer Community

- [ ] **Step 6: Write Netflix section to README.md**

- [ ] **Step 7: Write Tesla/X section to README.md**

- [ ] **Step 8: Write NVIDIA section to README.md**

- [ ] **Step 9: Write Salesforce section to README.md**

- [ ] **Step 10: Write Oracle section to README.md**

- [ ] **Step 11: Add project header and table of contents to README.md**

Add at the top of README.md:
- Project title and description
- Awesome badge (optional)
- Table of contents with anchor links to each company section

- [ ] **Step 12: Final review and link check**

- Verify all markdown renders correctly
- Spot-check a sample of links for validity
- Ensure consistent formatting across all sections

- [ ] **Step 13: Commit**

```bash
git add README.md
git commit -m "feat: add US companies batch 2 and finalize README (Netflix, Tesla/X, NVIDIA, Salesforce, Oracle)"
```
