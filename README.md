##1. Gradle 代码片段
 
 1. 使用方式
 在 module 的build.gradle 引入 依赖即可
 
 > 统计 方法执行顺序
 ```
apply from: 'AppMethodOrder.gradle'

 ```
 > 自动输出所有task的耗时
 ```
apply from:'taskListener.gradle'
 ```
 
  > 自动判断task的build类型 是debug模式还是release模式
  ```
 apply from:'taskRelease.gradle'
  ```
  
 > 对于jenkins 自动化打包 时 windows 平台缓存路径过长超过256字符的bug 直接参考 gradle.properties
    
 > Travis CI -持续集成时 直接复制拷贝 目录文件 .travis.yml 到项目根目录即可