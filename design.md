# Anthropic.com Design Document

> 参照元: https://www.anthropic.com/  
> 作成日: 2026-06-20

---

## 1. ブランド概要

Anthropic のホームページは、**シンプル・誠実・高品質** を体現したデザインです。過剰な装飾を排し、落ち着いたアイボリー系のカラーパレットと洗練されたタイポグラフィを組み合わせることで、AI 安全研究企業としての信頼感を表現しています。

---

## 2. カラーパレット

### プライマリカラー

| 名前                    | HEX       | 用途                                         |
| ----------------------- | --------- | -------------------------------------------- |
| Slate Dark (Brand Text) | `#141413` | プライマリテキスト、ボタン背景、フッター背景 |
| Ivory Light             | `#faf9f5` | ページ背景、プライマリボタンテキスト         |
| Ivory Medium            | `#f0eee6` | セカンダリ背景                               |
| Ivory Dark              | `#e8e6dc` | ホバー状態のセカンダリ背景                   |

### セカンダリカラー

| 名前                 | HEX       | 用途                       |
| -------------------- | --------- | -------------------------- |
| Slate Medium         | `#3d3d3a` | ホバー状態のボタン背景     |
| Slate Light          | `#5e5d59` | リンクホバー、サブテキスト |
| Cloud Medium (Agate) | `#b0aea5` | 補助テキスト、薄いテキスト |
| Cloud Light          | `#d1cfc5` | 境界線・区切り線           |
| White                | `#ffffff` | カード背景                 |

### アクセントカラー（ブランドスウォッチ）

| 名前    | HEX       |
| ------- | --------- |
| Accent  | `#c6613f` |
| Clay    | `#d97757` |
| Coral   | `#ebcece` |
| Fig     | `#c46686` |
| Heather | `#cbcadb` |
| Sky     | `#6a9bcc` |
| Cactus  | `#bcd1ca` |
| Olive   | `#788c5d` |
| Kraft   | `#d4a27f` |
| Manilla | `#ebdbbc` |
| Oat     | `#e3dacc` |

### ボーダーカラー

| 名前            | 値          |
| --------------- | ----------- |
| Slate Faded 10% | `#1414131a` |
| Slate Faded 20% | `#14141333` |
| Ivory Faded 10% | `#faf9f51a` |
| Ivory Faded 20% | `#faf9f533` |

---

## 3. タイポグラフィ

### フォントファミリー

| 種類                  | フォント          | フォールバック      |
| --------------------- | ----------------- | ------------------- |
| Display Serif         | `Anthropic Serif` | Georgia, sans-serif |
| Display Sans / Detail | `Anthropic Sans`  | Arial, sans-serif   |
| Monospace             | `Anthropic Mono`  | Arial, sans-serif   |
| 本文 (Paragraph)      | `Anthropic Serif` | Georgia, sans-serif |

### フォントサイズスケール

#### Display（見出し）

| トークン     | サイズ（min → max）     |
| ------------ | ----------------------- |
| display-xxxl | clamp(3.5rem → 6rem)    |
| display-xxl  | clamp(2.75rem → 4.5rem) |
| display-xl   | clamp(2.5rem → 4rem)    |
| display-l    | clamp(2.25rem → 3rem)   |
| display-m    | clamp(1.75rem → 2rem)   |
| display-s    | 1.5rem                  |
| display-xs   | 1.25rem                 |

#### Paragraph（本文）

| トークン     | サイズ   |
| ------------ | -------- |
| paragraph-l  | 1.5rem   |
| paragraph-m  | 1.25rem  |
| paragraph-s  | 1.125rem |
| paragraph-xs | 1rem     |

#### Detail（補助テキスト）

| トークン  | サイズ   |
| --------- | -------- |
| detail-xl | 1.25rem  |
| detail-l  | 1.125rem |
| detail-m  | 1rem     |
| detail-s  | 0.875rem |
| detail-xs | 0.75rem  |

### フォントウェイト

| 種類     | ウェイト |
| -------- | -------- |
| Regular  | 400      |
| Medium   | 500      |
| Semibold | 600      |
| Bold     | 700      |

### ラインハイト

| トークン | 値                    |
| -------- | --------------------- |
| 1        | 1.0                   |
| 1.05     | 1.05                  |
| 1.1      | 1.1                   |
| 1.3      | 1.3                   |
| 1.4      | 1.4（デフォルト本文） |
| 1.5      | 1.5                   |

### レタースペーシング

| トークン | 値                |
| -------- | ----------------- |
| 0em      | 0em（デフォルト） |
| -0.005em | -0.005em          |
| -0.02em  | -0.02em           |

### 実測値（主要要素）

| 要素               | フォント        | サイズ | ウェイト | 行高   |
| ------------------ | --------------- | ------ | -------- | ------ |
| body               | Anthropic Serif | 20px   | 400      | 28px   |
| h1（ヒーロー）     | Anthropic Sans  | ~54px  | 700      | ~59px  |
| h2（フィーチャー） | Anthropic Serif | ~82px  | 400      | ~91px  |
| フッターテキスト   | Anthropic Sans  | 12px   | 400      | 16.8px |

---

## 4. スペーシング

### Space スケール

| トークン | 値                    |
| -------- | --------------------- |
| space-1  | 0.25rem (4px)         |
| space-2  | 0.5rem (8px)          |
| space-3  | 0.75rem (12px)        |
| space-4  | 1rem (16px)           |
| space-5  | 1.5rem (24px)         |
| space-6  | clamp(1.75rem → 2rem) |
| space-7  | clamp(2rem → 2.5rem)  |
| space-8  | clamp(2.25rem → 3rem) |
| space-9  | clamp(2.5rem → 4rem)  |
| space-10 | clamp(3rem → 5rem)    |
| space-11 | clamp(3.5rem → 6rem)  |
| space-12 | clamp(5.5rem → 10rem) |

### Gap スケール

| トークン | 値                    |
| -------- | --------------------- |
| gap-xs   | 0.5rem                |
| gap-s    | 1rem                  |
| gap-m    | 1.5rem                |
| gap-l    | clamp(2.25rem → 3rem) |
| gap-xl   | clamp(2.5rem → 4rem)  |

### Section スペース

| トークン    | 値                    |
| ----------- | --------------------- |
| extra-small | clamp(1.75rem → 2rem) |
| small       | clamp(2.5rem → 4rem)  |
| medium      | clamp(3.5rem → 6rem)  |
| main        | clamp(5.5rem → 10rem) |
| large       | clamp(7rem → 14rem)   |
| page-top    | clamp(6rem → 12rem)   |

---

## 5. グリッドシステム

- **カラム数**: 12カラム
- **最大幅**: 89.5rem (1432px)
- **サイドマージン**: clamp(2rem → 5rem)（両端）
- **ガター**: clamp(1.75rem → 2rem)（カラム間）
- **コンテナ (main)**: `min(89.5rem, 100vw) - margin × 2`
- **コンテナ (small)**: 12カラムのうち8カラム分

---

## 6. ボーダー・シェイプ

| プロパティ   | 値                |
| ------------ | ----------------- |
| border-width | 0.0625rem (1px)   |
| radius-small | 0.25rem (4px)     |
| radius-main  | 0.5rem (8px)      |
| radius-large | 1rem (16px)       |
| radius-round | 100vw（ピル形状） |

---

## 7. ナビゲーション

| プロパティ         | 値      |
| ------------------ | ------- |
| ナビ高さ           | 4.25rem |
| バナー高さ         | 2.75rem |
| ドロップダウン遷移 | 200ms   |
| メニュー開閉       | 400ms   |

- スタイル: 透明背景（ページ背景と一体化）
- ロゴ: Anthropic "AV" モノグラム（左上）
- メニュー: ハンバーガー（モバイル右上） / テキストリンク（デスクトップ）
- 文字色: `#141413`

---

## 8. ボタン

### Primary

| プロパティ | 値        |
| ---------- | --------- |
| 背景色     | `#141413` |
| テキスト色 | `#faf9f5` |
| ホバー背景 | `#3d3d3a` |
| 境界線     | `#141413` |

### Secondary

| プロパティ     | 値          |
| -------------- | ----------- |
| 背景色         | transparent |
| テキスト色     | `#141413`   |
| ホバー背景     | `#141413`   |
| ホバーテキスト | `#faf9f5`   |
| 境界線         | `#141413`   |

### Tertiary

| プロパティ   | 値                         |
| ------------ | -------------------------- |
| 背景色       | transparent                |
| テキスト色   | `#141413`                  |
| 境界線       | `#1414131a`（10% opacity） |
| ホバー境界線 | `#141413`                  |

---

## 9. コンポーネント

### ヒーローセクション
- 背景: `#faf9f5`
- 大見出し: Anthropic Sans / Bold / display-xxl / `#141413`
- インラインリンク: 下線付き
- サブコピー: Anthropic Serif / Regular / 本文サイズ

### フィーチャーカード（Latest Releases）
- 背景: `#f0eee6`（Ivory Medium）
- 角丸: 1rem
- レイアウト: 3カラムグリッド
- 見出し: Anthropic Sans / Bold
- 本文: Anthropic Serif / Regular
- メタ情報: Anthropic Sans / 小サイズ / 大文字（uppercase）

### 記事リスト（Featured articles）
- レイアウト: テーブル状の行リスト
- 境界線: 下ボーダー `#1414131a`
- 見出しとカテゴリを左右に配置

### フッター
- 背景: `#141413`
- テキスト: `#faf9f5`
- フォント: Anthropic Sans
- レイアウト: 4カラムグリッド（Products / Solutions / Resources / Company）
- SNSアイコン: LinkedIn / X / YouTube

---

## 10. モーション・インタラクション

| プロパティ         | 値                    |
| ------------------ | --------------------- |
| ドロップダウン遷移 | 200ms                 |
| メニュー開閉       | 400ms                 |
| リンクホバー色     | `#141413` → `#5e5d59` |

---

## 11. アクセシビリティ

| プロパティ                   | 値                                             |
| ---------------------------- | ---------------------------------------------- |
| フォーカスボーダー幅         | 0.125rem                                       |
| フォーカスオフセット（外側） | 0.25rem                                        |
| フォーカスオフセット（内側） | -0.125rem                                      |
| スキップリンク               | "Skip to main content" / "Skip to footer" あり |

---

## 12. レスポンシブデザイン

すべての主要サイズは `clamp()` によるフルイドタイポグラフィ・スペーシングを採用しています。

| ブレークポイント | 対応                                    |
| ---------------- | --------------------------------------- |
| モバイル         | ハンバーガーメニュー、1カラムレイアウト |
| タブレット       | グリッド縮小、フォントサイズ流動変化    |
| デスクトップ     | 12カラムフルグリッド、最大幅 1432px     |