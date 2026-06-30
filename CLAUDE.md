# AI活用ポートフォリオLP 制作ルール

> コピーして `ccc-workspace/1_projects/ai-portfolio-lp/CLAUDE.md` として配置する。`プロジェクト名` だけ自分用に書き換える。

## プロジェクト
- プロジェクト名：とうまろのAI活用ポートフォリオLP
- フォルダ名：ai-portfolio-lp
- 公開方針：GitHub Public / Vercel Public

## 目的
このプロジェクトでは、自分のプロフィール、AI活用テーマ、作ったもの、これから作りたいものをまとめる1枚のLPを作り、GitHubとVercelで公開する。

## 親ルール
親フォルダの `CLAUDE.md` にあるPAC原則・安全ルール・検証ルールを前提にする。このファイルではLP制作固有の制約だけを追加する。

## 制作制約
- まずMVPとして小さく作る
- 単一の `index.html` で作る
- Tailwind CDNを使う
- Node.js、npm、Astro、Next.js、Vite、localhost、開発サーバーは使わない
- `index.html` をブラウザで直接開いて確認する
- 画像なしでも完成する構成にする
- 画像、ロゴ、スクショを使う場合は `assets/` に置く
- 初期セットアップ時に `assets/` と `_archive/` がなければ作る

## 作業の流れ
- `profile.md`：LPに載せる自分の情報
- `lp-plan.md`：LPの設計図
- `index.html`：LP本体
- まず質問に答えて `profile.md` を作る
- 次にPlan Modeで `lp-plan.md` を作る
- その後、`profile.md` と `lp-plan.md` を元に `index.html` を作る
- Claudeは提案者。最終決定は人間が行う

## 修正方針
- 内容が違う場合は `profile.md` に戻る
- 構成が違う場合は `lp-plan.md` に戻る
- 見た目が違う場合は、内容と構成を変えずに見た目だけ改善する
- 表示崩れは `index.html` を修正する

## frontend-designを使うとき
`frontend-design` を使うときは、掲載内容・セクション構成・CTA・リンク・技術方針を変えず、余白・配色・タイポグラフィ・カードUI・レスポンシブ・軽いhover表現だけを改善する。単一HTML + Tailwind CDNを維持する。

## GitHub公開
GitHubはPublicリポジトリを標準にする。
含める：`CLAUDE.md`、`index.html`、`README.md`、`assets/`（中身がある場合）
含めない：`profile.md`、`lp-plan.md`、`_archive/`
push前に公開されるファイル一覧を必ず確認する。

## 完了条件
- `index.html` がブラウザで表示できる
- スマホ幅でも大きく崩れない
- 公開してはいけない個人メモや秘密情報が含まれていない
- GitHub Publicリポジトリに保存できている
- Vercel公開URLができている
