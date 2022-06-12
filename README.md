
##  数据库表结构

1. 会员表 ( userTable )

| **列名** | vipNo | vipName | sex | age | cardDate | phone | heigh | weight |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | VIP卡号 | 姓名 | 性别 | 年龄 | 注册时间 | 手机号码 | 身高(cm) | 体重(kg) |
| **数据类型** | String | String | String | int | Date | String | int | double |
| **约束** | PK , NotNull | NotNull | NotNull | - | - | - | - | - |


2. 员工表 ( workerTable )

| **列名** | workerNo | name | sex | age | hiredate | phone | position | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 职位 | 备注信息 | 密码 |
| **数据类型** | String | String | String | int | Date | String | String | String | String |
| **约束** | PK , NotNull | NotNull | NotNull | - | - | - | - | - | NotNull |


3. 管理员表 ( adminTable )

| **列名** | workerNo | name | sex | age | hiredate | phone | position | info | pwd |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 工号 | 姓名 | 性别 | 年龄 | 入职时间 | 手机号 | 职位 | 备注信息 | 密码 |
| **数据类型** | String | String | String | int | Date | String | String | String | String |
| **约束** | PK , NotNull | NotNull | NotNull | - | - | - | - | - | NotNull |


4. 器材分类表( equipmentTable )

| **列名** | eNo | name | number |
| :----: | :----: | :----: | :----: |
| **说明** | 器材分类编号 | 器材名称 | 器材数量 |
| **数据类型** | String | Strinhg | int |
| **约束** | PK , NotNull | NotNull | NotNull |

5. 器材状态表 ( eqSatatusTable)

| **列名** | statusNo | status | eNO |
| :----: | :----: | :----: | :----: |
| **说明** | 器材编号 | 可选状态：broken,repair,usage,unable | 器材编号(分类) |
| **数据类型** | String | String | String |
| **约束** | PK , NotNull | NotNull | NotNull |


6. 可选课表( classTable )

| **列名** | classNo | name | workerNo | classTime | classDate | price |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **说明** | 课程编号 | 课程名 | 上课教师工号 | 课时 | 课程开始时间 | ¥价格(单位：分) |
| **数据类型** | String | String | String | int | Date | int |
| **约束** | PK , NotNull | NotNull | NotNull | - | - | - |


7. 会员选课表( courseScheduleTable )

| **列名** | csNo | classNo | vipNo | time |
| :----: | :----: | :----: | :----: | :----: |
| **说明** | 选课编号 | 课程编号 | vip卡号 | 选课时间 |
| **数据类型** | String | String | String | Date |
| **约束** | PK , NotNull | NotNull | NotNull | - |
