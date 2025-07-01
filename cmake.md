IDE（Integrated Development Environment）集成开发环境，将开发的大部分功能集成到一个界面中
有以下核心功能：
1. 代码编辑器（语法高亮，自动补全，格式化，智能提示）
2. 编辑器：调用底层工具链
3. 调试器：支持断点，变量监视，调用栈分析
4. 项目管理

## CMakeLists.txt
命令：
1. cmake_minimum_required: cmake最低版本（非必须，不加会警报）
cmake_minimum_required（VERSION 3.0）
2. project:定义项目（名称，版本，描述，web主页，支持语言），
project(<PROJECT-NAME>
       [VERSION <major>[.<minor>[.<patch>[.<tweak>]]]]
       [DESCRIPTION <project-description-string>]
       [HOMEPAGE_URL <url-string>]
       [LANGUAGES <language-name>...])

3. add_executable(可执行程序， 源文件)： 生成可执行程序