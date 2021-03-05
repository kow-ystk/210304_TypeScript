# 210304 TS研修

## チュートリアル
https://www.typescriptlang.org/docs/handbook/typescript-tooling-in-5-minutes.html

## tscコマンドが見つからない→パスを通す
https://shimablogs.com/typescript-tsc-command-not-found

## メモ

### constとlet
- varのスコープは「関数」。汚染しやすい。constやletは「ブロック」。
- 再代入と可変は違う。constは上書きできない。ただし、constに定義した配列に値は追加できる。
- 基本的にconst。letによる再代入はロジックが複雑化しやすい。

### 式と文
- 式: 13, 'foo', barという変数, 関数式→これらは変数に代入できる
- 文: ifやforは変数に代入できない
- ブロック文:
{
    console.log("hoge");
    console.log("poge");
}

### 関数
- 関数宣言は巻き上げが起きる function hoge(){}
- 関数式 const hoge= function(){}
- アローファンクションは短くかける&thisを束縛しない
#### thisのコンテキストが変わる場面
- アロー関数以外の関数
- クラス
- オブジェクト
- bind関数

### オブジェクト
- method
- ゲッター、セッター
- const {age, name} = person 分割代入
- オブジェクトのコピーObject.assignとかconst copied = {...hoge}
- オブジェクトのコピーではネストされたオブジェクトはコピーされない shallow copyという(deepにコピーしたいということ自体がまちがい)

## 疑問
- 束縛
- this
- spread {...a}
- class
- promise
- try catch
- async / await


