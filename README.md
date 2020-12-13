## Css Grid Layout (IE11対応) の解説

###### 目次
1. [GridLayoutとFlexboxの使い分け](#GridLayoutとFlexboxの使い分け)
2. [列と行の指定はgrid-templateを使用](#列と行の指定はgrid-templateを使用)
3. [補足](#補足)

## GridLayoutとFlexboxの使い分け
#### Grid Layout
- 列と行を必要とする多次元レイアウト
- タイル状にコンテンツを並べるようなサイト
- ページ全体で粒度の高いコンポーネントに実装することが多い

#### Flexbox
- 一方向に並べたレイアウト
- ナビゲーションメニューなど、複合コンポーネントのレイアウト調整に最適

## 列と行の指定はgrid-templateを使用
grid-template-columns、grid-template-rowsを使用すると、IEでgrid-gapが上手く効かないため。

## 補足
##### 注意事項
postcss-loaderの設定が変更（ver4.0.0～）
[https://github.com/webpack-contrib/postcss-loader](https://github.com/webpack-contrib/postcss-loader)

##### 参考
[MDN grid-template](https://developer.mozilla.org/ja/docs/Web/CSS/grid-template)
