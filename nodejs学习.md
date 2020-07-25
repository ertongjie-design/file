### 8.3 启动和关闭MongoDB数据库

启动：

```shell
# mongodb 默认使用执行 mongod 命令时所处盘符根目录下的/data/db 作为自己的数据存储目录
# 所以在第一次使用该命令之前先新建一个 /data/db/ 目录
mongod
```

如果想要修改默认的数据存储位置，可以：

```shell
mongod --dbpath=数据目录路径
```

停止：

```shell
直接在控制台Ctrl+C或者直接关闭控制台
```

### 8.4.连接和退出数据库

连接

```shell
# 该命令默认连接本机的MongoDB服务
mongo
```

退出

```shell
# 在连接状态下输入exit退出连接
exit
```

### 8.5 基本命令

+ `show dbs`
  - 查看显示所有数据库
+ `show collections`
  - 查看当前数据库中的集合
+ `db`
  + 查看当前操作的数据库
+ `use 数据库名称`
  - 切换到指定数据库（如果没有会新建，但只有存在数据后才会新建）

#### 8.6 在 Node 中如何操作 MongoDB 数据

## 10 异步编程

### 10.1 回调函数

### 10.2 Promise

回调地狱：callback hell

![373dc8f22770f5eef6459af75a8bf061](C:\Users\Administrator\Pictures\abandon\373dc8f22770f5eef6459af75a8bf061.jpg)

如下是三个异步操作，无法保证执行顺序

```javascript
var fs = require('fs')

fs.readFile('./data/a.txt', 'utf8', function (err, data) {
  if (err) {
    // return console.log('读取失败')
    // 抛出异常
    //    1. 阻止程序的执行
    //    2. 把错误消息打印到控制台
    throw err
  }
  console.log(data)
})
fs.readFile('./data/b.txt', 'utf8', function (err, data) {
  if (err) {
    // return console.log('读取失败')
    // 抛出异常
    //    1. 阻止程序的执行
    //    2. 把错误消息打印到控制台
    throw err
  }
  console.log(data)
})
fs.readFile('./data/c.txt', 'utf8', function (err, data) {
  if (err) {
    // return console.log('读取失败')
    // 抛出异常
    //    1. 阻止程序的执行
    //    2. 把错误消息打印到控制台
    throw err
  }
  console.log(data)
})

```

为保证执行顺序：

```javascript
var fs = require('fs')

fs.readFile('./data/a.txt', 'utf8', function (err, data) {
  if (err) {
    // return console.log('读取失败')
    // 抛出异常
    //    1. 阻止程序的执行
    //    2. 把错误消息打印到控制台
    throw err
  }
  console.log(data)
  fs.readFile('./data/b.txt', 'utf8', function (err, data) {
    if (err) {
      // return console.log('读取失败')
      // 抛出异常
      //    1. 阻止程序的执行
      //    2. 把错误消息打印到控制台
      throw err
    }
    console.log(data)
    fs.readFile('./data/c.txt', 'utf8', function (err, data) {
      if (err) {
        // return console.log('读取失败')
        // 抛出异常
        //    1. 阻止程序的执行
        //    2. 把错误消息打印到控制台
        throw err
      }
      console.log(data)
    })
  })
})

```

为了解决以上编码方式带来的问题（回调地狱嵌套），所以在EcamScript 6 中新增了一个API: `Promise`。

Promise的基本语法：





