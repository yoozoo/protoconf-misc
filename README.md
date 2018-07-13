# protoconf

`protoconf`是一个方便配置中心应用与管理的**命令行**工具。

## 运行环境

`protoconf`使用纯Go开发，故可能以单一可执行文件的形式提供，无需运行时环境便可运行于：

* windows
* linux
* mac

32/64位系统均可支持。

# 安装

具体安装，可以参考[这里](docs/配置中心_php_confd.md)。

# 功能

## 代码生成

`protoconf`主要通过代码生成的形式在方便应用开发，目前支持一下方面的代码生成：

* java
  * spring boot
* php
* confd配置文件

代码生成是以protobuff的插件形式提供，即：

## 管理功能

`protoconf`主要通过命令行工具来方便配置中心管理，命令格式类似：

  protoconf action app.proto --endpoints --user

### action

action包括：

* `list` list all keys
* `get` get value for one key
* `getall` get value for all keys
* `set` set value for one key
* `grant` grant one key to one user
* `grantall` assign all keys to one user
* `revoke` grant one key read access to a user
* `revokeall` grant all key read access to one user
* `findref` find all app reference
