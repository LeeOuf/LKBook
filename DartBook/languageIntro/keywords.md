# 关键字

下表为 Dart 语言的关键字。

| abstract 1 | continue   | false        | new        | this      |
| ---------- | ---------- | ------------ | ---------- | --------- |
| as 1       | default    | final        | null       | throw     |
| assert     | deferred 1 | finally      | operator 1 | true      |
| async 2    | do         | for          | part 1     | try       |
| async* 2   | dynamic 1  | get 1        | rethrow    | typedef 1 |
| await 2    | else       | if           | return     | var       |
| break      | enum       | implements 1 | set 1      | void      |
| case       | export 1   | import 1     | static 1   | while     |
| catch      | external 1 | in           | super      | with      |
| class      | extends    | is           | switch     | yield 2   |
| const      | factory 1  | library 1    | sync* 2    | yield* 2  |

1 带有上标 **1** 的关键字是 *内置关键字*。避免把内置关键字当做标识符使用。 也不要把内置关键字 用作类名字和类型名字。 有些内置关键字是为了方便把 JavaScript 代码移植到 Dart 而存在的。 例如，如果 JavaScript 代码中有个变量的名字为 `factory`， 在移植到 Dart 中的时候，你不必重新命名这个变量。

2 带有上标 **2** 的关键字，是在 Dart 1.0 发布以后又新加的，用于 支持异步相关的特性。 你不能在标记为 `async`、 `async*`、或者 `sync*` 的方法体内 使用 `async`、 `await`、或者 `yield` 作为标识符。 

所以其他单词都是 *保留词*。 你不能用保留词作为关键字。

