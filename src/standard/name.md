## 命名法：

### 1.驼峰命名法(小驼峰)

**getUser**

### 2.帕斯卡命名法(大驼峰)

**GlobalHeader**

### 3.短横线命名法

**user-center**

### 4.下划线命名法

**MAX_LENGTH**

## 文件、文件夹命名：

- 文件夹作为**路由页面**时用小写字母，包含多个单词时，单词之间建议使用半角的连词线 ( - ) 分隔, 即**短横线命名法**，此时 vue 文件为**index.vue**。
- 文件夹作为**vue 组件**时用**大写驼峰命名法**。
- 文件作为**vue 组件**时用**大写驼峰命名法**。
- 文件作为**use 函数**时用**小驼峰命名法**。
- 其余文件用**短横线命名法**。

## 变量命名：

### 命名方式 : 小驼峰式命名方法

**命名规范 : 类型+对象描述的方式，如果没有明确的类型，就可以使前缀为名词**

| 动词 | 含义                   | 返回值                                               |
| ---- | ---------------------- | ---------------------------------------------------- |
| can  | 判断是否可执行某个动作 | 函数返回一个布尔值 true: 可执行; false: 不可执行     |
| has  | 判断是否含有某个值     | 函数返回一个布尔值 true: 含有此值; false: 不含有此值 |
| is   | 判断是否为某个值       | 函数返回一个布尔值 true: 为某个值; false: 不为某个值 |
| get  | 获取某个值             | 函数返回一个非布尔值                                 |
| set  | 设置某个值             | 无返回值、返回是否设置成功或者返回链式对象           |

```ts
/** 是否可读 */
function canRead() {
	return true;
}

/** 获取姓名 */
function getName() {
	return "";
}
```

## 常量

### 命名方法 : 使用大写字母和下划线来组合命名，下划线用以分割单词。

```ts
const MAX_COUNT = 10;
const URL = "http://www.baidu.com";
```

## TS 类型接口 interface 和 type

### 命名方法：大写驼峰

```typescript
interface PersonInfo {
	/** 姓名 */
	name: string;
	/** 性别 '0':男; '1': 女; '2': 未知 */
	gender: "0" | "1" | "2";
	/** 年龄 */
	age: 25;
}
```