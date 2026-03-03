# YouTube Analytics HTMLレポート制作タスク

## 目的
「コンサル転職ch (by Strategists)」チャンネルのYouTube分析レポートをHTMLで作成し、GitHub Pages で公開する。

## 参考スタイル
- myvision_reference.html: MyVision競合分析レポートのスタイル参考（日本語、Chart.js使用、ミニマルデザイン）
- consulting_reference.html: コンサル転職ガイドのスタイル参考

## データ
- youtube_report_20260304_0251.txt: テキスト分析レポート
- youtube_videos.csv: 89本の動画データ（再生数、いいね、コメント、duration）
- youtube_analytics_90d.csv: 過去90日の日別データ（再生数、視聴時間、登録者増減等）

## チャンネル基本情報
- チャンネル名: コンサル転職ch (by Strategists)
- 登録者数: 624人
- 総再生数: 69,187回
- 動画本数: 89本
- 過去90日再生数: 22,883回
- 平均視聴率: 35.3%
- 登録者純増(90日): +99人

## 流入元(90日)
- YouTube検索: 14,162回 (62%)
- チャンネル登録者: 3,192回 (14%)
- チャンネルページ: 2,323回 (10%)
- 外部URL: 1,157回 (5%)
- 関連動画: 327回 (1.4%) ← 伸びしろ

## HTMLレポート要件
1. **myvision_reference.htmlと同等以上の品質**（Chart.js使用、日本語、ミニマルデザイン）
2. **含めるセクション:**
   - エグゼクティブサマリー（現状と課題）
   - チャンネル概要（KPI一覧）
   - 月別トレンド推移（Chart.js折れ線グラフ）
   - 流入元分析（Chart.js円グラフ）
   - 上位動画分析（再生数Top10テーブル）
   - 動画投稿頻度と再生数の相関
   - 視聴時間・視聴率分析
   - 競合・業界比較（一般的なYouTube平均値と比較）
   - 具体的な成長戦略提言（優先度付き、5つ以上）
3. **ファイル名:** index.html
4. **GitHubへのpush:**
   - 新規リポジトリ `yyamamoto-alt/strategists-youtube-analysis` を作成
   - `gh repo create yyamamoto-alt/strategists-youtube-analysis --public --description "Strategists YouTube Channel Analysis Report"`
   - index.htmlをpushしてGitHub Pagesを有効化
   - `gh api repos/yyamamoto-alt/strategists-youtube-analysis/pages -X POST -f source='{"branch":"main","path":"/"}'`

## 完了したら
openclaw system event --text "Done: YouTubeチャンネル分析HTMLレポートを作成・GitHub Pages公開完了" --mode now
