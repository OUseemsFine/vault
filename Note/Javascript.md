# Grammer：
- use strict: modern mode(class, module auto use strict)
- $, _ can be used as variable name
- const, let (convention: upper letter to stand for const), var(old-fashioned)
- dynamically typed: it meas it supports distinct data type 
- special value: NaN, Infinity
- bigInt: to store big number(not frequently used)
- 在 JavaScript 中，有三种包含字符串的方式: 反引号是 **功能扩展** 引号。它们允许我们通过将变量和表达式包装在 `${…}` 中，来将它们嵌入到字符串中, similar to usage of printf ,可以在 `${…}` 内放置任何东西
- 相比较于其他编程语言，JavaScript 中的 `null` 不是一个“对不存在的 `object` 的引用”或者 “null 指针”。

JavaScript 中的 `null` 仅仅是一个代表“无”、“空”或“值未知”的特殊值。
- 如果一个变量已被声明，但未被赋值，那么它的值就是 `undefined`;
- `typeof` 运算符返回参数的类型。当我们想要分别处理不同类型值的时候，或者想快速进行数据类型检验时，非常有用。
-  `typeof null` 的结果为 `"object"`。这是官方承认的 `typeof` 的错误，这个问题来自于 JavaScript 语言的早期阶段，并为了兼容性而保留了下来。`null` 绝对不是一个 `object`。`null` 有自己的类型，它是一个特殊值。`typeof` 的行为在这里是错误的。
- alert, prompt, confirm 
- typecast: String(), Number(), Boolean()
- a** b is a^b (b can be 1/2)
- 只要任意一个运算元是字符串，那么另一个运算元也将被转化为字符串 1 + '2' = '12'
- + 可作为一元运算符等价于Number()
- 大写的 `"A"` 并不等于小写的 `"a"`。哪一个更大呢？实际上小写的 `"a"` 更大。这是因为在 JavaScript 使用的内部编码表中（Unicode），小写字母的字符索引值更大。
- **严格相等运算符 `===` 在进行比较时不会做任何的类型转换,换句话说，如果 `a` 和 `b` 属于不同的数据类型，那么 `a === b` 不会做任何的类型转换而立刻返回 `false`。**
- 我们为何要研究上述示例？我们需要时刻记得这些古怪的规则吗？不，其实不需要。虽然随着代码写得越来越多，我们对这些规则也都会烂熟于胸，但是我们需要更为可靠的方法来避免潜在的问题：

- 除了严格相等 `===` 外，其他但凡是有 `undefined/null` 参与的比较，我们都需要格外小心。
- 除非你非常清楚自己在做什么，否则永远不要使用 `>= > < <=` 去比较一个可能为 `null/undefined` 的变量。对于取值可能是 `null/undefined` 的变量，请按需要分别检查它的取值情况。
- - 在使用 `>` 或 `<` 进行比较时，需要注意变量可能为 `null/undefined` 的情况。比较好的方法是单独检查变量是否等于 `null/undefined`。
-  空值合并运算符 '??'
- `break <labelName>` 语句跳出循环至标签处
- the para of a function can be function, that is a varName() means function return value
- 在处理完所有函数声明后，代码才被执行: 因此函数声明可以在任何地方
- `let` `func` `=` `(````arg1`,` arg2`,` `...``,` argN````)` `=>` expression`;`
- 如果我们只有一个参数，还可以省略掉参数外的圆括号，使代码更短。
- 




# variable: 

![[Pasted image 20240820093716.png]]

 An arrow function uses `() =>` instead of `function ()`