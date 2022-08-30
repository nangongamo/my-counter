## Move 初体验

编写 Move 代码、构建、打包、Starcoin Dev 网络部署上链、链上交互等等。



### 涉及 mpm 命令

```bash
# move 构建
mpm package build
# move 打包 二进制包
mpm release
# move 项目初始化
mpm package new <project_name>
```



### 快速创建一个 Move 项目

```bash
mpm package new <project_name>
```



### Move 项目结构

```
project_name
├── Move.toml
└── sources
```



### 定义模块的语法

```move
module <address>::<identifier> {
    // module body
}
```



### 资源命名空间

```
<address>::<module_identifier>::<structure>
```



### 熟悉命令

- account execute-function

  ```
  account execute-function --function  <0x地址>::<模块>::<函数> --arg xxx
  ```



### 发展

> 1. `script` 可能会被废弃，推荐用 `script function` 做入口方法。
> 2. 下个版本的 Move 会用 `public entry fun` 替代 `public(script) fun`

