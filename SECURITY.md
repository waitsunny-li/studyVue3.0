# Reporting a Vulnerability



### compiler-core
  - 这个编译器的暴露了 AST 和 baseCompile 相关的 API，它能把一个字符串变成一棵 AST

### runtime-core
  - 核心模块

### runtime-dom
  - 这个模块是基于上面模块而写的浏览器上的 runtime，主要功能是适配了浏览器环境下节点和节点属性的增删改查。它暴露了两个重要 API：render 和 createApp，并声明了一个 ComponentPublicInstance 接口。

### reactivity 
  - 这是一个极其重要的模块，它是一个数据响应式系统。其暴露的主要 API 有 ref(数据容器)、reactive(基于 Proxy 实现的响应式数据)、computed(计算数据)、effect(副作用) 等几部分

### compiler-core
  - 这个编译器的暴露了 AST 和 baseCompile 相关的 API，它能把一个字符串变成一棵 AST

### compiler-dom
  - 这个模块则基于上个模块，针对浏览器做了适配，如对 textarea 和 style 标签做了特殊处理。