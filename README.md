# IdGuard

[![](https://jitpack.io/v/ZTWave/IdGurad.svg)](https://jitpack.io/#ZTWave/IdGurad)

#### 介绍
Android 资源混淆

#### 使用说明

 **注：请在执行操作前备份代码** 

在`project`的`build.gradle`中的`buildscript`下添加

```
repositories {  
  maven { url 'https://jitpack.io' }  
}  
dependencies {  
  classpath 'com.github.ZTWave:IdGurad:0.0.5'  
}
```

在app下的build.gradle中添加

```
plugins {
  id 'idguard'
}
```

在`Android Studio` 的`Task`中可以找到 `LayoutGuard` `IdGuard` `ResGuard` 这三个`Task `

1. `LayoutGuard` : 可以将`layout`文件进行随机命名并更新引用
2. `IdGuard` : 可以将`view`的`id`进行重命名并更新引用
3. `ResGuard` : 可以把 `mipmap` 和 `drawable` 中的 资源文件进行随机命名并更新引用

![GradleTask](https://pic.imgdb.cn/item/64a542e81ddac507cc932105.jpg)

#### 感谢

[XmlClassGuard](http://https://github.com/liujingxing/XmlClassGuard)
