

## 2.起步

安装：

```shell
npm i mongoose
```

hello world:

```javascript
var mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/test', { useMongoClient: true });
mongoose.Promise = global.Promise;

var Cat = mongoose.model('Cat', { name: String });

var kitty = new Cat({ name: 'Zildjian' })
kitty.save(function (err) {
  if (err) {
  	console.log(err)
  } else {
    console.log('meow')
  }
})
```

## 3.官方指南

### 3.1 设计 Schema 发布 Model

```javascript
var mongoose = require('mongoose')

var Schema = mongoose.Schema

// 1. 连接数据库
// 指定连接的数据库不需要存在，当向数据库中插入第一条数据时会自动创建
mongoose.connect('mongodb://localhost/itcast')

// 2. 设计文档结构（表结构）
// 字段名称就是表结构中的属性名称
// 约束的目的是为了数据的完整性，不有脏数据
var userSchema = new Schema({
  username: {
    type: String,
    required: true // 必须有
  },
  password: {
    type: String,
    required: true
  },
  email: {
    type: String
  }
})

// 3. 将文档结构发布为模型
//		mongoose.model 方法就是用来将一个文档结构发布为模型
//		第一个参数：传入一个大写名词单数字符串用来表示你的数据库名称
//							mongoose 会自动将大写名词的字符串生成 小写复数 的集合名称
//							例如这里的 User 最终会变成 users 集合名称
//		第二个参数：你的文档结构
//
//		返回值：模型构造函数
var User = mongoose.model('User', userSchema)

// 4. 当我们有了模型构造函数之后，就可以使用这个构造函数对 users 集合中的数据展开操作
```

### 3.2 增加数据

```javascript
var admin = new User({
  username: 'admin',
  password: '123456',
  email: 'admin@admin.com'
})

admin.save(function (err, ret) {
  if (err) {
    console.log('保存失败')
  } else {
    console.log('保存成功')
    console.log(ret)
  }
})
```

### 3.3 查询

查询所有：

```javascript
User.find(function (err, ret) {
  if (err) {
    console.log('查询失败')
  } else {
    console.log(ret)
  }
})
```

按条件查询所有：

```javascript
User.find({
  username: 'zs'
}, function (err, ret) {
  if (err) {
    console.log('查询失败')
  } else {
    console.log(ret)
  }
})
```

查询单个：

```javascript
User.findOne({
  username: 'zs'
}, function (err, ret) {
  if (err) {
    console.log('查询失败')
  } else {
    console.log(ret)
  }
})
```



### 3.4 删除数据

根据条件删除所有：

```javascript
User.remove({
  username: 'zs'
}, function (err, ret) {
  if (err) {
    console.log('删除失败！')
  } else {
      console.log('删除成功！')
      console.log(ret)
  }
})
```

根据条件删除一个：

```javascript
Model.findOneAndRemove(conditions, [options], [callback])
```

根据id删除一个：

```javascript
Model.findByIdAndRemove(id, [options], [callback])
```

### 3.5 更新数据

根据条件更新所有：

```javascript
Model.update(conditions, doc, [options], [callback])
```

根据指定条件更新一个：

```javascript
Model.findOneAndUpdate([conditions], [update], [options], [callback])
```

根据id更新一个：

```javascript
User.findByIdAndUpdate('', {
  password: '123'
}, function (err, ret) {
  if (err) {
    console.log('更新失败')
  } else {
    console.log('更新成功')
  }
})
```

