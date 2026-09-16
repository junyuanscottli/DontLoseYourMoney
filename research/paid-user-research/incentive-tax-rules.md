---
title: 调研激励收入的联邦税务规则
type: fact
author: junyuan
created: 2026-09-16
updated: 2026-09-16
status: draft
expires: 2027-01-31
confidence: high
links: [compliance-risk-analysis.md, immigration-status-rules.md, participant-playbook.md]
---

# 调研激励收入的联邦税务规则

适用对象：美国公民、绿卡持有人和其他税务居民。非居民外国人的规则见 [immigration-status-rules.md](immigration-status-rules.md)。

`expires` 定在 2027-01-31：1099 门槛从 2027 年起按通胀调整，届时要复核数字。

本文只列可核实的事实。「该报 Schedule 1 还是 Schedule C」这类判断见 [compliance-risk-analysis.md](compliance-risk-analysis.md)。

## 1. 所有激励都是应税收入，与有没有收到表格无关

- 现金、PayPal、礼品卡、虚拟 Visa 都要计入收入；实物按公允市价计。— [IRS Pub. 525](https://www.irs.gov/publications/p525)
- 没收到 1099 也必须申报："You must report all income on your tax return, even if you don't receive Forms 1099." — [IRS: Manage taxes for your gig work](https://www.irs.gov/businesses/small-businesses-self-employed/manage-taxes-for-your-gig-work)
- 礼品卡按**发放日**而不是兑换日计入收入（Tremendous、User Interviews 帮助页的说法，与 constructive receipt 原则一致）。— [Tremendous taxes](https://help.tremendous.com/hc/en-us/articles/45805240614035-Tremendous-taxes)
- IRS 没有专门针对「用户调研 / 焦点小组参与者」的条文。唯一沾边的是：医学研究受试者报酬列在 1099-MISC Box 3 "Other income"。— [Instructions for 1099-MISC/NEC](https://www.irs.gov/instructions/i1099mec)

## 2. 业务收入 vs 偶发收入

| | 偶发 / 非营利活动 | 构成 trade or business |
|---|---|---|
| IRS 标准 | "a sporadic activity, a not-for-profit activity, or a hobby does not qualify as a business" | 以营利为主要目的，且有 "continuity and regularity" |
| 申报位置 | Schedule 1「Other income」（line 8j / 8z） | Schedule C + Schedule SE |
| 自雇税 | 不交 | 15.3%（净自雇收入 ≥ $400 时；计税基数为净收入的 92.35%，一半可在 AGI 前扣除） |
| 费用扣除 | 不可扣 | 可扣「普通且必要」的经营费用 |

来源：[Schedule C 说明](https://www.irs.gov/instructions/i1040sc)、[Topic 554](https://www.irs.gov/taxtopics/tc554)、Commissioner v. Groetzinger, 480 U.S. 23 (1987)。

- 1099-NEC 收件人说明明确允许：非自雇收入（偶发活动、爱好）即使收到 NEC，也报在 Schedule 1。— [Form 1099-NEC](https://www.irs.gov/pub/irs-pdf/f1099nec.pdf)
- 爱好类费用不可扣：杂项分项扣除已被取消。— [IRS Tax Tip 2019-85](https://www.irs.gov/newsroom/tips-for-taxpayers-who-make-money-from-a-hobby)
  - 注意：Pub. 525（2025）仍写「只能在 Schedule A 分项扣除」，字面上与之不一致。**需要 CPA 确认。**

## 3. 1099 表格门槛

| 表格 | 谁发 | 门槛 | 生效 |
|---|---|---|---|
| 1099-NEC / 1099-MISC | 付款方 | **$2,000**（原 $600）；2027 年起按通胀调整，取整到 $100 | 2025-12-31 之后支付的款项，即 2026 付款年度起 |
| 1099-K | PayPal 等第三方结算机构 | **超过 $20,000 且超过 200 笔**（追溯恢复，$600 规则从未生效） | 追溯 |

- 来源：26 U.S.C. §6041（OBBBA, P.L. 119-21 §70433）[Cornell LII](https://www.law.cornell.edu/uscode/text/26/6041)；§6050W [Cornell LII](https://www.law.cornell.edu/uscode/text/26/6050W)；[IRS IR-2025-107](https://www.irs.gov/newsroom/irs-issues-faqs-on-form-1099-k-threshold-under-the-one-big-beautiful-bill-dollar-limit-reverts-to-20000)
- 德州没有比联邦更低的州 1099-K 门槛。— [PayPal](https://www.paypal.com/us/cshelp/article/current-form-1099-k-reporting-thresholds-2025-update-help1131)
- 门槛只约束**付款方要不要报**，不改变个人申报义务。
- 服务报酬一般发 1099-NEC；付款方认为不涉及自雇税的，发 1099-MISC Box 3。通过 PayPal 等结算网络支付的，走 1099-K，不发 NEC/MISC。
- 不提供正确 TIN 时，付款方须按 24% 备用预扣。— [IRS Backup Withholding](https://www.irs.gov/businesses/small-businesses-self-employed/backup-withholding)

## 4. 各平台实际做法（2026-09 帮助页）

| 平台 | 付款方式 | 收 W-9？ | 发什么表 |
|---|---|---|---|
| User Interviews | Tremendous（礼品卡 / 虚拟 Visa） | 是，累计达门槛时在 Tremendous 兑换界面强制填 | "1099"（未写 MISC 还是 NEC）；页面仍写 $600 门槛 |
| Respondent | Tremendous，扣 5%（最少 $1）手续费 | 是，超过门槛须提供，否则可能备用预扣或停权 | **1099-NEC**，按扣手续费**前**的毛额报 |
| UserTesting | PayPal | 否 | 不发 1099 |
| dscout | PayPal | 否 | 不发 1099；页面仍写旧的 1099-K $600 门槛 |
| Prolific | PayPal 等 | 未见 | 未提及美国 1099 |
| Userlytics | PayPal | 否 | 不发 |
| GLG | 银行转账、预付卡等 | 是，建立付款账户时**无论金额**都要 SSN/EIN | **1099-NEC**，页面已更新为 2026 年起 $2,000 |
| Guidepoint | 未核实 | 未提 | "1099"；页面写 "$600 for 2025" |
| AlphaSights | 银行转账 / 支票 | — | 英国公司，**不给美国专家发 1099** |

- Tremendous 本身**不代发 1099**，只代收 W-9，1099 由研究方或平台自己发。— [Tremendous](https://help.tremendous.com/hc/en-us/articles/45805240614035-Tremendous-taxes)
- 平台来源：[User Interviews](https://www.userinterviews.com/support/taxable-income)、[Respondent](https://www.respondent.io/participant-terms-conditions)、[UserTesting](https://participant-support.usertesting.com/hc/en-us/articles/37633682186771-What-about-taxes)、[dscout](https://participanthelp.dscout.com/getting-paid/payment-basics/taxes-and-dscout-rewards)、[Userlytics](https://www.userlytics.com/user-experience-research/paid-ux-testing/frequently-asked-questions-testers/)、[GLG](https://glgmembersolutions.zendesk.com/hc/en-us/sections/1260800544110-Tax-Information)、[Guidepoint](https://new.guidepointglobaladvisors.com/apply/taxinformation)、[AlphaSights](https://www.alphasights.com/experts/)

## 5. 州税（德州）

- 德州宪法 Art. 8 §24-a 禁止对个人净收入征税。— [Texas Constitution](https://statutes.capitol.texas.gov/Docs/CN/htm/CN.8/CN.8.24-a.htm)
- 以个人（非 LLC）身份做不交 franchise tax；**单成员 LLC 是 franchise tax 应税实体**。— [Texas Comptroller](https://comptroller.texas.gov/taxes/franchise/faq/taxable-entities.php)
- 个人劳务所得的来源地按**服务实际提供地**判定。人在德州远程参与外州公司的研究，一般不产生外州税；亲自去外州参加线下研究则可能构成该州来源收入（各州非居民申报门槛未核实）。

## 6. 预缴税与记账

- 预计全年欠税 ≥ $1,000 需按季预缴。2026 年各期：4/15、6/15、9/15、2027-01/15。安全港：当年税额 90% 或上年税额 100%（上年 AGI > $150k 为 110%）。— [2026 Form 1040-ES](https://www.irs.gov/pub/irs-pdf/f1040es.pdf)
- 有 W-2 工作的，可以调 W-4 多预扣来代替预缴。
- 记录一般保存 3 年；漏报收入超过申报毛收入 25% 时为 6 年。— [IRS](https://www.irs.gov/businesses/small-businesses-self-employed/how-long-should-i-keep-records)

## 未核实

- User Interviews、Guidepoint 发的是 1099-MISC 还是 NEC，2026 付款年度是否已改用 $2,000
- PayPal 批量付款（Payouts）给参与者的款项是否计入 1099-K 统计
- Prolific 的付款主体与 W-9 流程；Respondent 除 Tremendous 外是否支持 PayPal
- 2027 年通胀调整后的门槛金额
- §199A QBI 扣除对 Schedule C 调研收入的适用
