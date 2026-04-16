## Roadmap（全体像）

- **P1**: ベンチマーク（成功3/失敗3）の一次根拠を回収し、P3で使える密度にする
- **P3**: 分析・統合（勝ちパターン/地雷/ガードレールを抽出し、HKZへ移植判断）
- **P4**: 検証設計（コンセプトテスト/観測指標/ガードレールの運用設計）
- **P5**: レポート（最終出力の形にまとめる）

## 現在の進捗（このコミットでやったこと）

### P1（残ギャップ潰し切り）: 完了

一次情報の追記先はすべて `01_research/sources/` に集約。

- **S1（エンジニアのミカタ）**: `01_research/sources/2026-04-16_tashiro-engineermikata_sources.md`
  - `SalarySystem.html` / `features/` / PRTimes から **83%定義・内訳、平均170万UP主張、伴走の具体（定期ヒアリング/単価交渉/キャリア相談）** を一次追記
  - 算出条件が取れない箇所は **「見当たらず」** を明示
- **S2（キッカケエージェント）**: `01_research/sources/2026-04-16_moro-kikkakeagent_sources.md`
  - **YouTube導線URL**（`https://www.youtube.com/@it_bosatsu_moro`）を確定
  - **LINE登録→面接対策限定動画（9選）限定配布** の一次文言を追記
- **S3（Staneer）**: `01_research/sources/2026-04-16_watanabe-staneer_sources.md`
  - Pitta個別ページから **面談時間45min** を一次追記
  - 公式一次で未確認の **回数/成果物/無料範囲/監修体制** を「未確認」として明示（補助リンクは一次と分離）
- **F2（DYM/景表法）**: `01_research/sources/2026-04-16_failure-dym-job-support_sources.md`
  - 消費者庁PDF（一次）から、**NG表示の骨子＋表示文言例（例: 「就職率驚異の96%!!」）** を引用可能な形で追記
  - ローカル保存: `01_research/sources/caa_representation_cms207_220427_01.pdf`
- **F3（永信国際/許可取消）**: `01_research/sources/2026-04-16_failure-eishin-kokusai-license-revocation_sources.md`
  - 厚労省一次から **取消理由/欠格事由/根拠条文** を抜粋
  - HKZ向けに **情報取扱い・利益相反・守秘・初動Runbook・提供範囲明文化** のガードレール素案へ翻訳して追記

## 次のセッションでやること（すぐ開始できる順）

### 1) P3（分析・統合）を開始

- **勝ちパターン抽出**（`03_analysis/`）
  - S1/S2/S3の一次から、「思想→制度」「透明な見立て」「入口設計」「属人性コントロール」を要素分解してまとめる
- **地雷/ガードレール抽出**（`04_insights/`）
  - F2（表示統制/数値の根拠）とF3（許認可/欠格/コンプラ）を、HKZの対外表現・運用ルールに落とす
- **移植判断**
  - 「HKZに採用する/捨てる（理由つき）」を明文化（P4の検証設計に直結する粒度で）

### 2) P4（検証設計）へ接続

- `04_insights/concept_test_plan.md` を、P1で得た「刺さる約束/根拠/NG表現」で更新
- `05_outputs/report_draft.md` の成功基準を、観測指標（何件でGo寄りか等）に落とす

## 参照

- P1の残ギャップ一覧/次アクションメモ: `01_research/notes/p1_benchmark_gaps_and_actions.md`
