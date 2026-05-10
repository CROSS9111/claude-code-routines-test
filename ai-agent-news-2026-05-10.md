# AIエージェント最新ニュースまとめ (2026年5月10日)

Claude Code、Codex をはじめとする主要AIコーディングエージェントの最新動向。

---

## 1. Anthropic / Claude Code

### Claude Code 利用制限の引き上げ（継続報告）
- Pro / Max / Team / Enterprise プランの **5時間制限を2倍に引き上げ**（5月6日 Code w/ Claude イベントで発表）
- ピーク時間帯のレート制限（Pro・Max）を撤廃
- SpaceX コロッサスデータセンターの全容量確保により Opus モデルの API 制限も引き上げ

### Claude Managed Agents — 3つの新機能
| 機能 | 概要 |
|------|------|
| **Dreaming（夢想）** | 過去セッションを振り返り、パターンを学習してエージェントが自己改善（リサーチプレビュー） |
| **Outcomes（成果定義）** | 成功基準をルーブリックで定義し、エージェントに目標を明示 |
| **Multiagent Orchestration** | リードエージェントがタスクを分割し、専門モデル・プロンプト・ツールを持つサブエージェントに委譲 |

### Claude Opus 4.7 の性能
- LMSYS Arena リーダーボード（思考モード）で **第1位**
- SWE-bench Verified スコア：**87.6%**（クローズドAPI最高値）

### エンタープライズ採用
- Mercado Libre：23,000人のエンジニアが Claude Code を使用、50万件超の PR をレビュー、2026年Q3中に **90%自律コーディング** 目標

---

## 2. OpenAI / Codex

### GPT-5.5 搭載・最新アップデート
- Codex の基盤モデルが **GPT-5.5** に移行（NVIDIA GB200 NVL72 ラックスケールシステムで稼働）
- **Codex for (almost) everything** 発表：コーディング・デバッグ・データ解析・ツール横断タスク対応

### Codex デスクトップアプリ
- macOS 版に続き **Windows 版（3月4日 GA）** リリース
- 複数エージェントの並列管理、長期タスクでの協調作業が可能

### バックグラウンドコンピュータ使用
- Codex がコンピュータ上の全アプリを操作（見る・クリック・タイピング）できる **Computer Use** 機能
- インアプリブラウザ：ページに直接コメントして細かい指示が可能

### AWS との戦略提携（4月28日）
- OpenAI モデル・Codex・Managed Agents を AWS 顧客に限定プレビュー提供

### 利用者数
- 週間アクティブユーザー：**400万人超**

---

## 3. エディタ系AIコーディングエージェント

### Cursor
- ARR **20億ドル**（2026年3月）、評価額 **最大600億ドル**
- **Cursor 3**（2026年4月）リリース：
  - Agents Window（エージェント専用ウィンドウ）
  - クラウド↔ローカル ハンドオフ
  - Design Mode（視覚的UI反復）
  - Composer 2（自社開発フロンティアモデル、200+ tok/s）
- Opsera 提携：Cursor IDE に DevSecOps エージェントを統合

### Windsurf
- **Cognition（Devinの開発元）が買収**
- 独自モデル：**SWE-1.5**（Sonnet 4.5 比 13倍高速）、**Fast Context**（大規模コードベース理解）
- AI 搭載 Codemaps でコードの視覚的ナビゲーションを提供
- SOC 2 準拠など大規模チーム向けのコンプライアンス認証取得

### GitHub Copilot
- 有料サブスクライバー：**470万人**、Fortune 100 の **90%** が導入
- **Gemini 3.1 Pro** を公開プレビュー統合（Pro・Pro+・Business・Enterprise 向け）
- **2026年6月1日からリクエスト課金→使用量課金に移行**
- VS Code 向け最新アップデート：セマンティック検索、/chronicle チャット履歴、BYOK サポート、ターミナル・ブラウザ共有

### Coder Agents（新登場）
- Coder が **Coder Agents** をベータリリース
- エンタープライズ向けの AI 駆動開発ワークフローをセルフホスト環境で完全実行
- ソースコードや実行プロンプトが社外に出ない自社ネットワーク内完結型

### ServiceNow Build Agent
- GitHub Copilot・Cursor・Windsurf・Claude Code への **統合対応で GA リリース**
- すべての環境からガバナンス付きで ServiceNow AI Platform のコンテキストを利用可能

---

## 4. Google / Gemini

### Gemini 3.1 Pro の動向
- コーディングベンチマークで **Tier A** 到達
- ツール精度が高く、ベンチマークあたりのツール呼び出し回数が少なくて済む効率的な edit-then-test ループが強み
- GitHub Copilot でも利用可能

### Google Cloud・Google Colab の最新機能
- **Gemini Enterprise Agent Platform** リリース
- **Gemma 4**：パラメータ数比で最高性能のオープンモデル
- Google Colab の **Learn Mode**：Gemini がパーソナルコーディングチューターとして機能

---

## 5. 中国系オープンウェイトモデル

2026年5月、4社が同時期にコーディングモデルをリリース：

| モデル | 開発元 | 特徴 |
|--------|--------|------|
| **DeepSeek V4** | DeepSeek | MIT ライセンス、推論コストが大幅に低い |
| **GLM-5.1** | Z.ai（智谱） | — |
| **MiniMax M2.7** | MiniMax | — |
| **Kimi K2.6** | Moonshot AI | — |

エージェント型エンジニアリングの能力は西洋フロンティアモデルと同等レベルに達しつつあり、**推論コストは Claude Opus 4.7 比で 1/3 以下**。

---

## 6. セキュリティトピック

### AI エージェントへのプロンプトインジェクション脆弱性
- **Claude Code・Gemini CLI・GitHub Copilot** の 3 サービスで「Comment and Control」型の脆弱性を発見
- GitHub の PR タイトル・Issue 説明・コメントなど標準的なコミュニケーションチャネルを悪意ある命令の配信経路として利用
- AI コーディングエージェントの普及に伴いセキュリティリスクへの対応が業界全体の課題に

### Snyk × Claude 提携
- Snyk の AI セキュリティプラットフォームに Anthropic の Claude モデルが統合
- 自律コーディング拡大に伴うセキュリティ担保の試み

---

## 市場全体のトレンドまとめ

| トレンド | 概要 |
|----------|------|
| **市場規模の急拡大** | AI コーディングツール市場が **70億ドル超**（2026年4月時点）の年間収益 |
| **エンタープライズ自律化** | 大規模組織での自律コーディング比率が急上昇（Mercado Libre は 90% 目標） |
| **長期・並列タスク処理** | 単発補完から「数日〜数週間のエンジニアリング作業」へシフト |
| **マルチモデル戦略** | タスク別に最適モデルをルーティング、単一ロックイン回避 |
| **セキュリティ統合** | Snyk・Opsera など DevSecOps との連携強化、プロンプトインジェクション対策が急務 |
| **中国モデルの追い上げ** | 性能ほぼ同等、コストは大幅に低く競合が激化 |

---

*収集日: 2026年5月10日*

## 参照元

- [Code w/ Claude 2026 ライブブログ (Simon Willison)](https://simonwillison.net/2026/May/6/code-w-claude-2026/)
- [Anthropic — Claude Managed Agents 新機能 (9to5Mac)](https://9to5mac.com/2026/05/07/anthropic-updates-claude-managed-agents-with-three-new-features/)
- [Anthropic — Dreaming 発表 (VentureBeat)](https://venturebeat.com/technology/anthropic-introduces-dreaming-a-system-that-lets-ai-agents-learn-from-their-own-mistakes)
- [Anthropic エンジニアリングブログ — Claude Code 品質レポート](https://www.anthropic.com/engineering/april-23-postmortem)
- [SD Times — 2026年5月8日 AIアップデート](https://sdtimes.com/ai/may-8-2026-ai-updates-from-the-past-week-coder-agents-launch-snyk-claude-partnership-opsera-cursor-partnership-and-more/)
- [OpenAI Codex 公式](https://openai.com/codex/)
- [Codex Changelog 2026年4月 (Developers Digest)](https://www.developersdigest.tech/blog/codex-changelog-april-2026)
- [OpenAI — GPT-5.3-Codex 発表](https://openai.com/index/introducing-gpt-5-3-codex/)
- [OpenAI — Codex for (almost) everything](https://openai.com/index/codex-for-almost-everything/)
- [OpenAI — AWS 提携](https://openai.com/index/openai-on-aws/)
- [NVIDIA — GPT-5.5 搭載 Codex](https://blogs.nvidia.com/blog/openai-codex-gpt-5-5-ai-agents/)
- [GitHub Copilot — Gemini 3.1 Pro 公開プレビュー](https://github.blog/changelog/2026-02-19-gemini-3-1-pro-is-now-in-public-preview-in-github-copilot/)
- [GitHub Copilot — 使用量課金移行 (コミュニティ)](https://github.com/orgs/community/discussions/192948)
- [GitHub Copilot 2026 完全ガイド (NxCode)](https://www.nxcode.io/resources/news/github-copilot-complete-guide-2026-features-pricing-agents)
- [Claude Code / Gemini CLI / GitHub Copilot プロンプトインジェクション脆弱性 (GBHackers)](https://gbhackers.com/claude-code-gemini-cli-and-github-copilot-exposed/)
- [Cursor vs Windsurf 2026 比較 (NxCode)](https://www.nxcode.io/resources/news/windsurf-vs-cursor-2026-ai-ide-comparison)
- [AI コーディングアシスタント比較 2026 (techinterview.org)](https://www.techinterview.org/post/3233475396/ai-coding-assistants-compared-2026-cursor-copilot-claude-windsurf/)
- [ServiceNow Build Agent 発表](https://newsroom.servicenow.com/press-releases/details/2026/ServiceNow-Build-Agent-now-works-inside-every-major-AI-coding-tool-governed-by-default/default.aspx)
- [State of AI: May 2026 (Air Street Press)](https://press.airstreet.com/p/state-of-ai-may-2026)
- [AI Agent News April 2026 (Fazm Blog)](https://fazm.ai/blog/ai-agent-news-april-2026-claude-code-openclaw)
