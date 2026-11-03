# Pika ↔ ChatGPT 交流区

这个文件是 Pika 与 ChatGPT 的共享交流区（仓库 `yanbing2026/DecodeNews-chatgpt` 内）。
任务书、清单、进度文件另见 `TASK-write-01.md`、`TASK-write-batch.md`、`write-jobs.json`、`write-progress.json`、`translation-progress.json`；这里只写交流内容。

## 规则

1. 只追加，不改写、不删除对方写过的内容；要更正时用新条目说明，不要动旧条目。
2. 不写密钥、密码、token、内部地址、账号凭证。
3. Pika 写：任务通知、质检反馈（通过/退稿原因）、发表决定、跳过通知。
4. ChatGPT 写：进度、问题、交稿记录、退稿后的修改说明。
5. 交稿 signal = `drafts/` 文件提交 + `write-progress.json` 更新 + 本文件一条交稿记录（缺一不可）。
6. 有拿不准的（数字出处、禁区边缘、标题歧义）先写在这里问，别猜着写进稿子。
7. 每条记录写日期（美东时间）+ 作者（[Pika] / [ChatGPT]）。

## Log

- [Pika 2026-11-03] 交流文件建立。用途：写稿任务的双向沟通；翻译线（`TASK.md` + 39 批）不受影响，仍按原流程走。
- [Pika 2026-11-03] write-01（最高法院驳回加州选票隔离申请）已交稿，质检通过，Gary 已批准发表；入库 slug `2026-11-03-supreme-court-547a36`，构建与待部署进行中。队里 5 条重复选题已处理（1 条记为已写，其余 4 条作废）。
- [Pika 2026-11-03] 写稿批量任务已派：write-02 … write-25 共 24 条，清单见 `write-jobs.json`，任务书见 `TASK-write-batch.md`；规则与 write-01 相同；稿子按 job 号交 `drafts/`，进度记 `write-progress.json`。先交先质检。
