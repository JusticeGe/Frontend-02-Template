[toc]

#学习笔记

## 语言基础
  1. 语言分类
    - 非形式语言
    - 形式语言（乔姆斯基体系）
      - 0型 无限制语法
      - 1型 上下文相关文法
      - 2型 上下文无关文法
      - 3型 正则文法
      > JavaScript大部分是上下文无关文法。但是实际上是上下文相关文法
  2. 产生式（BNF）
    - 用尖括号括起来的名称来表示语法结构名
    - 语法结构分为基础结构和需要用其他语法结构定义的复合结构
      - 基础结构称为终结符
      - 复合结构称为非终结符
    - 引号和中间字符表示终结符
    - 可以有括号
    - `*`表示重复多次
    - `|`表示或
    - `?`表示至少一次
  3. 现代语言分类
    - 形式语言
      - 用途分类
        - 数据描述语言 `JSON`
        - 编程语言
      - 表达方式
        - 声明式语言
        - 命令式语言
  4. 编程语言的性质
    - 图灵完备性（`命令式`）
    - lambda（`函数式`）
    - 动态和静态
      - 动态
        - 在用户设备上运行
        - 产品实际运行时
        - Rumtime
      - 静态
        - 程序员设备
        - 产品开发时
        - Compiletime
      - 类型系统
        - 动态类型系统和静态类型系统
        - 强类型和弱类型
        - 复合类型
          - 结构体
          - 函数签名
        - 子类型
        - 泛型
          - 泛变和形变
  5. 一般式命令式语言设计方式
    - 原子性
    - 表达式
    - 表达式语句

## JavaScript
- `Grammar` 原子
  - `Literal` 字面值
  - `Variable` 变量
  - `keywords` 关键字
  - `whitespace` 空白符
  - `Line Terminator`
- `Runtime` 运行时
  - `Types` 类型
    - `Number`
    - `String`
        - `Character` 字符
        - `Code Point`
        - `Encoding`
    - `Boolean`
    - `Object`
    - `Null`
    - `Undefined`
    - `Symbol`
    - `Bigint` 制定中
  - `Execution Context` 执行上下文

## `Number`
  - `Double Float`
    - `Sign(1)` 符号位
    - `Exponent(11)` 指数位
    - `Fraction(52)` 有效位数
    - 精度丢失
    - `DecimalLiteral` 十进制
      - 前后分别支持小数点
      - 科学计数法
    - `BinaryIntegerLiteral` 二进制
      - `0b`
    - `OctalIntegerLiteral` 八进制
      - `0o`
    - `HexIntegerLiteral` 十六进制
      - `0x`

## `String`
  - `Character`
  - `Code Point` [参考资料](http://www.ruanyifeng.com/blog/2007/10/ascii_unicode_and_utf-8.html)
    - `ASCII` 27个计算机常见字符
    - `Unicode` 编码集
    - `UCS`
    - `GB`
      - `GB2312`
      - `GBK(GB13000)`
      - `GB18030`
    - `ISO-8859`
    - `BIG5`
  - `Encoding`

## 其他类型
> 注： undefined 可以作为变量使用，所以在赋值时最好使用`void 0`

## 对象
- 类
- 对象
- 原型
  - 原型链
    - 相似性
    - `Property`
    - `[[Prototype]]`
    - `原型查找`获取属性的行为
    - 数据属性
    - 访问器属性
    - `Host Object`


