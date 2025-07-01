IDE（Integrated Development Environment）集成开发环境，将开发的大部分功能集成到一个界面中
有以下核心功能：
1. 代码编辑器（语法高亮，自动补全，格式化，智能提示）
2. 编辑器：调用底层工具链
3. 调试器：支持断点，变量监视，调用栈分析
4. 项目管理

## CMakeLists.txt
## 命令：
1. cmake_minimum_required: cmake最低版本（非必须，不加会警报）
cmake_minimum_required（VERSION 3.0）
2. project:定义项目（名称，版本，描述，web主页，支持语言），
project(<PROJECT-NAME>
       [VERSION <major>[.<minor>[.<patch>[.<tweak>]]]]
       [DESCRIPTION <project-description-string>]
       [HOMEPAGE_URL <url-string>]
       [LANGUAGES <language-name>...])

3. add_executable(可执行程序， 源文件)： 生成可执行程序

4. set(变量 源文件): 将多个源文件存储为变量,类似宏定义
set(A[2] a.c b.c c.c)
set(A a.c;b.c;c.c)
变量和分割各有两种写法
调用A用${A}

5. 指定C++标准
自带宏CMAKE_CXX_STANDARD
6. 制定可执行程序输出路径
自带宏EXECUTABLE_OUTPUT_PATH, 建议用绝对路径
7. aux_source_directory(< dir > < variable >)将dir所有的源文件存到variable中
8. file(GLOB/GLOB_RECURSE 变量名 要搜索的文件路径和文件类型)
9. include_directories(headpath)添加头文件

## CMake指令
1. cmake CMakeLists的地址：执行cmake
	（地址在同一级“.",上一级”.."）
2. aux_source_directory(< dir > < variable >)将dir所有的源文件存到variable中
3. 