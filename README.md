
# 一、D8

D8 是一个非常有用的调试工具，你可以把它看成是 debug for V8 的缩写。我们可以使用 d8 来查看 V8 在执行 JavaScript 过程中的各种中间数据，比如作用域、AST、字节码、优化的二进制代码、垃圾回收的状态，还可以使用 d8 提供的私有 API 查看一些内部信息。

# 二、使用jsvu安装D8

jsvu是一个js引擎管理工具，如下图所示。

![alt text](image.png)

 
## 1. 本地安装jsvu

可以使用```npm install jsvu -g```进行全局安装，我们这里为了避免影响到其他内容，采取了本地安装的方法。

```js
npm install jsvu -D
```

## 2. 安装引擎

前面我们提到jsvu是一个js引擎管理工具，所以需要自己选择需要使用的引擎。直接执行```npx jsuv```命令。

### 1. 选择系统

第一步选择适合自己的系统即可。

![alt text](image-1.png)

### 2. 选择js引擎

第二步选择自己需要的js引擎，默认是全部都下载的，我们需要将除了v8 debug其余的js引擎使用空格键去掉，然后只选择一个v8 debug。

![alt text](image-2.png)

### 3. 回车安装

选择正确的引擎以后回车进行安装。

![alt text](image-3.png)
