# flutter

#### 环境配置
1. 获取Flutter SDK
```
git clone -b beta https://github.com/flutter/flutter.git
export PUB_HOSTED_URL=https://pub.flutter-io.cn //国内用户需要设置
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn //国内用户需要设置
export PATH=`pwd`/flutter/bin:$PATH
```
2. 运行flutter doctor
```
flutter doctor
```
该命令检查您的环境并在终端窗口中显示报告。Dart SDK已经在捆绑在Flutter里了，没有必要单独安装Dart。 仔细检查命令行输出以获取可能需要安装的其他软件或进一步需要执行的任务（以粗体显示）
其中你可能需要安装android studio，android SDK，升级XCODE版本等问题，按粗体提示安装即可。 

3. 更新环境变量（可以在第二步执行）
* 确定您Flutter SDK的目录，您将在步骤3中用到。
* 打开(或创建) $HOME/.bash_profile. 文件路径和文件名可能在您的机器上不同.
* 添加以下行并更改[PATH_TO_FLUTTER_GIT_DIRECTORY]为克隆Flutter的git repo的路径:
```
export PUB_HOSTED_URL=https://pub.flutter-io.cn //国内用户需要设置
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn //国内用户需要设置
export PATH=PATH_TO_FLUTTER_GIT_DIRECTORY/flutter/bin:$PATH
```
注意：PATH_TO_FLUTTER_GIT_DIRECTORY 为你flutter的路径【第一步git clone下来存放flutter的路径】，比如“~/document/code”
* 运行 source $HOME/.bash_profile 刷新当前终端窗口.

#### 配置编辑器（VS CODE)
```
1. 安装 VS Code, 安装1.20.1或更高版本.
2. 安装 Dart Code 插件
```
#### 创建项目以及启动项目
```
1. 启动 VS Code
2. 调用 View>Command Palette…
3. 输入 ‘flutter’, 然后选择 ‘Flutter: New Project’ action
4. 输入 Project 名称 (如myapp), 然后按回车键
5. 指定放置项目的位置，然后按蓝色的确定按钮
6. 等待项目创建继续，并显示main.dart文件
```
需要注意： 项目必须在VSCODE中使用flutter create这种方式创建，不然无法使用热更新及一些未知问题。

#### 参考资料
* [安装](https://flutterchina.club/setup-macos/)
* [配置编辑器](https://flutterchina.club/get-started/editor/#vscode)
* [创建项目以及启动](https://flutterchina.club/get-started/test-drive/#vscode)