欢迎大家补充经验， 共同进步


## 深圳 2018 20k+ react向 前端遇到的面试题

### JS
1. redux中间件原理
2. redux-router的为什么可以在所有路由中的可以保存状态
3. 有没有看过什么令你眼前一亮的库，里面用到什么技术
4. vue和react的区别
5. 什么是函数编程
6. mobx用过吗
7. 你写技术博客的习惯吗
8. 继承的方法有几种，可以简单说一些吗
9. 装饰器用过吗
10. 说说你对redux的理解
11. express的中间件原理
12. node模块的查找方式
13. 说一下react的生命周期顺序


### 布局
1. 1px的问题遇到过吗?你的解决方案的原理可以简单说一下吗
2. 点击底部输入框，输入法面板挡住页面底部有什么解决方案
3. flex布局，调节子元素位置相关的属性有哪一些


### 职业问题
1. 你对自己以后的职位规划是什么
2. 你对加班怎么看



## 知乎校招
1. 如何把一个 长的url 短编码以及解码        
    不用考虑解析url  直接采用映射关系
    <pre><code>   
      const arr = [{   
        long: '',   
        short: '',    
      }]    
      // const url = 'https://github.com/xiao-ben/FE-Interview-experience/edit/master/README.md'    
      decode = (url) => {    
         obj = {    
            long: url,    
            short:  'https://github.com/' + arr.length   //很多条时采用base64编码(arr.length) 具体方法自行百度    
         };    
         arr.push(obj);    
         return obj.long;     
      }     
      undecode = (url) => {     
         return arr.find(item => item.short === url).long;    
      }    
    </code></pre>    
  
2. 考虑如果很多url  两台服务器存储会有什么问题
3. typescript 相关知识点 
4. export 和  default 除了{} 还有什么差别
5. reaxt router api 以及 匹配原理
6. setstate 之后干了什么
7. diff算法 以及 返回什么
   返回的是对 dom 树的一系列操作
8. context api
9. react16 有哪些变动
10. 组件通信 以及 redux 和 mobx的优劣
11. css moudles 根据什么加的 hash
    根据路径加文件名
12. promise.cancle实现
    new 一个然后race


## 夜未央 上海
1. node.js  
2. 介绍算法  
3. 谈设计模式和自己的理解等等     
4. react相关知识   
5. 作用域和闭包    
6. h5新特性   
7. 如果一个页面同时有成百个ajax请求会出现什么问题，怎么处理   
8. localstorage最大存储到5m，那么现在如果数据超过甚至更多，你会怎么处理，或有其他更好方法

## 风林 深圳
1. 如何理解html语义化
2. css实现垂直居中有多少种方案
3. 如何清除浮动
4. 盒模型
5. 选择器优先级如何确定
6. 如何实现深拷贝
7. 如何用正则实现string.trim()
8. 写出至少三种数组去重
9. js如何实现继承
10. http 301 跟 302 的区别是什么
11. Cache-Control 跟 Etage 的区别
12. 如何强制释放闭包，原型链顶端是什么
13. 如何对数组进行乱序
14. 使用闭包实现一个函数，每执行一次返回值加1

## 北京 校招 
1.webpack 多入口 如何配置  publicpath的左右 [chunkhash]根据是如何实现的 
2.babel5 与 babel 6 的不同 
3.如何封装自己的 http.js(用途 比如统一携带token)
4.async await  相关知识点
5.promise.all([1, 2, 3]) 如果其中一个 出现错区之后 如何保证其他的正常运行
6.http 相关 比如 一个请求包含什么 返回包含什么 以及如何判断一个请求 是同步还是异步
7.flex 布局相关
8.vue 双向数据绑定原理
