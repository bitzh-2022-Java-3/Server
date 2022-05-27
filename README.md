# Server

## 设计阶段：


### 1. 数据库表结构
以下的所有表中，以第一个列名作为该表的主键
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

| **列名** | eNo | name | number |
| :----: | :----: | :----: | :----: |
| **说明** | 器材编号(具体到种类) | 器材名称 | 器材数量 |
| **数据类型** | String | Strinhg | int |

5. 器材状态表 ( equipment satatus table)

| **列名** | statusNo | status | eNO |
| :----: | :----: | :----: | :----: |
| **说明** | 器材编号(具体到某个) | 状态：broken,repair,usage,unable | 器材编号(分类) |
| **数据类型** | String | String | String |


6. 选课表( class table )

| **列名** | classNo | name | workerNo | classTime | classDate | price |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 课程编号 | 课程名 | 上课教师工号 | 课时 | 课程开始时间 | ¥价格(单位：分) |
| **数据类型** | String | String | String | int | Date | int |


7. 课程表( class schedule table )

| **列名** | vipNo | classNo | time | surplusTime |
| :----: | :----: | :----: | :----: | :----: |
| **说明** | VIP卡号 | 课程编号 | 报名时间 | 剩余课时 |
| **数据类型** | String | String | Date | int |
