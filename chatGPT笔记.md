# 知识库
作为一个知识库，**它比百度优秀！**
不需要你在广告中分辨你想要的内容  

问百度你需要分辨出哪个是你要的
![image](https://user-images.githubusercontent.com/130332194/234740681-fe6ea905-af40-4176-be90-b3a8b71e645e.png)

问GPT更便捷一些
![chat-shot](https://user-images.githubusercontent.com/130332194/234740791-daff7ee9-ba82-4669-b688-ba3664de5bd3.png)
## 解决方案

### 写一个小脚本
怎么用bat文件做一个一键关机的脚本
![image](https://user-images.githubusercontent.com/130332194/234764830-b1096709-d1c9-4d8b-91ba-db19e1b76361.png)

加上可以中途取消的操作
![image](https://user-images.githubusercontent.com/130332194/234764883-8a8fb7e7-c346-4067-8eec-b9206b25dee7.png)
可以通过对话进行详细的内容追问和完善

### 针对两阶段机制 做提问
让他给你示例代码  在最后 它可以给你一些解释
![image](https://user-images.githubusercontent.com/130332194/234770962-c1b811ba-1b6b-4099-8a97-0698a885740f.png)



## 基础知识
### 问一个小知识
MathContext 的枚举值都是什么意思
![image](https://user-images.githubusercontent.com/130332194/234768993-7b318203-59df-4837-bce2-15d4a4acec9c.png)

你也可以让他针对你看不懂的地方 详细讲讲
![image](https://user-images.githubusercontent.com/130332194/234771112-468c8fc3-614a-4bc7-a21e-f72ce01194b1.png)
![image](https://user-images.githubusercontent.com/130332194/234771134-38a0e6e6-57d9-4aa9-a26b-866099588657.png)


# 开发助手
丑话说在前面（待补充）：
- 1 chatGPT在写代码时不会用到这些私有库的 可以通过一点点喂一个给gpt的方式使用  使用成本很高
- 2 涉及到商密的问题 不能把私有仓库喂给gpt
- 3 由于对话输入字数限制 你不能将你现有的复杂业务实现类一次性的喂给gpt  如果想改一部分内容 也有一个使用成本的问题
- 4 它有时会一本正经的胡说八道
- 5 当你纠正他时 他态度很好 但是不会坚持立场  你说什么就是什么  这会导致摄于你的局限性纠正了一个正确的方法

最好的方式：
**基于现阶段（我用的是GPT3.5）**
- 1 你将它作为**一个无情的写代码机器**  而你是**一个有感情的人**指挥机器实现你的想法 
- 2 你还需要是一个真正懂开发的人 在它给出代码时 审核它是不是胡说八道还是确实可用的代码
- 3 你的提问技巧很大程度上决定了它是否能准确理解

## SQL书写
### 创建一个多表关联的查询语句
写一个sql语句 基表 decompost_budget_subject 别名s 关联 decompost_budget 别名m 关联条件 m.id = sub.decompostBudgetId 关联表 decompost_budget_activities 别名 act 关联条件 act.subjectId = sub.id 查询结果 uuid（） 返回唯一码作为ID s表查询 subjectCode subjectName act表查询 indicator 根据条件 当type等于01的时候 amount记为0 当是02的时候 记为amount 合计amount字段 按s表的type字段分组合计 返回结果进行非空判断   条件是s表ID 
![按要求输出一个sql](https://user-images.githubusercontent.com/130332194/234523584-224d7e09-1980-4a86-b8d3-f1f22a2baa0a.png)

## 前端代码书写
### 前端从0开始
#### 写一个实际项目的代码
我想写一个查询窗口的前端代码，同时我要用的有一部分组件是私有库
接下来你要慢慢的**辅助它**进行代码编写， 说出你的想法 让它帮你完成
针对一些私有库你要知道怎么用了才能去并规定它怎么写，这还是有门槛的
![chat-shot (2)](https://user-images.githubusercontent.com/130332194/234776623-9a2a5a15-e9cb-43c4-babf-aa4586bdb238.png)

## 后端代码书写
### 后端新类和服务创建
#### 创建一个数据库表相关的实体 my-batis  从controler iservice serviceimpl mapper po 
先指定它是一个什么类型的开发  以后输出的内容都将基于此实现
![写一个userPO类 添加简单的查询方法](https://user-images.githubusercontent.com/130332194/234562530-215bbe4c-9b54-4727-96f6-56f453d9a455.png)

### 后端方法
#### 业务代码的校验和调优
一个生成计划明细的方法
![chat-shot](https://user-images.githubusercontent.com/130332194/234756074-78594dea-7437-4b87-9c59-dce9a8ddeee4.png)

### 帮忙写注释
![image](https://user-images.githubusercontent.com/130332194/234764121-cc12dbcf-1f77-433d-83c6-ef0d086f7ce9.png)

# 文档助手
## 文档书写
### 写一份提纲
帮我写一份业务软件的立项材料 用markdown代码
![一个简单的文档提纲](https://user-images.githubusercontent.com/130332194/234549153-abf63892-6c5d-415e-87f8-e971b9a563d3.png)
### BUG分析报告
写一个BUG分析报告 内容为因为没有判断库存信息是否存在 下面代码中存在使用空指针情况 导致生产环境报错 
![BUG分析报告](https://user-images.githubusercontent.com/130332194/234550999-355d4e91-311d-4b32-98ae-85379255b39d.png)


# 测试助手
## 测试用例
### 给定一个方法形成测试用例
Q:针对 createRollSale 这个后端方法 作为接口 写一份测试用例
A:好的，假设要测试 `createRollSale` 方法的正确性和完整性，可以根据以下情况编写测试用例：

1. 测试输入为空的情况：传入空的销售计划和明细列表，期望方法能够正常执行并返回。
2. 测试输入缺失必要参数的情况：例如不传入滚动周期 PO 对象 Map 或者组织名称等必要参数，期望方法抛出对应的异常或错误。
3. 测试输入数据规模较小的情况：例如传入少量的销售计划和明细数据，检查方法生成的滚动销售计划是否符合预期。
4. 测试输入数据规模较大的情况：例如传入大量的销售计划和明细数据，检查方法生成的滚动销售计划是否符合预期，并且检查方法执行时间是否合理。
5. 测试输入数据边界情况：例如传入指标类型下只有一个销售计划或只有一个销售明细，检查方法的输出结果是否符合预期，是否会出现异常。

这些测试用例可以以 JUnit 的形式编写，具体实现方式可以参考如下代码片段：

```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

public class ExampleTest {
    @Test
    public void testCreateRollSaleWithEmptyInputs() {
        // Arrange
        List<RollSaleVO> emptyList = Collections.emptyList();
        List<RollSaleDetailVO> emptyDetailList = Collections.emptyList();

        // Act
        createRollSale(emptyList, new RollSaleVO(), "orgName", emptyDetailList, new HashMap<>(),
                Collections.emptyList(), Collections.emptyList(), Collections.emptyList());

        // Assert
        Assertions.assertTrue(true, "Method should not throw any exception");
    }

    @Test
    public void testCreateRollSaleWithMissingInputs() {
        // Arrange
        List<RollSaleVO> emptyList = Collections.emptyList();
        List<RollSaleDetailVO> emptyDetailList = Collections.emptyList();

        // Act + Assert
        Assertions.assertThrows(IllegalArgumentException.class, () -> {
            createRollSale(emptyList, null, "orgName", emptyDetailList, new HashMap<>(),
                    Collections.emptyList(), Collections.emptyList(), Collections.emptyList());
        });
    }

    // .... 其他测试用例
}
``` 
由于我不了解您的具体业务和代码实现细节，以上只是一些简单的示例测试用例，您可以根据实际情况进行扩展和调整。







