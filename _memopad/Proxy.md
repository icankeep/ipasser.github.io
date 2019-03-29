代理
---
  - 静态代理 --> 代理类需要实现和被代理类一样的接口并重写相应的方法，在被代理对象访问前进行预处理操作和扫尾操作
  - 动态代理
    - JDK动态代理
    - CGLIB动态代理

Spring中AOP
---
- 如果目标对象的实现类实现了接口，Spring AOP 将会采用 JDK 动态代理来生成 AOP 代理类
- 如果目标对象的实现类没有实现接口，Spring AOP 将会采用 CGLIB 来生成 AOP 代理类——不过这个选择过程对开发者完全透明、开发者也无需关心