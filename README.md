# Server

## 数据库表结构

### 会员表 ( user table )
| uid | name | pwd | phone | group |
| :----: | :----: | :----: | :----: | :----: |
| 用户唯一标识id | 昵称 | 密码 | 手机号 | 用户权限组: user |

### 员工表 ( worker table )
| wid | name | sex | age | hiredate | phone | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 备注信息 | 密码 |
| String | String | String | int | Date | String | String | String(MD5)

### 管理员表 ( admin table )
| uid | name | pwd | phone | group |
| :----: | :----: | :----: | :----: | :----: |
| 用户唯一标识id | 昵称 | 密码 | 手机号 | 用户权限组: admin |

### 器材表( equipment table )
| eid | name | number |
| :----: | :----: | :----: |
| 同类器材唯一标识id | 器材名称 | 器材数量 |

### 器材状态表 ( equipment satatus table)
| status_eid | status |
| :----: | :----: |
| 器材唯一标识id | 状态：repair,usage,unable |

