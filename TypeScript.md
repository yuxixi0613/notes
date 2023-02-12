# 环境

### 1.下载Node.js

### 2.安装Node.js

傻瓜式安装

### 3.npm全局安装typescript

> 进入命令行cmd
>
> 输入：`npm i -g typescript`

### 4.创建一个ts文件

### 5.使用tsc对ts文件进行编译

> 进入命令行
>
> 进入ts文件所在目录
>
> 执行命令：tsc xxx.ts





# 语法

## 变量类型声明

```typescript
变量类型声明
let a: number = 1;
let b: string;
b = 'qwe'
```



## 函数中类型声明

```tsx
函数中类型声明

1.参数类型声明
参数数量不可多不可少
function sum(a: number, b: number) {
    return a + b;
}
console.log(sum(123, '456'));

2.返回值类型声明
function sum(a: number, b: number): number {
    return a + b;
}
console.log(sum(123, '456'));
```



## 类型

### 字面量

```tsx
let a: 10;
a = 10;

联合类型
let b: "male" | 'female';	|表示或的意思
b = "male";
b = "female";

let c: boolean | string;
c = true;
c = "hello";

```



### any

> 任意类型，相当于关闭TS的类型检测
>
> 不建议使用，万不得已才使用

```tsx
let d: any;	显式的any
let d;		隐式的any
d = 10;
d = 'hello';
d = true;
```



### unknown

> unknown实际是一个类型安全的any
>
> unknown类型的变量不能直接赋值给其他变量

```tsx
let e: unknown;
e = 10;
e = "hello";
e = true;

let s: string;

s = d;	d的类型是any，可以赋值给任意变量

e = 'hello';
s = e;	报错

处理：
1.判断
if(typeof e === 'string'){
    s = e;
}

2.类型断言
    语法：
        a)	变量 as 类型
        b)	<类型>变量
s = e as string；
s = <string>e;
```



### void

> 表示空值，以函数为例，表示没有返回值

```tsx
function fn(): void{
    
}

function fn(): void{
    return 123;	报错
}
function fn(): void{
    return；	可以这样
}
function fn(): void{
    return undefined;	可以这样
}
function fn(): void{
    return null;	可以这样
}
```



### never

> 表示永远不会返回结果

```tsx
function fn(): never{
    throw new Error('报错了！');
}
```



### object

> 表示一个js对象
>
> 语法：`{属性名: 属性值,属性名: 属性值}`
>
> 在属性名后加`?`，表示属性是可选的

```tsx
let b: {name: string};
b = {name: '孙悟空', age: 18}
```



### 联合类型

见字面量

```tsx
联合类型
let b: "male" | 'female';	|表示或的意思
b = "male";
b = "female";

let c: boolean | string;
c = true;
c = "hello";
```



### 类型推断

```tsx
类型推断
let c = true;
c = false;
c = 1;	报错
```



### 类型断言

见unknown

```tsx
类型断言
    语法：
        a)	变量 as 类型
        b)	<类型>变量
s = e as string；
s = <string>e;
```

























