//1.1.===============================================================

//1.Object.defineProperty 修饰的属性不参于循环，不可枚举
var person={
  name:'张三',
  sex:'男',
  //age:11,
}
Object.defineProperty(person,'age',{
  value:18,
  enumerable:true, //控制属性是否枚举，默认是false
  writable:true, //控制属性是否可以修改，默认是false
  configurable:true//Kongzhi属性是否可以删除,默认是false
  get:function(){
    console.log("hello")
  }
})

console.log(person)
console.log(Object.keys(person))

//1.2.数据代理===============================================================

//数据代理 通过一个对象代理另一个对象的属性
let obj={x:100}
let obj2={y:300}
Object.defineProperty(obj2,'x',{
  get(){
    return obj.x;
  },
  set(value){
    obj1.x=value
  }
})

console.log(obj2.x)

