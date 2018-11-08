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


### snake case(スネークケース)

単語毎の接続を`_`(アンダーバー)で行う方式  
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

単語毎の接続を`-`(ハイフン)で行う方式  
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

## C lang

宗派が多すぎるためこれがデファクトスタンダードというものでもない  
スネークケースで実装されている場合もかなり多い

### 変数

lowerCamelCase

```c
int totalScore = 0;

char *variableName;
```

### 定数

snake_case & UPPER

```c
int MAX_NAME_LENGTH = 32;

char EXCLUSION_CHAR = 'X';
```

### 関数

lowerCamelCase

```c
int addNumbers(int x, int y) {}

bool isEqualString(char *expected, char *actual) {}
```

### 構造体

UpperCamelCase

```c
struct EnemyCharacter {};
```

## C++ lang

宗派が多すぎるためこれがデファクトスタンダードというものでもない  
スネークケースで実装されている場合もかなり多い

### 変数

Cと同じ

### 定数

Cと同じ

### 関数

Cと同じ

### 構造体

Cと同じ

### クラス

UpperCamelCase

```c
class MagicWarrior {};
```

### メンバ変数

lowerCamelCase

```c
class MagicWarrior {
    int hp = 100;
    int attackPoint = 12;
};
```

宗派によっては`int m_hp`の様に、メンバ変数の先頭に`m_`をつけたりもする。

## Java

### 変数

lowerCamelCase

```java
int totalScore = 0;

String variableName;
```

### 定数

snake_case & UPPER

```java
int MAX_NAME_LENGTH = 32;

char EXCLUSION_CHAR = 'X';
```

### 関数

lowerCamelCase

```java
int addNumbers(int x, int y) {}

boolean isEqualString(char *expected, char *actual) {}
```

### クラス

UpperCamelCase

```java
class MagicWarrior {};
```

## Ruby

### 変数

snake_case & lower

```ruby
total_score = 0

variable_name = 'variable name'
```

### 定数

snake_case & UPPER

```ruby
MAX_NAME_LENGTH = 32

EXCLUSION_CHARS = ['X', 'BUG'].freeze
```

### 関数

snake_case & lower

```ruby
def add_numbers(x, y)
    ...
end

def equal_string?(expected, actual) {}
```

### クラス

UpperCamelCase

```ruby
class MagicWarrior
    ...
end 
```

## Python

### 変数

snake_case & lower

```python
total_score = 0

variable_name = 'variable name'
```

### 定数

snake_case & UPPER

```python
MAX_NAME_LENGTH = 32

EXCLUSION_CHARS = ['X', 'BUG']
```

### 関数

snake_case & lower

```python
def add_numbers(x, y):
    pass

def is_equal_string(expected, actual):
    pass
```

### クラス

UpperCamelCase

```python
class MagicWorrior:
    pass
```

### private変数 & メソッド

前後に`__`(アンダーバー2つ)

```python
class MagicWorrior:
    def __init__(self):
        pass
```

## Go

### 変数

lowerCamelCase

```go
var score int = 0

var pie = 3.14159265358979323846264338

name := "variable name"
```

### 定数

snake_case & UPPER

```go
MAX_NAME_LENGTH := 32

EXCLUSION_CHARS := []string["X", "BUG"]
```

### private関数

lowerCamelCase

```go
func addNum(x, y) int {
    return x + y
}

func isEqualStr(expected, actual) bool { }
```

### public関数

UpperCamelCase

```go
func AddNum(x, y) int {
    return x + y
}

func IsEqualStr(expected, actual) bool { }
```

## Scala

Javaと同じ

## PHP

言語仕様として変数名の先頭に`$`(ドルマーク)が必要  

## JavaScript

C++とかと同じ感じ

## Kotlin

Javaと同じで良いんちゃう？

## C#

Javaと同じで良いんちゃう？

## CSS

とりあえず全小文字のチェーンケースを使えばハズレはない  
特殊なスネークケースと特殊なチェーンケースと通常のスネークケースと通常のチェーンケースが複雑に混ざった記法が結構デファクトスタンダードで定義されていたりもする  

## VB

忘れた

## Shell

???
