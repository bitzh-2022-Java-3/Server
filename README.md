# Server

## 设计阶段：


### 1. 数据库表结构

1. 会员表 ( user table )

| **列名** | vipNo | name | sex | age | cardDate | phone | heigh | weight | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | VIP卡号 | 姓名 | 性别 | 年龄 | 注册时间 | 手机号码 | 身高(cm) | 体重(kg) |  密码 |
| **数据类型** | String | String | String | int | Date | String | int | double | String(MD5) |


2. 员工表 ( worker table )

| **列名** | workerNo | name | sex | age | hiredate | phone | position | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 职位 | 备注信息 | 密码 |
| **数据类型** | String | String | String | int | Date | String | String | String | String(MD5) |


3. 管理员表 ( admin table )

| **列名** | workerNo | name | sex | age | hiredate | phone | position | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 职位 | 备注信息 | 密码 |
| **数据类型** | String | String | String | int | Date | String | String | String | String(MD5) |


4. 器材表( equipment table )

| **列名** | eid | name | number |
| :----: | :----: | :----: | :----: |
| **数据类型** | **说明** | 同类器材唯一标识id | 器材名称 | 器材数量 |


5. 器材状态表 ( equipment satatus table)

| **列名** | status_eid | status |
| :----: | :----: | :----: |
| **说明** | 器材唯一标识id | 状态：broken,repair,usage,unable |
| **数据类型** | String |
