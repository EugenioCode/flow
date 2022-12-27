<h1 align="center">rich-workflow</h1>

<p>
  <a href="https://npmcharts.com/compare/rich-workflow?minimal=true"><img src="https://img.shields.io/npm/dt/rich-workflow" alt="Downloads"></a>
  <a href="https://www.npmjs.com/package/rich-workflow"><img src="https://img.shields.io/npm/v/rich-workflow" alt="Version"></a>
  <a href="https://www.npmjs.com/package/rich-workflow"><img src="https://img.shields.io/npm/l/rich-workflow" alt="License"></a>
</p>


> rich 工作流. 覆盖项目全链路生命周期，在于统一脚手架、同构化方案、命令，集中维护、管理，更具语义化


## 安装

```sh
npm i rich-workflow -g
```

## 使用

### 1、脚手架操作

#### 获取模板列表  
```sh
rich list
```

#### 创建项目
```sh
rich init <模板名称> [项目名称]

# 利用本地的模板缓存创建项目
rich init <模板名称> [项目名称] --offline
```

#### 项目启动
```sh
rich run dev
```

#### 项目构建
```sh
rich run build
```

#### js代码格式化
```sh
rich run lint:es [<文件地址>...] [<路径>...] [--fix]
```

#### style代码格式化
```sh
rich run lint:style  [<文件地址>...] [<路径>...] [--fix]
```

### 2、Git操作集

#### branch: 分支相关操作
```sh
# 创建分支
rich branch [-b] <分支名>

# 删除分支
rich branch -d <分支名>

# 关键词匹配所有分支
rich branch -s <关键词>
```
#### renew: 远程更新分支
```sh
# 删除指定的分支，从master重新创建
rich renew [<分支名>...]
```

#### merge: 合并分支
```sh
# 合并到master后删除该远程分支
rich merge [<分支名>]
```

#### push: 推送代码至远程
```sh
# 推送代码时会同步到远程
rich push
```

#### ignore: 删除并忽略指定文件
```sh
# 删除项目中所有.DS_Store文件，并添加至.gitnore
rich ignore .DS_Store
```

## 3、安装插件

```sh
rich install eslint

rich install stylelint

rich install commitlint
```

## 4、安装license
```sh
rich license --year 2021-2023 --holder rich-workflow
```