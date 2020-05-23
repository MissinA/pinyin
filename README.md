#为lua创造的快速中文转拼音库
>Fast Chinese to Pinyin library for Lua
##安装使用指南
使用luaroks安装
`luarocks install pinyin`
或者直接将pinyin.lua复制到您的项目或者LUA_PATH中

##代码指南
```lua
local pinyin = require'pinyin'
pinyin(chars, isString, separator)
```
@参数1为您要转换的字符串
@参数2如果为true则返回字符串,否则返回为表
@参数3为参数2的增加选项制定拼音间字符

##代码示例
```lua
local pinyin = require'pinyin'
print(pinyin("你好世界", true, "-"))
--输出: ni-hao-shi-jie  n-h-s-j
```
>有两个返回值，第一个返回值为全部拼音，第二个为首拼.
