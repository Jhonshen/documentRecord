# go踩坑
- for range的坑，对于对象遍历时，不能修改对象中的值，类似于取到的是值而不是引用
- go中没有++i 这种用法
- 判断map是否存在某个key可以用if exist
- 有一些代码比较多的go依赖无法引入，可以参考：[解决方案](https://blog.csdn.net/shixiaoyan_/article/details/103411343)
# thrift踩坑
- 建议新增字段在最下方添加并且指定为optional
- 对于上下游thrift定义不一致的情况下，指定为optional在序列化时会给予默认值
