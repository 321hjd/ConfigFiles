# ConfigFiles
各种环境的常用配置文件

* Windows下链接建立方式（一般用符号链接，注意**需要管理员权限**）

  `mklink [[/D] | [/H] | [/J]] Link Target`

  * `/D`：创建目录符号链接。不加此选项默认为文件符号链接。
  * `/H`：创建硬链接而非符号链接。
  * `/J`：创建目录联接。
  * `Link`：指定新的符号链接名称。
  * `Target`：指定新链接引用的路径(相对或绝对，最好使用绝对路径，移动源文件后链接也不会失效)。

* 注意：ConfigFiles文件夹应该放在用户目录下！

* 示例：将`_vimrc`配置文件链接到用户目录下
    `mklink C:\Users\xxx\_vimrc C:\Users\xxx\ConfigFiles\Vim\_vimrc`

  
