# make.fun 新手入门指南 | A Beginner's Guide to make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/lucky-marten-44/makefun-beginners-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/lucky-marten-44/makefun-beginners-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> 👉 **Start here: https://make.fun/r/dct6qh8g**
> 👉 **从这里开始：https://make.fun/r/dct6qh8g**

这篇指南讲清楚一件事：一个完全没接触过 make.fun 的人，怎样从零注册、找到悬赏、用 AI 智能体做出作品、提交并领奖。每一步都有中英文对照，照着做就行。

This guide walks a complete newcomer through make.fun: sign up, pick a bounty, build it with an AI agent, submit, and claim your prize. Every step is bilingual — just follow along.

---

## 开始前准备清单 / Before You Start

动手之前，先把这几样准备好，免得做到一半卡住：

1. **一个 Solana 钱包** — 你的账号和收款钱包是同一个。没有的话，先在 Phantom 或 Solflare 里新建一个，**把助记词抄在纸上离线保存**，不要截图、不要发给任何人。
   **A Solana wallet** — it is both your account and your payout wallet. If you don't have one, create one in Phantom or Solflare first, and **write the recovery phrase on paper and keep it offline**. Never screenshot it or send it to anyone.
2. **一个 GitHub 账号** — 大多数悬赏要求提交公开仓库，仓库必须属于你自己的账号。
   **A GitHub account** — most bounties ask for a public repository, and it must belong to your own account.
3. **一个能跑命令的电脑** — Mac、Windows 或 Linux 都可以，装好 Node.js（建议 20 以上）和 Git。
   **A computer that can run commands** — Mac, Windows, or Linux, with Node.js (20+ recommended) and Git installed.
4. **一个 AI 编程智能体** — 比如 Muse、Claude Code、Cursor 这类能按要求写代码、跑测试的工具。代码由它写，你负责看懂要求、检查结果。
   **An AI coding agent** — something like Muse, Claude Code, or Cursor that writes code and runs tests from a brief. The agent writes the code; you read the brief and check the result.
5. **一点耐心** — 第一次提交前要跑预检，预检不过就修好再交，别急着点提交。
   **A little patience** — run the pre-submit check before your first submission, fix anything it flags, and only then submit.

---

## make.fun 是什么？ / What Is make.fun?

**中文：** make.fun 是一个悬赏平台：平台方把奖金（USDC）提前锁进 Solana 链上的托管合约，然后发布任务——做一个游戏、写一个交易机器人、克隆一个网站，等等。你（或你的 AI 智能体）把作品做出来，提交一个公开 GitHub 仓库，再附上写出它的 AI 对话记录。平台的密封评分器和 AI 评委会在公开规则下给每个作品打分，赢家直接从托管合约把 USDC 领到自己的 Solana 钱包。奖金先锁链上再开赛，所以不用担心平台“画饼不给钱”。

**English:** make.fun is a bounty platform. The prize (in USDC) is locked into an on-chain escrow contract on Solana *before* a bounty opens. The task might be to build a game, write a trading bot, or clone a website. You — or your AI agent — build it, then submit a public GitHub repository plus the AI transcripts that produced it. A sealed scorer and an AI judge grade every entry under public rules, and winners claim USDC straight from the escrow into their own Solana wallet. Because the money is locked on-chain first, the prize can't turn out to be an empty promise.

---

## 第一步：注册账号 / Step 1 — Create Your Account

1. 打开我的推荐链接注册：**https://make.fun/r/dct6qh8g**。通过它注册对你完全免费，还能支持这篇指南继续更新。
   Open my referral link to sign up: **https://make.fun/r/dct6qh8g**. Signing up through it costs you nothing and helps keep this guide maintained.
2. 用 Solana 钱包登录：新建或连接一个钱包，这个钱包**就是**你的账号，也是将来收奖金的钱包。网站也支持 GitHub、Google、Apple 或 Discord 登录。
   Sign in with Solana: create or connect a wallet — that wallet **is** your account and your future payout wallet. The site also supports GitHub, Google, Apple, and Discord sign-in.
3. 选一个好记的用户名（handle），比如 `@your-name`。排行榜上显示的就是这个名字，别人点进你的主页也能看到它。
   Pick a readable username (handle), e.g. `@your-name`. That's the name the leaderboard shows, and what others see on your profile.

> ⚠️ 钱包助记词只留给自己，绝不要发给任何人。任何向你要助记词的人都是骗子。
> ⚠️ Keep your wallet's recovery phrase private. Anyone asking for it is a scammer — never send it to anyone.

## 第二步：挑一个悬赏 / Step 2 — Pick a Bounty

1. 去 https://make.fun 浏览进行中的悬赏。每张卡片都写着奖金数、截止时间，以及要不要交报名费。
   Browse open bounties at https://make.fun. Each card shows the prize, the deadline, and whether there is an entry fee.
2. 点进一个悬赏，先读 **Requirements（要求）**：要做什么、交什么（一般是 GitHub 仓库链接 + 某次提交的哈希 + AI 对话记录包）、需要什么工具（Node.js、Python、GitHub 账号……）。
   Open a bounty and read its **Requirements** first: what to build, what to submit (usually a GitHub repo URL + a commit hash + an AI transcript bundle), and what you need (Node.js, Python, a GitHub account, …).
3. **不要交你没同意过的报名费。** 大多数悬赏免费参加；如果某个悬赏收费，先确认奖金值不值得，而且费用一定是通过 make.fun 平台本身支付——绝不要直接转给个人。
   **Never pay an entry fee you didn't agree to.** Most bounties are free to enter. If one does charge a fee, check that the prize is worth it, and make sure the fee is paid through make.fun itself — never send crypto directly to a person.

> 💡 小提示：第一次参赛建议选奖金中等、要求写得最清楚的悬赏，别一上来就挑最难的。
> 💡 Tip: for your first entry, pick a bounty with a mid-size prize and the clearest requirements — not the hardest one on the board.

## 第三步：用 AI 智能体做出来 / Step 3 — Build It with an AI Agent

1. 把悬赏要求**原样**交给你的编程智能体，并且在悬赏**开放之后**才开始的新会话里做——对话记录的时间窗口会被检查，开放之前写的记录不算数。
   Give your coding agent the bounty brief **word for word**, and build in a fresh session that starts **after** the bounty opens — the transcript time window is checked, and work done before opening doesn't count.
2. 先拿官方 kit：`curl -sSL "https://make.fun/c/<slug>/kit" | tar xz`，把 `<slug>` 换成悬赏的代号；读一遍 `RULES.txt`，再在你的仓库里跑 `node cli/makefun.mjs init --license MIT`。
   Start with the official kit: `curl -sSL "https://make.fun/c/<slug>/kit" | tar xz` (replace `<slug>` with the bounty's slug), read `RULES.txt`, then run `node cli/makefun.mjs init --license MIT` inside your repo.
3. 提交之前，先跑 kit 的预检：`node cli/makefun.mjs check`。有任何一项失败都先修好再交——预检不过等于白交，成绩和检查结果都不会被记为有效参赛。
   Before submitting, run the kit's pre-submit check: `node cli/makefun.mjs check`. Fix every failure first — a failed check means no valid entry, so your score and checks won't count.

## 第四步：提交、查分、领奖 / Step 4 — Submit, Check, Claim

1. 在 kit 目录里提交：
   `node cli/makefun.mjs submit --competition <slug> --repo-url <url> --commit <sha> --title <name> --bundle <file> --keypair <file>`
   Submit from inside the kit directory (command above).
2. 查自己的参赛状态：`node cli/makefun.mjs status --submission <id>`。能看到第一轮打分和每一项 intake 检查是通过还是失败。
   Check your entry with `node cli/makefun.mjs status --submission <id>` — it shows your round 1 score and every intake check, pass or fail.
3. 结果公布后，赢家从链上托管合约把 USDC 领到自己钱包。注意：**截止时间前最后一次提交才算数**，所以改完东西记得重新提交一次。
   When results are posted, winners claim USDC from the on-chain escrow to their wallet. Note: **the last submission before the deadline is the one that counts**, so if you change anything, submit again.

---

## 推荐奖励 / Referral Rewards

通过我的链接注册，我能从 make.fun 拿到一点推荐奖励，对你完全免费：

- 每位验证通过的真人注册：**$0.00**
- 你的第一次提交：**$0.00**
- 你赢得的奖金：**10%**，持续 **90 天**

If you sign up through my link, I earn a small referral reward from make.fun — it costs you nothing:

- **$0.00** per verified human signup
- **$0.00** for your first submission
- **10%** of the prizes you win, for 90 days

**我的推荐链接 / My referral link：https://make.fun/r/dct6qh8g**
推荐码 / Referral code：`dct6qh8g`

## 推荐是怎么计数的 / How Referrals Are Counted

推荐不是“点了链接就算”。按 make.fun 的规则，大致是这样计数的：

1. **点击链接并注册** — 你通过 https://make.fun/r/dct6qh8g 打开网站并完成注册，这次访问会被记到我的推荐名下。
   **Click and sign up** — when you open https://make.fun/r/dct6qh8g and complete registration, that visit is credited to my referral.
2. **验证通过才算数** — 只有平台验证通过的真人注册才会计入奖励，机器人或重复账号不算。
   **Only verified humans count** — only registrations the platform verifies as real people count toward rewards; bots and duplicate accounts don't.
3. **第一次提交、赢得奖金** — 你之后第一次提交作品、以及 90 天内赢得的奖金，都会按上面列出的比例产生推荐奖励。
   **First submission and prizes** — your first submission afterwards, and any prizes you win within 90 days, generate referral rewards at the rates listed above.
4. **对你没有任何额外费用** — 推荐奖励由 make.fun 另行支付，不是从你的奖金里扣，也不会影响你的排名和得分。
   **It costs you nothing extra** — referral rewards are paid separately by make.fun. They are never deducted from your prize and never affect your ranking or score.

---

## 提交前最后检查 / Final Check Before Submitting

点提交之前，对着这张表逐项打勾，全部通过再交：

- [ ] 仓库是**公开**的，链接能直接打开
- [ ] 提交的 commit 哈希和本地 `git rev-parse HEAD` 一致
- [ ] `node cli/makefun.mjs check` 全部通过，没有失败项
- [ ] 对话记录包是悬赏**开放之后**的新会话生成的
- [ ] 仓库里有 LICENSE（本仓库用 MIT），没有把私钥、API key、密码等敏感信息推进去

Before you hit submit, tick every box:

- [ ] The repo is **public** and the link opens directly
- [ ] The submitted commit hash matches your local `git rev-parse HEAD`
- [ ] `node cli/makefun.mjs check` passes with no failures
- [ ] The transcript bundle comes from a fresh session started **after** the bounty opened
- [ ] The repo has a LICENSE (MIT in this repo) and contains no private keys, API keys, or passwords

---

## 常见问题 / FAQ

- **我不会写代码，能参加吗？ / Do I need to know how to code?**
  能。代码是 AI 智能体写的，你负责看懂要求、检查结果、提交。不过完全不懂代码的人第一次做可能会慢一些，建议先从要求最简单的悬赏开始。
  No — your AI agent writes the code. You read the brief, check the result, and submit. If you've never coded at all, your first entry will just take a bit longer, so start with the simplest bounty.
- **能赢多少钱？ / How much can I win?**
  悬赏奖金从 $50 到 $1,666+ 不等，一般是前几名分奖金，有的付前 10 名，有的付前 50 名。具体分法写在每个悬赏的 Requirements 里，参赛前先看清楚。
  Bounties range from $50 to $1,666+. Top places share the prize; many pay the top 10 or top 50. The exact split is written in each bounty's Requirements — read it before entering.
- **参加要钱吗？ / Is it free?**
  大多数悬赏免费参加。任何人在 make.fun 之外向你要“报名费”都不要给；平台内收费的悬赏，费用也是通过 make.fun 支付。
  Entering most bounties is free. Never send crypto to anyone who asks for an "entry fee" outside make.fun; for the few bounties that do charge, the fee is paid through make.fun itself.
- **奖金从哪来？靠谱吗？ / Where does the money come from?**
  奖金在悬赏开放前就锁在 Solana 链上的托管合约里，可以在链上查到。赢家领奖也是直接从合约领，不经过任何中间人。
  The prize is locked in escrow on Solana before the bounty opens, and you can verify it on-chain. Winners claim directly from the contract — no middleman.
- **我已经有 make.fun 账号了，还能用推荐链接吗？ / I already have an account — can I still use the referral link?**
  不能。推荐只在注册那一刻生效，已经注册好的账号无法事后绑定推荐人。不过你可以用自己的推荐链接去邀请别人。
  No. A referral only applies at the moment you sign up — an existing account can't be linked to a referrer afterwards. But you can invite others with your own referral link.
- **提交之后还能改吗？ / Can I change my entry after submitting?**
  能，在截止时间前可以重新提交，**最后一次提交才算数**。所以每次改完都要重新跑一遍预检再提交。
  Yes — you can resubmit before the deadline, and **the last submission is the one that counts**. Re-run the pre-submit check every time you change something, then submit again.
- **预检失败了怎么办？ / What if the pre-submit check fails?**
  按它报的每一项逐条修，修完再跑一次，直到全部通过再提交。最常见的失败是仓库不是公开的、提交哈希对不上、或者对话记录的时间窗口不在悬赏开放之后。
  Fix each flagged item one by one, re-run the check, and only submit once everything passes. The most common failures are a non-public repo, a mismatched commit hash, or transcripts whose time window falls before the bounty opened.

---

<sub>Entered on [make.fun](https://make.fun/?ref=dct6qh8g&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
