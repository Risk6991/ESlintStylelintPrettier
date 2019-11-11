# ESlintStylelintPrettier

◎prettier Eslint Stylelint　導入手順

npm list -g --depth=0
グローバルにインストールしたパッケージ一覧を表示
（オプションは階層を示す。これでインストールしたもののみ表示できる）

・Eslintインストール
npm i -D Eslint
・Eslintのinit使って設定ファイルを自動生成
npx (npm bin)/eslint --init

To check syntax, find problems, and enforce code style
commonJS
.js形式
popular　→　JS standerd
※最後に基本設定ほか追加パッケージが素直に自動インストールする

◎ESLint 環境構築　※initコマンドについて解説
https://qiita.com/jobscale/items/eae90308ad885fa2c78c

✗.prettierrc.jsを作成
　→　推奨設定を利用し、変えたいところだけeslintrcの中に書く。
　　　暫定これで。楽だし
（prettierの設定用。eslintrc.***の中に書いても同じ）

◎prettier導入
npm i -D prettier eslint-config-prettier eslint-plugin-prettier

◎共存設定について
https://prettier.io/docs/en/integrating-with-linters.html#eslint

extends　と　parser　に追加記述（RMMプログラミングメモ参照）

ruleにprettierのルールを記載する。
◎prettier公式サイト　オプションについて
https://prettier.io/docs/en/options.html


◎.eslintignore　記述（gitignoreのようなもの）
.vscode
node_modules
out
など。

◎Stylelint導入
npm i -D stylelint stylelint-config-standard stylelint-scss
