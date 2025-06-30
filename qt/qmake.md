qmake用于项目配置，类似cmake
.pro文件是项目配置文件，类似于CMakeLists.txt

## 控制台命令
qmake ：根据.pro文件生成MakeFile
qmake -project ：生成.pro文件（自动添加sources）
## 编译语法

TARGET = myapp       # 生成的可执行文件名
SOURCES += main.cpp  # 源文件列表
HEADERS += myclass.h # 头文件列表
INCLUDEPATH += .       # 将当前目录加入头文件搜索路径（用于加入自定义头文件）
### 模块声明
QT += widgets        # 图形界面组件
QT += core        # 核心模块（默认包含）
QT += gui        # 图形界面基础（默认包含）
QT += network        # 网络功能
QT += sql        # 数据库
QT += multimedia        # 多媒体
### 模板类型
TEMPLATE = app    # 应用程序
TEMPLATE = lib     # 库
TEMPLATE = subdirs    # 子项目管理
TEMPLATE = aux     # 非编译项目
