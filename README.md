# 260611_grid-lanes

ICS MEDIA の記事「CSS だけでメイソンリーレイアウト - `display: grid-lanes`の使い方」のサンプル集です。
Slidev のスライドで作成したデモを、ビルド不要の素の HTML / CSS / JavaScript に移植したものです。

## デモ一覧

| ページ           | 内容                                           | 記事の対応セクション             |
| ---------------- | ---------------------------------------------- | -------------------------------- |
| `index.html`     | デモ集のトップ（対応状況バッジ付き）           | —                                |
| `columns.html`   | CSS Columns の限界（タブ順序が列ごとに縦移動） | CSS Columns の擬似解と、その限界 |
| `waterfall.html` | 最小コード＋幅スライダーでレスポンシブを確認   | Hello Grid Lanes / レスポンシブ  |
| `brick.html`     | waterfall（縦）と brick（横）の切り替え        | 方向の切り替え                   |
| `span.html`      | `grid-column` / `span` / マイナスインデックス  | スパンと明示的配置               |
| `tolerance.html` | `flow-tolerance` をスライダーで変える          | flow-tolerance                   |
| `animejs.html`   | anime.js で追加・並び替え・高さ変更・削除      | JS との連携                      |
| `gsap-flip.html` | GSAP Flip で並び替え遷移                       | JS との連携                      |

## 動作環境

- `display: grid-lanes` は **Safari 26.4 以降**で安定版に対応しています。
- 非対応のブラウザー（Chromium 系・Firefox など）では、各デモが `@supports` によって
  **CSS Columns へフォールバック**し、近似表示になります（本来の挙動は確認できません）。
- 最新の対応状況は [Can I use](https://caniuse.com/mdn-css_properties_display_grid-lanes) を参照してください。

## ローカルで開く

各 HTML は単体で開けます。`animejs.html` と `gsap-flip.html` は CDN から
ライブラリを読み込むため、ネットワーク接続が必要です。

```sh
# 任意の静的サーバーで配信（例）
npx serve .
```

## ライセンス

MIT License
