# Server

## 数据库表结构

### 会员表 ( user table )
| vid | name | sex | age | cardDate | phone | heigh | weight | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| VIP卡号 | 姓名 | 性别 | 年龄 | 注册时间 | 手机号码 | 身高(cm) | 体重(kg) |  密码 |
| String | String | String | int | Date | String | int | double | String(MD5) |

### 员工表 ( worker table )
| wid | name | sex | age | hiredate | phone | position | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 职位 | 备注信息 | 密码 |
| String | String | String | int | Date | String | String | String | String(MD5) |

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
| 器材唯一标识id | 状态：broken,repair,usage,unable |

