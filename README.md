# hinui-digitaltwin-v6

島根県邑南町日貫地区のデジタルツイン v6（公開用の単一HTML）。2026-10-18 の踏査を反映した版。

**v5からの変更（2026-10-19）**：入口の先頭に **見る地図**（`view/`・2D・写真のサムネが地図の印・左の一覧・吹き出し・背景6枚）を追加。区画を **A区・B区・前回植樹エリアの3面**に作り直し（B区の西辺・南辺は未実測＝点線）、これまでの仮の枠・間伐区・推定の椿450本・伐採予定域・工事区・苗床の補正案は画面から外した。10/18 の記録 59地点・写真60枚、志賀さんの植栽区境界6点を追加。現地記録は出発前チェックに✗があると最初の「＋記録」で1回だけ注意を出す（止めない）。`wide/` はv5と同じ。v5＝ https://motoki-design.github.io/hinui-digitaltwin-v5/ （凍結・残してある）。

**公開URL： https://motoki-design.github.io/hinui-digitaltwin-v6/**

| | 中身 |
|---|---|
| `view/index.html` | **見る地図**（2D・Leaflet 1.9.4 同梱・EPSG:6671 をそのまま座標に） |
| `record/index.html`＋`sw.js` | **現地記録（2D）**（service worker でオフライン・植樹モード `?mode=plant`） |
| `valley/index.html` | **実験林の谷 0.5 m**（3D・`?x=&y=` でその点へ寄る） |
| `wide/index.html` | **広域 2 m**（v5 と同一バイト） |
| `index.html` | 入口 |

どれも**単一HTML・外部参照ゼロ**。生成元＝作業リポジトリ `hinui-dt-v3`（v6a）の `tools/build_view.py`・`build_record.py`・`build_valley.py`・`make_site_index.py`。
