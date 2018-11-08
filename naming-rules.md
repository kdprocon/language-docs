# 言語毎の命名規則

## 規則名

### lower camel case(ロワーキャメルケース)

先頭小文字で始まり、単語毎に先頭文字を大文字でつなげ、基本小文字の方式  
名称は、文字列がこぶのあるラクダ（キャメル）に見えることからつけられた  

```c
// good
lowerCamelCase

// bad
UpperCamelCase

// bad
snake_case

// bad
SNAKE_CASE

// bad
cain-case

// bad
CAIN-CASE
```


### upper camel case(アッパーキャメルケース)

先頭大文字で始まり、単語毎に先頭文字を大文字でつなげ、基本小文字の方式  
名称は、文字列がこぶのあるラクダ（キャメル）に見えることからつけられた  

```c
// bad
lowerCamelCase

// good
UpperCamelCase

// bad
snake_case

// bad
SNAKE_CASE

// bad
cain-case

// bad
CAIN-CASE
```


### snake case(スネークケース)

単語毎の接続を`_`(アンダーバー)で行う方式  
名称は、文字列がヘビ（スネーク）のように見えることからつけられた  
スネークケースには大小文字の区別を名称に反映していないので実際にこの名称を使うときは気をつける必要がある  

```c
// bad
lowerCamelCase

// bad
UpperCamelCase

// good
snake_case

// good
SNAKE_CASE

// bad
cain-case

// bad
CAIN-CASE
```

### chain case(チェーンケース)

単語毎の接続を`-`(ハイフン)で行う方式  
名称は、文字列が鎖（チェーン）のように見えることからつけられた  
チェーンケースには大小文字の区別を名称に反映していないので実際にこの名称を使うときは気をつける必要がある

```c
// bad
lowerCamelCase

// bad
UpperCamelCase

// bad
snake_case

// bad
SNAKE_CASE

// good
cain-case

// good
CAIN-CASE
```