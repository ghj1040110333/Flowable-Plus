## JAVA-开发
BufferingApplicationStartup:
 
 是Spring Boot 中的一个类，它的作用是在应用程序启动时缓冲处理请求。当应用程序启动时，通常会有一个短暂的延迟，因为需要加载和初始化各种组件。通过使用 BufferingApplicationStartup，可以在这个延迟期间缓冲处理请求，从而减少用户等待时间。

具体来说，BufferingApplicationStartup 会创建一个线程池来处理请求，这个线程池会在应用程序启动完成后才开始处理请求。这样，在应用程序启动过程中，所有的请求都会被缓存起来，等到应用程序启动完成后再进行处理。这样可以确保在应用程序启动过程中，用户的请求不会因为应用程序尚未完全准备好而受到影响。


## JS-开发

# 1.module.exports

module.exports 是 Node.js 中用于导出模块的语法。通过 module.exports，可以将一个对象、函数或值导出，以便其他模块可以使用它们

```
// 导出一个对象
  const myObject = {
    name: 'John',
    age: 30,
    sayHello: function() {
    console.log('Hello!');
    }
  };
  module.exports = myObject;
```

# 2.<router-view> 

是 Vue.js 中的一个组件，用于在单页面应用中显示路由对应的组件。它会根据当前路由的变化自动更新显示的组件。

theme-picker 是一个用于选择主题的组件