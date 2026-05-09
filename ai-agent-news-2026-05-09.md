# AIエージェント最新ニュースまとめ (2026年5月9日)

Claude Code、Codex をはじめとする主要AIコーディングエージェントの最新動向。

---

## 1. Anthropic / Claude Code

### Code w/ Claude 2026 イベント（5月6日）
- Claude Code の **5時間利用制限を2倍に引き上げ**（Pro / Max / Team / Enterprise プラン）
- ピーク時間帯のレート制限を Pro・Max で撤廃
- SpaceX のコンピュート容量追加により Opus モデルの API 制限も引き上げ

### Claude Managed Agents — 3つの新機能（5月7日）
| 機能 | 概要 |
|------|------|
| **Dreaming（夢想）** | 過去セッションを振り返り、パターンを学習してエージェントが自己改善 |
| **Outcomes（成果定義）** | 成功基準をルーブリックで定義し、エージェントに目標を明示 |
| **Multiagent Orchestration** | リードエージェントがタスクを分割し、専門エージェントに委譲 |

### Anthropic の成長
- 2026年Q1：年換算で **80倍** の収益・利用成長（計画の10倍を大幅超過）
- **Mercado Libre**（南米最大のECプラットフォーム）：23,000人のエンジニアが Claude Code を使用、50万件以上のPRをレビュー済み、2026年Q3中に**90%自律コーディング**を目標

### Claude Opus 4.7
- LMSYS Arena リーダーボード（思考モード）で **第1位**
- SWE-bench Verified スコア：**87.6%**（全ベンダーの最高値）

---

## 2. OpenAI / Codex

### 主要アップデート（2026年4月〜5月）
- **GPT-5.5 搭載**：Codex の基盤モデルとして最新の GPT-5.5 を採用。コーディング・デバッグ・データ解析・ツール横断タスクに優れる
- **Chrome 拡張機能リリース**（5月7日）：ブラウザ上で直接 Codex が動作。Web DevTools の使用、マルチタブ操作、Webアプリのテストが可能
- **スケジュール機能**：将来のタスクを予約し、長期作業（数日〜数週間）に自動復帰
- **インアプリブラウザ**：ページに直接コメントして細かい指示が可能

### Codex の戦略変化
「リポジトリを編集するコーディングエージェント」から **「長期エンジニアリング作業のためのエージェントワークスペース」** へ転換。

### 利用者数
- 週間アクティブユーザー数：**400万人超**（年初比 8倍）

---

## 3. エディタ系AIコーディングエージェント

### Cursor
- ARR **10億ドル突破**（創業2年以内）
- Opsera との提携：Cursor IDE に DevSecOps エージェントを統合
- 総合力で **2026年ベストAIコードエディタ** と複数のレビューで評価

### Windsurf
- **Cognition に2億5,000万ドルで買収**（Googleが創業チームを24億ドルで引き抜いた後）
- Cascade 機能（自律的なファイル読取・コマンド実行・反復）が差別化ポイント

### GitHub Copilot
- 有料サブスクライバー：**470万人**、Fortune 100 の **90%** が導入
- CLI v1.0.42（5月6日）：MCP サーバー警告の改善

### ServiceNow Build Agent
- GitHub Copilot・Cursor・Windsurf・Claude Code に**統合対応**し GA リリース

---

## 4. Google / Gemini

### Google Cloud Next '26（2026年4月）
- **Gemini Enterprise Agent Platform** リリース
- **Gemma 4**：パラメータ数比で最高性能のオープンモデルと評される
- Deep Research Max：高度なデータ解析向け
- Google Colab に **Learn Mode**：Gemini がパーソナルコーディングチューターに
- 第8世代 TPU 発表

### 動向
- Gemini 3.1 Pro がコーディングベンチマークで **Tier A** 到達
- マルチモーダルタスク（画像・ドキュメント）で特に強みを発揮

---

## 5. 中国系モデル（2026年5月時点）

4社が同時期にオープンウェイトのコーディングモデルをリリース：

| モデル | 開発元 | 規模 |
|--------|--------|------|
| **DeepSeek V4** | DeepSeek | 1.6兆パラメータ（Pro）/ 2840億（Flash）、MITライセンス |
| **GLM-5.1** | Z.ai（智谱）| — |
| **MiniMax M2.7** | MiniMax | — |
| **Kimi K2.6** | Moonshot AI | — |

エージェント型エンジニアリングの能力は西洋フロンティアモデルと同等レベルに達しつつあり、**推論コストは大幅に低い**。

---

## 6. Snyk × Claude — セキュリティ連携

Snyk の AI セキュリティプラットフォームに Anthropic の Claude モデルが統合。AI コーディングエージェントが普及する中、**セキュリティリスクへの対応**が業界課題として急浮上。

---

## 全体トレンドまとめ

1. **エンタープライズ導入の加速**：大規模組織での自律コーディング比率が急上昇
2. **長期・並列タスク処理**：単発補完から「数日〜数週間のエンジニアリング作業」へシフト
3. **マルチモデル戦略**：単一モデルへのロックインから、タスク別ルーティングへ
4. **セキュリティ統合**：Snyk・Opsera などセキュリティ/DevSecOps との連携強化
5. **中国モデルの追い上げ**：性能はほぼ同等、コストは大幅に低く競合激化

---

*収集日: 2026年5月9日*

## 参照元

- [Code w/ Claude 2026 ライブブログ (Simon Willison)](https://simonwillison.net/2026/May/6/code-w-claude-2026/)
- [SD Times — 2026年5月8日 AIアップデート](https://sdtimes.com/ai/may-8-2026-ai-updates-from-the-past-week-coder-agents-launch-snyk-claude-partnership-opsera-cursor-partnership-and-more/)
- [Anthropic — Claude Managed Agents 新機能 (9to5Mac)](https://9to5mac.com/2026/05/07/anthropic-updates-claude-managed-agents-with-three-new-features/)
- [Anthropic — Dreaming 発表 (VentureBeat)](https://venturebeat.com/technology/anthropic-introduces-dreaming-a-system-that-lets-ai-agents-learn-from-their-own-mistakes)
- [Anthropic エンジニアリングブログ — Claude Code 品質レポート](https://www.anthropic.com/engineering/april-23-postmortem)
- [OpenAI Codex 公式](https://openai.com/codex/)
- [Codex Changelog 2026年4月 (Developers Digest)](https://www.developersdigest.tech/blog/codex-changelog-april-2026)
- [OpenAI Codex Chrome 拡張機能 (MacRumors)](https://www.macrumors.com/2026/05/07/openai-codex-chrome-extension/)
- [GPT-5.5 発表 (OpenAI)](https://openai.com/index/introducing-gpt-5-5/)
- [DeepSeek V4 プレビュー (TechCrunch)](https://techcrunch.com/2026/04/24/deepseek-previews-new-ai-model-that-closes-the-gap-with-frontier-models/)
- [Google 2026年4月 AI アップデート](https://blog.google/innovation-and-ai/technology/ai/google-ai-updates-april-2026/)
- [ServiceNow Build Agent 発表](https://newsroom.servicenow.com/press-releases/details/2026/ServiceNow-Build-Agent-now-works-inside-every-major-AI-coding-tool-governed-by-default/default.aspx)
- [AI Agent News April 2026 (Fazm Blog)](https://fazm.ai/blog/ai-agent-news-april-2026-claude-code-openclaw)
- [State of AI: May 2026 (Air Street Press)](https://press.airstreet.com/p/state-of-ai-may-2026)
