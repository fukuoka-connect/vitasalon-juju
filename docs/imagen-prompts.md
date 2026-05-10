# VITA SALON JuJu 素材生成ログ

- 生成日: 2026-05-10
- 対象LP: https://fukuoka-connect.github.io/vitasalon-juju/
- 業種: 痩身エステサロン（医療提携／天神）
- カラーパレット: 生成り `#FBF6F2` × ダスティローズ `#E0B5AC` × モカブラウン `#A07868` × シャンパンゴールド `#C9A876`
- スタイル: ミニマル和洋ミックス／温かみのある高級感／編集系フォト×水彩装飾
- モデル: imagen-4-ultra（※ 2026-05-10時点で MCP の全モデルIDが 404。サーバーアップデート後リトライ要）
- 共通ネガティブ: 黒・赤・人物・テキスト・ロゴ・派手な彩度

## 共通スタイル指示
> Editorial Japanese-European luxury salon. Cream ivory base, dusty rose × mocha brown × champagne gold. No people, no text, no logos. Soft diffused window light. Photorealistic for photos / hand-painted watercolor for decorations. Calm, refined, premium.

---

## 商品・空間（Product / Background）

### 1. hero-01-room.jpg（HERO背景／施術室ムード）
- aspect: `16:9` / format: `image/jpeg` / person_generation: `dont_allow`
- 用途: `.hero` 背景レイヤー（CSSで右側 60% フェード、左に文字載せ）
- prompt:
```
Editorial-quality interior photograph of an upscale Japanese beauty slimming salon treatment room in Tenjin, Fukuoka. Soft cream-ivory walls (#FBF6F2), dusty rose linen (#E0B5AC) draping a single elegant white treatment bed, warm mocha brown wood (#A07868) accents, champagne gold (#C9A876) details on a slim console, a small ceramic vase with one blush rose, a single beeswax candle, sheer linen curtain catching afternoon light. Minimalist Japanese wabi-sabi meets European elegance. No people, no text, no logos. Soft diffused daylight from the right, gentle shadows, shallow depth of field, magazine-style composition with negative space on the left for overlay text. Calm, serene, luxurious, clean, premium spa atmosphere. Photorealistic, 35mm film aesthetic, muted warm tones.
```

### 2. ogp.jpg（OGP）
- aspect: `16:9` / format: `image/jpeg`
- 用途: `og:image` / Twitter card
- prompt:
```
Mood photograph for a luxury medical-affiliated slimming salon brand: a softly lit still-life arrangement on a cream linen surface — one stem of dusty pink rose, a small champagne gold dish, a folded ivory linen towel, a sprig of eucalyptus, soft window light from the upper left. Color palette strictly cream ivory (#FBF6F2), dusty rose (#E0B5AC), mocha brown (#A07868), champagne gold (#C9A876). No people, no text, no logos. Calm, refined, editorial mood, premium Japanese minimalism with European elegance. Photorealistic, soft diffused light, shallow depth of field, ample negative space for typography overlay.
```

### 3. pillar-01-medical.jpg（STRENGTHS 01 SAFETY）
- aspect: `4:3` / format: `image/jpeg`
- 用途: `.s-item:nth-child(1)` 左カラム or 右カラム差し替え
- prompt:
```
Editorial photograph symbolizing medical-beauty partnership: an elegant cream marble desk with a folded crisp white medical coat, a small sleek stethoscope placed neatly, a slender champagne gold pen, a leather-bound ivory notebook, a sprig of dusty pink rose laid beside, soft window light. Color palette cream ivory (#FBF6F2), dusty rose (#E0B5AC), mocha (#A07868), champagne gold (#C9A876). No people, no text, no logos. Premium, trustworthy, calm, refined Japanese clinical-spa aesthetic. Photorealistic, soft diffused daylight, shallow depth of field, ample negative space.
```

### 4. pillar-02-machine.jpg（STRENGTHS 02 MACHINE）
- aspect: `4:3` / format: `image/jpeg`
- 用途: `.s-item:nth-child(2)`
- prompt:
```
Editorial close-up photograph of a professional high-end beauty slimming machine — sleek minimalist white and champagne gold body, smooth curved handpiece resting on a folded ivory linen towel, soft warm window light catching the metallic edge, blurred cream interior in background. No people, no text, no logos. Premium professional aesthetic salon equipment. Color palette cream ivory, dusty rose accent, mocha brown, champagne gold. Photorealistic, magazine-quality product photography, shallow depth of field, refined minimal Japanese composition.
```

### 5. pillar-03-method.jpg（STRENGTHS 03 METHOD）
- aspect: `4:3` / format: `image/jpeg`
- 用途: `.s-item:nth-child(3)`
- prompt:
```
Top-down editorial photograph of a counseling desk: an open ivory linen-bound notebook with a blank page, a slim champagne gold pen, a pair of round wire-rimmed reading glasses, a small porcelain cup of herbal tea with steam, one stem of dusty pink rose laid diagonally, soft cream linen surface, gentle window light from upper-left. Color palette cream ivory (#FBF6F2), dusty rose (#E0B5AC), mocha (#A07868), champagne gold (#C9A876). No people, no text, no logos. Calm, attentive, sincere, premium Japanese editorial mood. Photorealistic, flat-lay knolling composition with breathing space.
```

---

## 装飾（Decorative・透過PNG）

### 6. deco-01-rose.png
- aspect: `1:1` / format: `image/png`
- 用途: `.problem` または `.voice` の浮遊装飾、opacity .15〜.22、回転 -8〜15deg
- prompt:
```
Delicate watercolor illustration of a single dusty rose flower with two soft leaves on a completely transparent background (PNG, no background, alpha channel). Soft hand-painted watercolor washes, blush pink to dusty rose tones (#E0B5AC, #C99A8A), muted mocha brown (#A07868) stem, subtle champagne gold (#C9A876) micro-accents on petal edges. Loose, airy, refined Japanese-European botanical art style. No shadows on the ground, no rectangular background, no text, no border. Minimal, elegant, luxurious decoration suitable for a premium beauty salon website ornamental float element.
```

### 7. deco-02-leaf.png
- aspect: `1:1` / format: `image/png`
- 用途: `.core` または `.cta` の浮遊装飾、opacity .18、回転 -22deg
- prompt:
```
Delicate hand-drawn line-art illustration of a slender botanical leaf branch (single eucalyptus-like sprig, three to five small soft leaves) on a completely transparent background (PNG, no background, alpha channel). Fine champagne gold (#C9A876) lines with subtle mocha brown (#A07868) accents, very thin elegant strokes, hint of watercolor wash in dusty rose. No shadows on the ground, no rectangular background, no text, no border. Refined, airy, luxurious decorative ornament for a premium Japanese beauty salon website.
```

---

## ステータス
| # | ファイル | ステータス |
|---|---|---|
| 1 | hero-01-room.jpg | ✅ 生成済・HEROのbackgroundに右寄せcoverで配置 |
| 2 | ogp.jpg | ✅ 生成済・ルートに複製してog:image反映 |
| 3 | pillar-01-medical.jpg | ✅ 生成済・STRENGTHS 01に配置 |
| 4 | pillar-02-machine.jpg | ✅ 生成済・STRENGTHS 02（左右反転レイアウト）に配置 |
| 5 | pillar-03-method.jpg | ✅ 生成済・STRENGTHS 03に配置 |
| 6 | deco-01-rose.png | ✅ 生成済・PROBLEM右上＆CTA左上に浮遊配置 |
| 7 | deco-02-leaf.png | ✅ 生成済・CTA左下に浮遊配置 |

## 2026-05-10 完了記録
- 旧APIキーが無料プラン側だったため、課金済みアカウントの新キー（`AIzaSyD_QXQiz...`）に差し替え
- `~/.claude.json` の `gemini-imagen` env を更新済み（次回Claude再起動でMCP経由でも生成可能に）
- 今回はMCPサーバー再起動を待たず、curl直叩きで7枚一括生成→保存→組み込み完了

## 既知の問題
- gemini-imagen MCPサーバーがハードコードしているモデルID（`imagen-3.0-generate-002` / `imagen-4.0-generate-preview-06-06` / `imagen-4.0-ultra-generate-preview-06-06`）はGoogle側で全停止しており、現状 404。
- MCPサーバーを最新版（`imagen-4.0-generate-001` 系の安定モデルに対応）に更新後、本ファイルのプロンプトでバッチ再実行すれば即生成完了する想定。

---

## 2026-05-10 リトライ記録（ソラ）
- gemini-imagen-mcp-server の `build/index.js` にハードコードされていた旧モデルIDを安定版にパッチ済み:
  - `imagen-3` → `models/imagen-4.0-fast-generate-001`
  - `imagen-4` → `models/imagen-4.0-generate-001`
  - `imagen-4-ultra` → `models/imagen-4.0-ultra-generate-001`
- Claude Code 再起動でMCPサーバー反映 → 同プロンプトでリトライすれば即生成可能
- 直接curlで叩いた際は無料プラン扱いの404が出たため、有料プラン紐付けキーが環境にあるか要確認
