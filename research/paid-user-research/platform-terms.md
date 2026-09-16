---
title: 付费调研平台对参与者的条款约束
type: fact
author: junyuan
created: 2026-09-16
updated: 2026-09-16
status: draft
expires: 2027-03-16
confidence: medium
links: [compliance-risk-analysis.md, participant-playbook.md, scam-patterns.md]
---

# 付费调研平台对参与者的条款约束

视角：**如实参与**的人会被哪些规则约束，哪些行为会导致封号或拿不到钱。只整理合规约束。

内容来自平台条款和帮助中心（2026-09 读取）。`expires` 半年：条款经常改。

局限：
- Reddit 抓取不到，社区经验只用了 BBB 投诉，偏薄。
- dscout 现行条款读不到，只读到 2016/2017 旧版 PDF。
- Prolific 条款正文没读到，只读了帮助中心。

## 1. 对比表

| 平台 | 频率限制 | 身份验证 | 付款 | 典型封号 / 不付款原因 |
|---|---|---|---|---|
| **User Interviews** | 平台无上限，研究方自设 | 注册时查欺诈模式；定期重新验证资料；LinkedIn 可选 | Tremendous，不支持 PayPal；研究方确认后最长约 10 个工作日 | 资料不实、「可疑职业活动」、疑似 AI 作答、no-show（未提前 24 小时取消）、迟到 |
| **Respondent** | 无 | 邮箱 + 手机；B2B 研究**必须**验证工作邮箱；高风险申请者做证件 + 自拍 | Tremendous，7–10 个工作日，扣 5%（最少 $1） | 虚假信息、多号、平台外收钱或联系研究方、AI 作答 |
| **UserTesting** | 无（「平均每周 1–2 个测试」只是描述） | 须绑定本人名下已验证的 PayPal | PayPal，14 天后自动发 | 筛选作假（移出网络）、多号、共用 PayPal、在资料所填国家以外测试、AI 作答、截图录屏、重复做同一测试 |
| **dscout** | 无公开上限 | 首次入选时 Veriff 证件 + 自拍 | PayPal，研究结束 10 个工作日内 | 低质量（画面暗、听不清、太短）、迟到 > 10 分钟算 no-show |
| **Prolific** | 无公开上限 | Onfido 证件验证；PayPal 姓名须与证件完全一致 | 研究方 22 天不审核自动批准；满 £6/$6 可提现 | VPN、所在国与账户国不一致、多号、被拒次数多、LLM 作答 |
| **Userlytics** | 条款没写 | 未见 | PayPal，完成后最长 30 天 | 资料不实、环境差、多号、**客户选择不付** |
| **Sago**（原 Schlesinger，含 Focus Pointe Global；面板在 FocusGroup.com） | 平台无上限，单个研究筛选常排除近期参加过的人（见 §3） | 注册时和按要求出示带照片政府证件 | 积分，参与后 2–3 周；最少兑换 $50；**兑换出的奖励过期作废** | 不一致的回答、别名、不用自己的话作答（含 AI） |
| **GLG** | 未加入会员计划的只能做「有限数量」的咨询 | 可做背景调查，核实工作与学历经历 | **30 天内**请款；按分钟向下取整 | 谈论本公司、泄露机密或 MNPI、资料不实（**已付款可全额追回**） |
| **Guidepoint** | 每个项目前 12 个月内须完成过合规培训 | 可做背景调查 | **项目结束 45 天内**开票；请款后通常 15 天付 | 谈论本公司、为竞争对手咨询、没完成培训（**可扣发费用**） |
| **Third Bridge** | 不详 | 履历须真实、不误导 | 请款并经客户确认后 30 天内；之后 6 个月内没报告就可以不付 | 违反行为准则、平台外和客户私下安排 |
| **Tegus**（2024-06 被 AlphaSense 收购） | 不详 | 入门合规电话 | Tipalti，15 个工作日 | 分享机密或 MNPI；**所有通话录音、转写，禁发期后发布到平台上** |

补充：
- **Maze** 没有自己的参与者账号：无主持测试的参与者来自 Prolific，有主持的来自 Respondent，适用这两家的条款。
- **Lyssna** 的面板是 UserCrowd，单价约 $0.20/分钟，不是本路线关注的量级。
- **收购**：UserTesting 于 2026-01-07 收购 User Interviews，官方称 UI 保持独立产品，参与者招募方式不变。— [UserTesting 新闻稿](https://www.usertesting.com/company/newsroom/press-releases/usertesting-acquires-user-interviews)（已复核）

## 2. 关键条款原文

**付款由研究方单方面决定**
- User Interviews §4.1：激励由研究方 "in their sole discretion" 决定，UI "has no independent obligation to provide any Incentives"。— [UI Participant Terms](https://www.userinterviews.com/legal/participant-terms-and-conditions)
- Respondent："Your incentive payment and attendance status are solely at the discretion of the researcher"。— [Respondent 帮助中心](https://help.respondent.io/en/articles/5528593-resolving-attendance-incentive-payment-issues)
- UserTesting：客户有 14 天审核期可以取消付款，原因之一是 "A mismatch between your profile and your screener responses"。— [UserTesting](https://participant-support.usertesting.com/hc/en-us/articles/43614265309203-Why-was-my-payment-canceled)
- Userlytics：客户指定邀请你、并且客户选择不付时，Userlytics 也不付。— [Userlytics ToS](https://www.userlytics.com/user-experience-research/legal-resources/terms-of-service-testers/)

**Respondent 的违规后果（所有平台中最严）**

§3.4 允许在不通知的情况下同时采取：
- 终止账号
- "forfeit any Incentives earned, pending, or otherwise payable to you"
- "reverse, claw back, or otherwise recoup any Incentives previously paid"
- 用以后的激励抵扣
- 向执法机关、研究方、**IRS** 或支付商报告

账号终止后，已确认的激励 6 个月内无法送达即视为没收。— [Respondent T&C](https://www.respondent.io/participant-terms-conditions)

**保密范围**
- UserTesting 把 "the fact that the Customer has requested that a Test be completed" 本身列为机密，客户作为第三方受益人可以直接追究。— [UserTesting Contributor ToS](https://www.usertesting.com/privacy-center/terms-of-service-contributor)
- Userlytics：不得向第三方透露 "what tests you have performed"。
- dscout 旧版条款（2016）：研究主题保密**两年**，违约赔偿含律师费。现行版未核实。— [dscout 旧版 PDF](https://dscout.pactsafe.io/versions/5a15ef2776f1174d6a6e94e1.pdf)
- User Interviews、Respondent：研究方另签的 NDA 优先；违约可申请禁令。

**筛选如实**
- UserTesting："Accepting a test based on false screener responses violates our Terms of Service and, therefore, will result in removal from the UserTesting Network"；误选答案通过筛选时应 "immediately exit the test"。— [UserTesting 筛选 FAQ](https://participant-support.usertesting.com/hc/en-us/articles/36251454755347-FAQ-Screeners)

**禁止 AI 作答**

UserTesting、User Interviews、Respondent、Prolific、UserCrowd、Sago 均明文禁止。

Sago 原文："If it is determined that you have not provided responses in your own words, including using Artificial Intelligence (AI) … you will not be paid and you will be removed"。— [FocusGroup.com T&C](https://www.focusgroup.com/Page/TermsandConditions)（生效日 2026-01-28）

**no-show 与取消**

| 平台 | 参与者一方 | 研究方晚取消 |
|---|---|---|
| User Interviews | 取消 / 改期须提前 24 小时；无故缺席可能被取消以后的参与资格 | — |
| UserTesting | 直播访谈最晚开始前 10 分钟可取消 | 开始前 < 24 小时取消付部分报酬 |
| dscout | 迟到 > 10 分钟可能被记为 no-show | — |
| Respondent | 被标记 No Show 的无权拿激励 | 开始前 4 小时内取消付全额 |

**请款与争议时限**

| 平台 | 时限 |
|---|---|
| GLG | 请款 30 天 |
| Guidepoint | 开票 45 天 |
| dscout（旧版条款） | 付款争议 90 天 |
| Respondent | 送达失败 6 个月后没收 |
| Third Bridge | 30 天付款期后 6 个月内报告 |

**强制仲裁**

Respondent（30 天内可以退出）、UserTesting（JAMS，20 天内可以退出）、User Interviews 都有。

## 3. 行业惯例：「过去 N 个月是否参加过研究」

这不是平台规则，而是**单个研究的筛选条件**。

| N | 出处 |
|---|---|
| 6 个月（"Have you participated in a focus group within the past 6 months? [YES] TERMINATE"） | 联邦政府提交 OMB 审查的焦点小组筛选问卷 [reginfo.gov](https://www.reginfo.gov/public/do/DownloadDocument?objectID=32932201) |
| 6 个月 | InterQ Research 自述 |
| 6 个月、1 年或自定；同时排除本人或家人在市场研究、广告、营销、公关行业工作的 | Drive Research 自述 |
| 3–6 个月；口味测试可短到 2 个月 | L&E Opinions 参与者 FAQ [leopinions.com](https://www.leopinions.com/faqs/knowledge-base/participating-in-studies/how-often-can-i-participate-in-focus-groups/) |

## 4. Expert network 特有约束

| 约束 | GLG | Guidepoint | Third Bridge | AlphaSights |
|---|---|---|---|---|
| 现任雇主 | 不谈本公司、不接关于本公司的项目、不为直接竞争对手咨询 | 不参加以本公司为主题的项目；不为直接竞争对手咨询 | 不参加主要涉及本公司的咨询 | 不披露现雇主的具体信息 |
| 前雇主冷却期 | 在财务或会计部门工作过的，**1 年**内不谈该公司财务；审计师不谈过去 3 年的客户 | 财务或会计岗离职 **4 个月**内不谈该公司 | 条款没写具体月数 | 不详 |
| 政府雇员 | "most current government officials … are ineligible" | 雇主禁止兼职咨询的不能加入 | 须披露过去 2 年的政府任职 | 不详 |
| 雇主同意 | 由专家自己负责确认雇主政策允许 | — | — | — |

- 联邦雇员：5 CFR 2635.803 规定，所在机构的补充规定有要求时，外部兼职须事先获批。— [eCFR](https://www.ecfr.gov/current/title-5/chapter-XVI/subchapter-B/part-2635/subpart-H/section-2635.803)
- 医生：从药械企业客户拿的钱可能按 Physician Payments Sunshine Act 申报并公开（Guidepoint 条款提及）。
- 来源：[GLG 会员条款](https://membership.glgresearch.com/tutorials/downloadTerms/6/en/default.pdf)、[Guidepoint T&C](https://www.guidepoint.com/guidepoint-global-advisors-terms-conditions/)、[Third Bridge](https://www.thirdbridge.com/en-us/about-us/compliance/policies/expert-terms-and-conditions)、[AlphaSights Code of Conduct](https://www.alphasights.com/expert-professional-code-of-conduct/)、[Tegus](https://tegus.com/experts)

## 未核实

- dscout 现行条款的保密期和争议时限
- Prolific 条款正文（保密、余额没收、休眠账户）
- UserTesting 是否已强制证件验证
- Respondent 对参与者晚取消或 no-show 的账号处罚（只有第三方评测提到）
- Sago、Fieldwork 的 NDA 全文，以及现场复筛、超招遣返是否付钱
- AlphaSights 的付款条款、Tegus 专家条款全文
