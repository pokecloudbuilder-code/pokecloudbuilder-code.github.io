# AdSense Content Plan

この手順書は、`https://www.pokecloudbuilder.com/` の自ドメイン内コンテンツを増やし、AdSense申請前のサイト品質を高めるための作業メモです。

目的は、単にページ数を増やすことではなく、訪問者と審査クローラーのどちらにも「このサイトには独自の有用な情報がある」と伝わる状態にすることです。

## 前提

- 事業サイト: `https://www.pokecloudbuilder.com/`
- リポジトリ: `pokecloudbuilder-code/pokecloudbuilder-code.github.io`
- 公開済みプロダクト:
  - Jam Blocks: `https://jam.pokecloudbuilder.com/`
  - 立体視メーカー: `https://rittai.pokecloudbuilder.com/`
  - 年齢・学年・和暦チェッカー: `https://nenrei.pokecloudbuilder.com/`
  - かのうさルーレット: `https://kanousa.pokecloudbuilder.com/`
- 開発中/準備中:
  - Scientific Calculator
- 既存ページ:
  - `index.html`
  - `contact.html`
  - `privacy-policy.html`
  - `sitemap.xml`
  - `robots.txt`

## 作業方針

- 自ドメイン内に、アプリ紹介・使い方・開発背景のページを追加する。
- Zenn記事の丸写しは避け、事業サイト側は短めで読みやすい紹介文にする。
- 各ページから対象アプリ、問い合わせ、関連するZenn記事へ自然にリンクする。
- アプリごとに「何ができるか」「誰向けか」「データの扱い」「使い方」を明記する。
- 公開済みアプリは「公開中」、未公開アプリは「公開準備中」と表現する。
- AdSense申請前は、広告コードを過剰に置かず、まずコンテンツ品質を優先する。

## 推奨ページ構成

### 1. Jam Blocks紹介ページ

ファイル案: `apps/jam-blocks.html`

優先度: 高

目的:

- Jam Blocksの概要を自ドメイン内でも説明する。
- 音楽練習用アプリとしての独自性を示す。
- Zenn記事だけに説明を依存しない状態にする。

入れる内容:

- Jam Blocksとは
- 一人練習で困ること
- できること
  - BPM設定
  - ドラムパターン
  - コード進行
  - ベース伴奏
  - ギター伴奏
  - ローカル保存
  - PWA
- データの扱い
  - 譜面データはブラウザ内に保存
  - サーバーへ自動送信しない
- 対象ユーザー
  - ギター/ベース/ドラムの個人練習
  - バンド練習前の下準備
  - コード進行に合わせて遊びたい人
- リンク
  - アプリを開く
  - 開発記事を読む
  - お問い合わせ

本文量目安:

- 800〜1,500文字程度

### 2. Jam Blocks使い方ページ

ファイル案: `guides/jam-blocks-how-to.html`

優先度: 高

目的:

- 実際に使う人向けの手順を提供する。
- 自ドメイン内の実用コンテンツを増やす。

入れる内容:

- 1. BPMを決める
- 2. ドラムパターンを選ぶ
- 3. コード進行を作る
- 4. ベース/ギターのパターンを選ぶ
- 5. ループ再生する
- 6. 保存する
- 7. JSONでバックアップする
- よくある質問
  - 音が鳴らない場合
  - 保存データはどこにあるか
  - スマホで使えるか
  - オフラインで使えるか

本文量目安:

- 1,200〜2,000文字程度

### 3. Jam Blocks開発メモページ

ファイル案: `notes/jam-blocks-webaudio.html`

優先度: 中

目的:

- 技術的な独自コンテンツを自ドメインにも置く。
- Zenn記事への導線を作る。

入れる内容:

- Web Audio APIで音を鳴らしていること
- `AudioContext.currentTime` とLook-ahead方式の簡単な説明
- なぜ外部音源を使わなかったか
- Alpha版で割り切ったこと
- 詳細はZenn記事へ誘導

本文量目安:

- 800〜1,500文字程度

### 4. 各既存アプリの紹介ページ

ファイル案:

- `apps/rittai.html`
- `apps/nenrei.html`
- `apps/kanousa.html`

優先度: 中

目的:

- 事業サイトのトップページだけでなく、各アプリごとの説明ページを用意する。
- 検索流入とAdSense審査上のコンテンツ量を補う。

各ページに入れる内容:

- アプリ概要
- 主な機能
- 使い方
- 利用シーン
- データの扱い
- アプリリンク
- 関連Zenn記事リンク
- お問い合わせリンク

本文量目安:

- 各800〜1,500文字程度

### 5. 開発ログ一覧ページ

ファイル案: `articles.html`

優先度: 中

目的:

- Zenn記事へのリンクを整理する。
- サイト全体として継続的に開発している印象を出す。

入れる内容:

- Jam Blocks記事
- 立体視メーカー記事
- 年齢・学年・和暦チェッカー記事
- かのうさルーレット記事
- Google Play準備記事

注意:

- 外部リンク集だけにしない。
- 各記事について、事業サイト側にも2〜3文の紹介文を添える。

### 6. サイト運営についてページ

ファイル案: `about.html`

優先度: 低〜中

目的:

- 誰が、どんな方針でアプリを作っているかを説明する。
- 事業サイトとしての信頼感を高める。

入れる内容:

- pokecloudbuilderについて
- 作っているもの
- 開発方針
- 個人情報や問い合わせへの考え方
- 事業者情報ページへのリンク

本文量目安:

- 600〜1,200文字程度

## 実装順

### Step 1: ディレクトリを作る

```bash
mkdir -p apps guides notes
```

作成予定:

- `apps/jam-blocks.html`
- `guides/jam-blocks-how-to.html`
- `notes/jam-blocks-webaudio.html`

### Step 2: 共通ナビゲーションを更新する

既存の `index.html`、`contact.html`、`privacy-policy.html` のヘッダーに、必要に応じて以下を追加する。

- `アプリ`
- `開発ログ`
- `お問い合わせ`

ただし、ナビゲーションが窮屈になる場合はトップページからの内部リンクを優先する。

### Step 3: Jam Blocks関連3ページを追加する

優先して作るページ:

1. `apps/jam-blocks.html`
2. `guides/jam-blocks-how-to.html`
3. `notes/jam-blocks-webaudio.html`

この3ページがあると、Jam Blocksが単なる外部アプリリンクではなく、自ドメイン内でも十分に説明されたプロダクトになる。

### Step 4: トップページから内部リンクする

`index.html` のJam Blocksカードに以下のリンクを追加する。

- アプリを開く
- 使い方を見る
- 開発メモを見る
- 開発記事を読む

外部リンクだけでなく、自ドメイン内ページへのリンクを必ず含める。

### Step 5: sitemap.xmlを更新する

新規ページを追加したら、必ず `sitemap.xml` に追加する。

追加例:

```xml
<url>
  <loc>https://www.pokecloudbuilder.com/apps/jam-blocks.html</loc>
</url>
<url>
  <loc>https://www.pokecloudbuilder.com/guides/jam-blocks-how-to.html</loc>
</url>
<url>
  <loc>https://www.pokecloudbuilder.com/notes/jam-blocks-webaudio.html</loc>
</url>
```

### Step 6: privacy-policy.htmlを確認する

確認項目:

- Jam Blocksが対象サービスに含まれている
- ブラウザ内保存データについて説明している
- お問い合わせフォームへの導線がある
- 第三者サービス利用の説明が実態と合っている

### Step 7: contact.htmlを確認する

確認項目:

- 対象アプリにJam Blocksがある
- 問い合わせ先が機能している
- 事業者情報が古くない

### Step 8: ローカル確認

簡易サーバーで確認する。

```bash
python3 -m http.server 8080
```

確認URL:

- `http://localhost:8080/`
- `http://localhost:8080/apps/jam-blocks.html`
- `http://localhost:8080/guides/jam-blocks-how-to.html`
- `http://localhost:8080/notes/jam-blocks-webaudio.html`
- `http://localhost:8080/privacy-policy.html`
- `http://localhost:8080/contact.html`
- `http://localhost:8080/sitemap.xml`

### Step 9: コミットしてプッシュ

```bash
git status --short
git add .
git commit -m "Add Jam Blocks content pages"
git push
```

GitHub Pages反映後、公開URLで確認する。

## AdSense申請前チェックリスト

- [ ] トップページに公開中プロダクトが自然に並んでいる
- [ ] Jam Blocksの紹介ページがある
- [ ] Jam Blocksの使い方ページがある
- [ ] Jam Blocksの技術/開発メモページがある
- [ ] 既存アプリの紹介ページが少なくとも1〜3本ある
- [ ] プライバシーポリシーが実態に合っている
- [ ] お問い合わせフォームが動作する
- [ ] `sitemap.xml` に新規ページが入っている
- [ ] `robots.txt` が `sitemap.xml` を指している
- [ ] 各ページに独自の本文がある
- [ ] 外部リンク集だけのページになっていない
- [ ] 404リンクがない
- [ ] スマホ幅で本文が読める
- [ ] 広告コードを置く場合、本文より広告が目立ちすぎていない

## 申請タイミングの目安

最低限:

- Jam Blocks紹介ページ
- Jam Blocks使い方ページ
- プライバシーポリシー更新
- お問い合わせフォーム
- sitemap更新

推奨:

- Jam Blocks関連3ページ
- 既存アプリ紹介ページ2〜3本
- 開発ログ一覧ページ
- aboutページ

この推奨状態まで作ってから申請したほうが、コンテンツ不足で落ちるリスクを下げやすい。

## 注意

AdSense審査は明確な合否基準が公開されているわけではありません。ページ数だけでなく、独自性、読みやすさ、サイトの信頼性、ポリシー準拠が見られる前提で整備します。
