# flutter与iOS的详细交互教程

iOS工程使用的是Swift

## 一、初始化工程

### 1.1 iOS初始化工程

使用Xcode创建工程，如图操作:

<img src="https://github.com/STShenZhaoliang/flutter-ios/raw/master/images/image1.png" width="100%" height="100%">

### 1.2 flutter初始化工程

在终端输入：`flutter create -t module flutter_demo`,`flutter_demo`是要创建的flutter工程的名称,如图所示：

<img src="https://github.com/STShenZhaoliang/flutter-ios/raw/master/images/image2.png" width="100%" height="100%">

### 1.3 初始化完成

全部的工程文件如图所示：

<img src="https://github.com/STShenZhaoliang/flutter-ios/raw/master/images/image3.png" width="100%" height="100%">

## 二、iOS工程配置

### 2.1 使用 Cocoapods 将 flutter 引入工程中

在Podfile添加以下代码, flutter_application_path为flutter工程的相对路径

```
flutter_application_path = "../flutter_demo"
eval(File.read(File.join(flutter_application_path, '.ios', 'Flutter', 'podhelper.rb')), binding)

```

如图操作见下：

<img src="https://github.com/STShenZhaoliang/flutter-ios/raw/master/images/image4.png" width="100%" height="100%">

然后执行pod install，安装完成如下：

<img src="https://github.com/STShenZhaoliang/flutter-ios/raw/master/images/image5.png" width="100%" height="100%">





