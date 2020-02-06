# PASSWORD
> 某天朋友说她游戏账号密码都忘记了，我就干脆写个网页来帮她记录账号密码。很简单的一个小项目。疫情在家，实在无聊，哈哈哈。

# 可行/不可行的功能
|  可行 |  不可行 |
| ------------ | ------------ |
| 登录  | 注册（需在数据库添加记录）  |
|  修改账号密码记录 | 修改游戏区号/角色昵称等功能  |
|  添加账号记录 | 无  |
|  删除账号记录 | 无法撤销删除操作  |
|  已登录验证 |  无 |
|  非法登录验证 |  无 |

# 值得注意的事情
- 使用的是MYSQL的PDO连接方式
- 运行环境MYSQL 5.6/PHP 7.1
- 你需要在以下文件修改你的数据库账号和密码

|  pass_add.php |
| ------------ |
| **pass_del.php** |
|  **pass_set.php** |
|  **pass_login.php**|
|  **pass_list.php** |
|  **pass_out.php** |

- 你还需要把目录下的SQL文件导入的你的数据库
- 创建新用户的时候在Members_Basic_Info 添加数据 Members_Token不填
- 创建新用户的时候还需要创建新的表，SQL语句如下
```sql
CREATE TABLE `新表名字` LIKE `test`;
```


