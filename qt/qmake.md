qmake用于项目配置，类似cmake
.pro文件是项目配置文件，类似于CMakeLists.txt

## 编译语法

TARGET = myapp       # 生成的可执行文件名
SOURCES += main.cpp  # 源文件列表
HEADERS += myclass.h # 头文件列表
### 模块声明
QT += widgets        # 图形界面组件
QT += core        # 核心模块（默认包含）
QT += gui        # 图形界面基础（默认包含）
QT += network        # 网络功能
QT += sql        # 数据库
QT += multimedia        # 多媒体
