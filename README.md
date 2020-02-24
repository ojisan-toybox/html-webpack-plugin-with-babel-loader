# html-webpack-plugin-with-babel-loader

babel-loader の `exclude: /node_modules/` 設定は必要？

## 現象

Error: /node_modules/react-dom/index.js?:7 　 return extendStatics(d, b);　が起きた

これは html-webpack-plugin を使った時に発現した。

ts-loader に`exclude: /node_modules/`つけると治った。

## 結果

babel-loader, ts-loader 共に`exclude: /node_modules/`なくても問題ない

理由は React 側にあるぽいので別レポジトリで実験する
