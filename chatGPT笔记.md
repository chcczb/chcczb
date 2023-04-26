# 开发助手
## SQL书写
### 创建一个多表关联的查询语句
写一个sql语句 基表 decompost_budget_subject 别名s 关联 decompost_budget 别名m 关联条件 m.id = sub.decompostBudgetId 关联表 decompost_budget_activities 别名 act 关联条件 act.subjectId = sub.id 查询结果 uuid（） 返回唯一码作为ID s表查询 subjectCode subjectName act表查询 indicator 根据条件 当type等于01的时候 amount记为0 当是02的时候 记为amount 合计amount字段 按s表的type字段分组合计 返回结果进行非空判断   条件是s表ID 
![按要求输出一个sql](https://user-images.githubusercontent.com/130332194/234523584-224d7e09-1980-4a86-b8d3-f1f22a2baa0a.png)
