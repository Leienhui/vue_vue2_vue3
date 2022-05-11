#  vue知识点





## vue基础知识

### 1.Vue是什么？

​	 Vue是一套动态构建用户界面的**渐进式** JavaScript 框架        ——尤雨溪

### 2. Vue特点

1. 遵循 **MVVM** 模式 

   ​	1. M：模型(Model) ：data中的数据

   ​    2. V：视图(View) ：模板代码

   ​     3. VM：视图模型(ViewModel)：Vue实例

2. 编码简洁, 体积小, 运行效率高, 适合移动/PC 端开发

3. 采用组件化模式，代码复用率高，易于维护

4. 声明式编码，无需操作dom，提高开发效率

5. 使用虚拟dom+diff算法，尽量复用dom节点

### 3.初识Vue



[Vue引入](vue_basic/01_初识Vue/初识Vue.html)



**一个vue实例不能同时接管多个容器，否则只有第一个容器有效**



[一个vue实例同时接管多个容器](vue_basic/01_初识Vue/一个Vue实例对应多个容器.html)

### 4.[Vue模板语法](vue_basic/02_Vue模板语法/模板语法.html)

### 5.[数据绑定](vue_basic/03_数据绑定/数据绑定.html)

### 6.[el与data的两种写法](vue_basic/04_el与data的两种写法/el与data的两种写法.html)

### 7.[Vue中的MVVM](vue_basic/05_MVVM模型/Vue中的MVVM.html)

### 8.数据代理

[Object.defineProperty](vue_basic/06_数据代理/1.回顾Object.defineProperty方法.html)

[何为数据代理](vue_basic/06_数据代理/2.何为数据代理.html)

[Vue中的数据代理](vue_basic/06_数据代理/3.Vue中的数据代理.html)

### 9.事件处理

[事件的基本使用](vue_basic/07_事件处理/1.事件的基本使用.html)

[事件修饰符](vue_basic/07_事件处理/2.事件修饰符.html)

[键盘事件](vue_basic/07_事件处理/3.键盘事件.html)

### 10.计算属性

[姓名案例_插值语法实现](vue_basic/08_计算属性/1.姓名案例_插值语法实现.html)

[姓名案例_methods实现](vue_basic/08_计算属性/2.姓名案例_methods实现.html)

[姓名案例_计算属性实现](vue_basic/08_计算属性/3.姓名案例_计算属性实现.html)

[姓名案例_计算属性简写](vue_basic/08_计算属性/4.姓名案例_计算属性简写.html)

### 11.监视属性

[天气案例](vue_basic/09_监视属性/1.天气案例.html)

[天气案例_监视属性](vue_basic/09_监视属性/2.天气案例_监视属性.html)

[天气案例_深度监视](vue_basic/09_监视属性/3.天气案例_深度监视.html)

[天气案例_监视属性_简写](vue_basic/09_监视属性/4.天气案例_监视属性_简写.html)

[姓名案例_watch实现](vue_basic/09_监视属性/5.姓名案例_watch实现.html)

### 12.[绑定样式](vue_basic/10_绑定样式/绑定样式.html)

### 13.[条件渲染](vue_basic/11_条件渲染/条件渲染.html)

### 14.列表渲染

[基本列表](vue_basic/12_列表渲染/1.基本列表.html)

[key的原理](vue_basic/12_列表渲染/2.key的原理.html)

[列表过滤](vue_basic/12_列表渲染/3.列表过滤.html)

[列表排序](vue_basic/12_列表渲染/4.列表排序.html)

[更新时的一个问题](vue_basic/12_列表渲染/5.更新时的一个问题.html)

[Vue监测数据改变的原理_对象](vue_basic/12_列表渲染/6.Vue监测数据改变的原理_对象.html)

[模拟一个数据监测](vue_basic/12_列表渲染/7.模拟一个数据监测.html)

[Vue.set的使用](vue_basic/12_列表渲染/8.Vue.set的使用.html)

[Vue监测数据改变的原理_数组](vue_basic/12_列表渲染/9.Vue监测数据改变的原理_数组.html)

[总结Vue数据监测](vue_basic/12_列表渲染/10.总结Vue数据监测.html)

### 15.[收集表单数据](vue_basic/13_收集表单数据/收集表单数据.html)

### 16.[过滤器](代码/vue_basic/14_过滤器/过滤器.html)

### 17.内置指令

[v-text_指令](vue_basic/15_内置指令/1.v-text_指令.html)

[v-html_指令](vue_basic/15_内置指令/1.v-html_指令.html)

[v-cloak_指令](vue_basic/15_内置指令/3.v-cloak_指令.html)

[v-once_指令](vue_basic/15_内置指令/4.v-once_指令.html)

[v-pre_指令](vue_basic/15_内置指令/5.v-pre_指令.html)

### 18.自定义指令

[自定义指令](vue_basic/16_自定义指令/1.自定义指令.html)

[回顾一个DOM操作](vue_basic/16_自定义指令/2.回顾一个DOM操作.html)

### 19.生命周期

[引出生命周期](vue_basic/17_生命周期/1.引出生命周期.html)

[分析生命周期](vue_basic/17_生命周期/2.分析生命周期.html)

[总结生命周期](vue_basic/17_生命周期/3.总结生命周期.html)

### 20.非单文件组件

[基本使用](vue_basic/18_非单文件组件/1.基本使用.html)

[几个注意点](vue_basic/18_非单文件组件/2.几个注意点.html)

[组件的嵌套](vue_basic/18_非单文件组件/3.组件的嵌套.html)

[VueComponent](vue_basic/18_非单文件组件/4.VueComponent.html)

[一个重要的内置关系](vue_basic/18_非单文件组件/5.一个重要的内置关系.html)

## [Vue脚手架路由等知识](vue_test/README.md)

## [vue3快速上手](../资料（含课件）/01_课件\vue3快速上手.md)


## vscode 知识点

```
GET http://127.0.0.1:5500/favicon.ico 404 (Not Found)
```

但使用 live server 插件以后，当选中`open with Live Server`他就会在本机 5500 的端口号上开一台内置的服务器，并把当前整个工程的所有文件及文件夹都作为这台服务器的根 资源。
