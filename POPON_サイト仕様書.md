# POPON ベビーマッサージ教室 ウェブサイト仕様書

## 基本情報

### サイト概要
- **サイト名**: POPON 姫路 ベビーマッサージ教室
- **目的**: 姫路市でのベビーマッサージ教室の集客・情報提供
- **対象**: 赤ちゃんとママ（0歳〜1歳程度）
- **地域**: 兵庫県姫路市（JR東姫路駅徒歩5分）

### 講師情報
- **講師名**: 田中紗理
- **教室名**: POPON
- **住所**: 兵庫県姫路市市之郷町
- **アクセス**: JR東姫路駅から徒歩5分、ホームセンターナフコ横、駐車場1台あり

---

## デプロイ・リポジトリ情報

### GitHub リポジトリ
- **リポジトリ名**: `popon-baby-massage`
- **URL**: https://github.com/higejori/popon-baby-massage
- **ブランチ**: `main`
- **所有者**: higejori

### Netlify デプロイ
- **サイトURL**: https://animated-haupia-9c5ff9.netlify.app
- **デプロイ方法**: GitHub連携による自動デプロイ
- **デプロイトリガー**: mainブランチへのプッシュ

---

## ファイル構成

```
C:\Claude code\08_POPONベビーマッサージ教室サイト\
├── POPON_サイト仕様書.md    # この仕様書
├── README.md                 # 簡易説明書
├── .git/                     # Gitリポジトリ管理ファイル
├── docs/                     # ドキュメントフォルダ
├── images/                   # 元画像フォルダ（参考用）
└── src/                      # 公開ファイル（Netlifyが参照）
    ├── index.html            # メインHTMLファイル
    ├── styles.css            # メインCSSファイル
    ├── robots.txt            # SEO用クローラー制御
    └── images/               # 画像フォルダ
        ├── POPON ロゴ.png    # ロゴ画像
        ├── メインビジュアル.JPG  # トップ画像
        ├── 田中紗理.JPEG      # 講師写真
        ├── ベビーマッサージの効果.JPEG
        ├── ベビーオイル.JPEG
        ├── マップ.png         # アクセスマップ
        ├── 現金.jpeg          # 支払い方法アイコン
        ├── ameba(ブログ).JPEG # ブログアイコン
        ├── line.JPEG          # LINE連絡アイコン
        ├── insta.JPEG         # Instagramアイコン
        ├── ベビーマッサージ コース内容.jpg
        ├── おくるみタッチケア コース内容.jpg
        ├── ハート.jpg         # 特徴アイコン
        ├── 花1.jpg           # 特徴アイコン
        ├── アクセス.jpg       # 特徴アイコン
        └── （その他装飾用画像）
```

---

## サイト構成・セクション詳細

### 1. ヘッダー
- **ロゴ**: POPON ロゴ.png
- **タイトル**: "POPON ~姫路 ベビーマッサージ教室~"
- **ナビゲーション**: 
  - ベビーマッサージとは
  - コース紹介
  - 講師紹介
  - ブログ
  - アクセス
  - お問い合わせ

**モバイル対応**: ハンバーガーメニュー（右上3本線）で折りたたみ表示

### 2. メインビジュアル
- **背景画像**: メインビジュアル.JPG
- **タイトル**: "POPON"
- **サブタイトル**: "~姫路 ベビーマッサージ教室~"
- **メッセージ**: "笑顔あふれる育児をしよう"
- **ボタン**: 
  - "お問い合わせ" (プライマリ)
  - "コースを見る" (セカンダリ)

### 3. POPONの特徴
- **セクションタイトル**: "POPONってどんなところ？"
- **3つの特徴**:
  1. **笑顔あふれる** (ハート.jpg)
  2. **落ち着いた空間** (花1.jpg)
  3. **アクセス良好** (アクセス.jpg)

### 4. ベビーマッサージとは
- **メインタイトル**: "赤ちゃんとママの絆を深める特別な時間"
- **効果リスト**: 5つの効果をアイコン付きで表示
- **オイル情報**: "赤ちゃんにやさしいオイルを使用" (ベビーオイル.JPEG)
- **効果画像**: ベビーマッサージの効果.JPEG

### 5. コース紹介
- **コース画像**: 
  - ベビーマッサージ コース内容.jpg
  - おくるみタッチケア コース内容.jpg
- **支払い方法**: 現金のみ (現金.jpeg)

### 6. 講師紹介
- **講師写真**: 田中紗理.JPEG
- **講師名**: 田中 紗理
- **メッセージ**: ママと赤ちゃんへの温かいメッセージ

### 7. アクセス
- **教室名**: POPON ベビーマッサージ教室
- **住所**: 兵庫県姫路市市之郷町
- **アクセス**: JR東姫路駅から徒歩5分
- **目印**: ホームセンターナフコ横
- **駐車場**: 1台あり
- **地図**: マップ.png

### 8. ブログ
- **タイトル**: "日々の様子をお届けしています"
- **ブログアイコン**: ameba(ブログ).JPEG
- **リンク**: https://ameblo.jp/tnk-babu/

### 9. お問い合わせ
- **LINE**: https://line.me/R/ti/p/@373naeod?oat_content=url&ts=06261348
- **Instagram**: https://www.instagram.com/popon_babu/

---

## 技術仕様

### HTML
- **ファイル**: `src/index.html`
- **構造**: HTML5セマンティック要素を使用
- **SEO対応**: 
  - metaタグ（description, keywords）
  - Open Graph対応
  - 構造化データ（JSON-LD）
- **レスポンシブ**: viewport meta設定済み

### CSS
- **ファイル**: `src/styles.css`
- **レスポンシブ**: 
  - デスクトップ: 1200px max-width
  - タブレット: 768px以下
  - モバイル: 480px以下
- **カラーテーマ**: オレンジ系（#ff8c42, #e67a3a）
- **フォント**: 日本語フォント（Hiragino Kaku Gothic ProN, メイリオ等）

### JavaScript
- **機能**: ハンバーガーメニューの開閉
- **関数**: 
  - `toggleMenu()`: メニュー開閉
  - `closeMenu()`: メニューを閉じる

### 画像最適化
- **preload**: ロゴとメインビジュアル
- **lazy loading**: その他の画像
- **content-visibility**: パフォーマンス最適化

---

## 更新・修正手順

### 1. ローカルでの修正
1. ファイルを編集（src/index.html または src/styles.css）
2. ブラウザでローカル確認

### 2. 変更をコミット
```bash
# プロジェクトフォルダに移動
cd "C:\Claude code\08_POPONベビーマッサージ教室サイト"

# 変更をステージング
git add .

# コミット（メッセージは変更内容を明記）
git commit -m "修正内容を具体的に記述

🤖 Generated with [Claude Code](https://claude.ai/code)

Co-Authored-By: Claude <noreply@anthropic.com>"
```

### 3. GitHubにプッシュ
```bash
# リモートリポジトリにプッシュ
git push
```

### 4. 自動デプロイ確認
- プッシュ後、NetlifyがGitHubから自動的にデプロイ
- 通常1-2分で https://animated-haupia-9c5ff9.netlify.app に反映
- Netlifyの管理画面: https://app.netlify.com/

---

## よく修正する項目と方法

### テキスト修正
**ファイル**: `src/index.html`

1. **ヘッダータイトル** (行59-60)
```html
<h1>POPON</h1>
<p>~姫路 ベビーマッサージ教室~</p>
```

2. **メインビジュアルのメッセージ** (行90)
```html
<h2 class="hero-message">笑顔あふれる育児をしよう</h2>
```

3. **講師からのメッセージ** (行203-208)
```html
<p>はじめまして、POPONの田中紗理です。</p>
<!-- 以下のメッセージを修正 -->
```

### スタイル修正
**ファイル**: `src/styles.css`

1. **色の変更**
```css
/* メインカラー */
--primary-color: #ff8c42;
--secondary-color: #e67a3a;
```

2. **フォントサイズ調整**
```css
/* デスクトップ */
.hero-title { font-size: 4rem; }
.hero-message { font-size: 1.4rem; }

/* モバイル */
@media (max-width: 768px) {
    .hero-message { font-size: 1rem !important; }
}
```

### 画像の差し替え
1. `src/images/`フォルダに新しい画像を配置
2. HTMLファイルで画像パスを変更
```html
<img src="images/新しい画像.jpg" alt="説明">
```

---

## 修正時の注意点

### スマホ対応
- **768px以下**と**480px以下**の両方のメディアクエリを確認
- ハンバーガーメニューの動作確認
- フォントサイズと余白の調整

### 画像関連
- images/ フォルダ内の画像は相対パス `images/ファイル名` で参照
- 新しい画像を追加する場合は src/images/ に配置
- ファイル名に日本語が含まれる場合は注意

### CSS特異性
- 重要な変更には `!important` を使用する場合あり
- モバイル用の設定は `.nav-menu` 系のセレクタを使用
- 特にナビゲーション関連は `.nav ul.nav-menu` で上書き

### SEO更新
- タイトルや説明文を変更する場合は、HTMLのmetaタグも更新
- 構造化データ（JSON-LD）の更新も検討

---

## トラブルシューティング

### よくある問題と解決方法

#### 1. 画像が表示されない
**原因**: 
- ファイルパスの間違い
- 画像ファイルが存在しない

**解決方法**:
```bash
# src/images/ フォルダに画像があるか確認
ls "C:\Claude code\08_POPONベビーマッサージ教室サイト\src\images"

# HTMLファイルのパスを確認
# ✓ 正しい: src="images/ファイル名.jpg"
# ✗ 間違い: src="../images/ファイル名.jpg"
```

#### 2. スマホでナビゲーションが透明
**原因**: CSS特異性の問題

**解決方法**:
```css
/* styles.cssで確認 */
.nav ul.nav-menu {
    background: #ffffff !important;
    backdrop-filter: none !important;
}
```

#### 3. デプロイされない
**解決手順**:
1. GitHubにプッシュされているか確認
```bash
git status
git log --oneline -3
```

2. Netlifyの管理画面でビルドログを確認
3. 必要に応じて手動デプロイ

#### 4. レイアウトが崩れる
**確認項目**:
- メディアクエリの設定
- CSS特異性の問題
- 新しいCSSが既存のスタイルと競合していないか

**解決方法**:
```css
/* 重要な変更には!importantを使用 */
.important-style {
    property: value !important;
}
```

### 緊急時の対応
```bash
# 直前のコミットに戻す
cd "C:\Claude code\08_POPONベビーマッサージ教室サイト"
git reset --hard HEAD~1
git push --force

# 特定のコミットに戻す
git log --oneline -10  # コミット履歴を確認
git reset --hard [コミットID]
git push --force
```

---

## 開発・デプロイフロー

### 通常の更新フロー
1. **要望確認** → 修正内容の整理
2. **ローカル修正** → ファイル編集
3. **動作確認** → ブラウザでテスト
4. **コミット** → git add & commit
5. **プッシュ** → git push
6. **デプロイ確認** → 本番サイトで確認

### 大きな変更時
1. **バックアップ** → 現在のコミットIDを記録
2. **段階的修正** → 小さな変更に分けて実装
3. **テスト** → 各段階で動作確認
4. **段階的コミット** → 機能ごとにコミット

---

## 参考情報・外部リンク

### サイト関連
- **本番サイト**: https://animated-haupia-9c5ff9.netlify.app
- **GitHub**: https://github.com/higejori/popon-baby-massage
- **Netlify管理画面**: https://app.netlify.com/

### 連絡先
- **LINE**: https://line.me/R/ti/p/@373naeod?oat_content=url&ts=06261348
- **Instagram**: https://www.instagram.com/popon_babu/
- **ブログ**: https://ameblo.jp/tnk-babu/

### 技術参考
- **HTML5**: https://developer.mozilla.org/ja/docs/Web/HTML
- **CSS3**: https://developer.mozilla.org/ja/docs/Web/CSS
- **Git**: https://git-scm.com/doc

---

## 更新履歴

### 2025年1月16日 - v1.0
- **初版完成**: サイト全体のデザイン・機能実装完了
- **主要機能**: 
  - レスポンシブデザイン
  - ハンバーガーメニュー
  - SEO対応
  - 画像最適化
- **デプロイ**: Netlify自動デプロイ設定完了

### 主要な修正履歴
- ヘッダー・メインビジュアル: 「姫路」追加
- メインビジュアル: 行間・フォントサイズ調整
- POPONの特徴: セクションタイトル追加
- ベビーマッサージとは: オイル説明簡略化
- ブログ: ボタン横幅調整
- 全体: スマホ表示最適化

---

**最終更新**: 2025年1月16日  
**作成者**: Claude Code  
**バージョン**: 1.0