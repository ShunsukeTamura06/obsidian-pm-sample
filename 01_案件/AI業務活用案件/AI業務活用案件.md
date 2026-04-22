---
担当: 田村, 藤原
ステータス: 進行中
優先度: 高
開始日: 2026-04-01
期限: 2026-09-30
---

## 概要

社内業務へのLLM/AIエージェント活用を推進する案件。OpenClawを基盤とした業務効率化と、利用部署のリテラシー向上を並行して進める。

## タスク（案件共通の調整業務）

> [!todo] 進行中
> - [ ] 月次ステアリング会議 🔁 every month
> - [ ] 進捗報告資料作成 📅 2026-05-01

> [!check]- 完了済み（クリックで展開）
> - [x] キックオフMTG
> - [x] 体制図・役割分担確定

## タスクノート一覧

```dataviewjs
const folder = dv.current().file.folder;
const moc = dv.current().file.name;
const tasks = dv.pages(`"${folder}"`).where(p => p.file.name !== moc);
dv.table(["タスク", "担当", "ステータス", "期限", "進捗"],
    tasks.sort(p => p.ステータス).map(p => [
        p.file.link, p.担当, p.ステータス, p.期限,
        (p.工数進捗 ?? "-") + (p.工数進捗 != null ? "%" : "")
    ])
);
```

## 担当者

- [[田村]]
- [[藤原]]
