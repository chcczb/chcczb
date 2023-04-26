# 开发助手
前后端工程存在私有库的问题，chatGPT在写代码时不会联系到上下文
## SQL书写
### 创建一个多表关联的查询语句
写一个sql语句 基表 decompost_budget_subject 别名s 关联 decompost_budget 别名m 关联条件 m.id = sub.decompostBudgetId 关联表 decompost_budget_activities 别名 act 关联条件 act.subjectId = sub.id 查询结果 uuid（） 返回唯一码作为ID s表查询 subjectCode subjectName act表查询 indicator 根据条件 当type等于01的时候 amount记为0 当是02的时候 记为amount 合计amount字段 按s表的type字段分组合计 返回结果进行非空判断   条件是s表ID 
![按要求输出一个sql](https://user-images.githubusercontent.com/130332194/234523584-224d7e09-1980-4a86-b8d3-f1f22a2baa0a.png)
## 后端新类和服务创建
### 创建一个数据库表相关的实体 my-batis  从controler iservice serviceimpl mapper po 
先指定它是一个什么类型的开发  以后输出的内容都将基于此实现
![写一个userPO类 添加简单的查询方法](https://user-images.githubusercontent.com/130332194/234562530-215bbe4c-9b54-4727-96f6-56f453d9a455.png)



# 文档助手
## 文档书写
### 写一份提纲
帮我写一份业务软件的立项材料 用markdown代码
![一个简单的文档提纲](https://user-images.githubusercontent.com/130332194/234549153-abf63892-6c5d-415e-87f8-e971b9a563d3.png)
### BUG分析报告
写一个BUG分析报告 内容为因为没有判断库存信息是否存在 下面代码中存在使用空指针情况 导致生产环境报错 
![BUG分析报告](https://user-images.githubusercontent.com/130332194/234550999-355d4e91-311d-4b32-98ae-85379255b39d.png)
