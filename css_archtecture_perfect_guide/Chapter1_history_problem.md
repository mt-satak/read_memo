## CSSのはじまり

案外古い（1994提唱）

### 役割・目的
HTMLやXML要素の装飾
文書の構造(HTML)と、スタイル(CSS)で棲み分けることが目的



## CSSの問題点

ページ数が増えるとCSSもどんどん複雑化してしまう、管理しきれなくなる
→カオス！
スタイリングの規則をきちんと決めてそれを守ってコーディングすることが大事
それも複数人で開発して行くとなると難しい、
→どうしてこうなった

### CSSはすべてがグローバルスコープ
＝すべてのスタイリングが鑑賞し合う可能性がある状態



## 複雑化するWEB開発

当初提唱された使い方からはだいぶ変わってきてしまった
文書の編集だけでなくアニメーションやユーザ操作に合わせた動的な表示処理など。
今日ではいちいち手作業でHTMLを用意することはほとんどなく、
CMSなどを通してページすることが多い

### 変更不可能なHTML/CSSと向き合う
CMSが吐き出すHTML/CSSを利用せざるを得ない局面も
→自分が書いたCSSとCMSが作ったHTML/CSSでうまく折り合いをつける必要がある

### 増加するページ数
数十・数百ページのWEBサイトを作るとなると、事前にきちんと設計しないと
想定外のCSS衝突やどこに何が書いてあるか分からない状態が起きてしまう

CSS is too fragile.

### 頻繁に変更される「状態」
ユーザ操作によって要素が動的に切り替わる場合も多々あり

### 解決策としてのCSS設計
個人・各社でオレオレCSSでルールを決めてやることもあるけどやはり管理が大変
大抵うまくいかない

OOCSS, BEM, など設計手法がいろいろある
絶対的なベストプラクティスは存在しないが、
・抽象化する
・分ける
この２つは共通して大事

### アトミックデザインの話
元々はデザインシステム構築・UIの思想・指針

・Atoms　原子（もっとも小さなパーツ）
・Molecules　分子
・Organisms　有機体
・Templates　テンプレート
・Pages　ページ（上記を結合した構造物）
の５つに分けて再整理する

アトミックデザインの思想に慣れることで「抽象思考」が身につく