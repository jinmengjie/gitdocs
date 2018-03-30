### 工程化

#### 对webpack、gulp、grunt等有没有了解？对比

[前端构建工具Gulp/browserify/webpack/npm？](https://www.zhihu.com/question/37694275/answer/78757253)

Grunt / Gulp 和 browserify / webpack 不是一回事。

1）Gulp / Grunt 可以理解为帮助前端自动化的工具，用于优化前端工作流程。比如自动刷新页面、combo、压缩css、js、编译less等等。[Grunt vs Gulp](https://www.cnblogs.com/chris-oil/p/5746427.html)

2）browserify / webpack 提供的是一个前端模块化的方案，和requirejs类似但又有不同。requirejs是一种在线"编译" 模块的方案，相当于在页面上加载一个AMD 解释器，以便于览器能够识别 define、exports、module，而这些东西就是用于模块化的关键。而browserify / webpack，则是一个预编译模块的方案。它是预编译的，不需要在浏览器中加载解释器。因此完全可以gulp+webpack 或者gulp+browserify这样的方式搭配使用，甚至，只使用webpack，由于其强大的插件支持，也能满足绝大多数需求了。

#### webpack的入口文件怎么配置，多个入口怎么分割

通过entry配置入口文件

[入门Webpack，看这篇就够了](https://www.jianshu.com/p/42e11515c10f)

#### webpack的loader和plugins的区别

[webpack之loader和plugin简介](https://zhuanlan.zhihu.com/p/28245984)

#### gulp的具体使用

[gulp资料收集](https://github.com/Platform-CUF/use-gulp)

#### 前端工程化的理解、如何自己实现一个文件打包，比如一个JS文件里同时又ES5 和ES6写的代码，如何编译兼容他们

[谁能介绍下web前端工程化？](https://www.zhihu.com/question/24558375/answer/139920107)

webpack进行文件打包，通过babel-loader转化ES6代码

