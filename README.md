# shunsoco-stack

業務の複雑さを、迷わず使えるWeb体験へ。

日本の小規模事業者や現場業務を想定したWebアプリ、業務システムを設計・実装しています。画面だけでなく、権限、データモデル、計算根拠、失敗時の復旧、テスト、公開後の運用までを一つの成果物として扱います。

## 公開中のプロジェクト

### AI調達・仕入先選定エージェント

調達要件から、Evidence付きのSupplier調査、不足情報の再調査、通常コードによる重み付き評価、交渉Draft、Human Reviewまでを一つのWorkspaceで支援するConcept Projectです。

- Stack: Next.js 16 / React 19 / TypeScript / Zod / Vitest / Vercel
- Demo: https://ai-procurement-supplier-agent.vercel.app
- Source: https://github.com/shunsoco-stack/ai-procurement-supplier-agent
- Note: Verified snapshot / External AI OFF / Human approval required

### 売上管理システム

売上登録、目標管理、顧客・商品・担当者・店舗別分析、CSV、監査ログを統合したConcept Projectです。整数円の金額計算とFirestore Security Rulesを重点的に検証しています。

- Stack: Next.js / React / TypeScript / Firebase / Recharts / Vitest
- Source: https://github.com/shunsoco-stack/sales-management-system
- Demo: https://sales-management-system-three-sage.vercel.app/demo/

### 在庫管理システム

複数拠点の入出庫、在庫移動、棚卸、履歴、権限、CSVを一元管理するConcept Projectです。Firebase Security RulesとEmulatorテストまで含めて検証しています。

- Stack: Next.js / React / TypeScript / Firebase / Recharts / Vitest
- Source: https://github.com/shunsoco-stack/inventory-management-system
- Demo: 未公開

### 個人事業主向け税金予測シミュレーター

売上、経費、控除から税金・社会保険料の概算と資金見通しを可視化するConcept Projectです。

- Stack: Next.js / React / TypeScript / Recharts / Firebase Hosting / Vitest
- Demo: https://freelance-tax-kj-019fe135.web.app/
- Source: https://github.com/shunsoco-stack/freelance-tax-simulator
- Note: 表示結果は概算であり、税務上の判断や申告の代替ではありません。

## 現在公開している領域

- AIエージェント: 根拠付きの調査、比較、不足情報の再調査、評価、Human Reviewを扱う意思決定支援
- 業務システム: 売上、在庫、履歴、検索、分析、権限を扱う業務データ管理
- 業務支援Webアプリ: 税金・社会保険料の概算と資金見通しの可視化
- 品質設計: TypeScript、Vitest、Testing Library、Firebase Emulator / Rulesテスト、静的解析

## Engineering principles

- APIキーがなくても主要フローを確認できるDemo Modeを用意する
- 計算、権限、保存などの重要処理を、検証可能なドメインロジックとして分離する
- 秘密情報をrepositoryへ含めず、`.env.example`と最小権限で構成する
- READMEに実装済み範囲、制約、検証方法、公開デモを明記する
- PC、タブレット、スマートフォン、キーボード操作、reduced motionを考慮する

## Stack

`Next.js` · `React` · `TypeScript` · `Firebase` · `Tailwind CSS` · `Vitest` · `Testing Library`

公開repositoryは、設計力と実装力を確認できる **Concept Project / 自主制作** です。実運用データを扱うプロジェクトは、セキュリティ上Privateで管理します。
