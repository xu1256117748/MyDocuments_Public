
## 前言  

&emsp;&emsp;**总仓库大小:** 一个账号下的所有仓库大小之和   
&emsp;&emsp;**单仓库数量:** 一个账号下单仓库数量之和   
&emsp;&emsp;**单仓库大小:** 创建的一个项目/仓库,该项目/仓库允许存储的大小  
&emsp;&emsp;**单文件大小:** 单仓库内允许上传的单个文件的大小   

## 先上结论:  

|                      | GitHub                                                       | gitee社区版<br/>(开源项目) | gitee社区版<br/>(个人私有仓库) | gitee企业版<br/> (免费版) | gitee企业版<br/> (协作开发) |
| -------------------- | ------------------------------------------------------------ | :------------------------: | :---------------------------: | :-----------------------: | :-------------------------: |
| 1.总仓库大小限制     | 无限制                                                       |             5G             |              5G               |            5G             |          20 ~ 100G          |
| 2.单仓库数量限制     | 无限制                                                       |            1000            |             1000              |            ━━━            |             ━━━             |
| 3.单仓库大小限制     | 理想推荐 < 1 G  <br/>强烈建议 < 5 G <br/>                    |             1G             |             500M              |           500M            |           1 ~ 3G            |
| 4.单文件大小限制     | < 100 M  <br/>通过git推送,单文件< 100 M <br/>通过git推送,可添加 50 MB - 100 M 的文件,但会收到警告 <br/>通过浏览器上传,单文件< 25 M |            50M             |              50M              |           100M            |         100 ~ 300M          |
| 5.附件总容量         | ━━━                                                          |             3G             |              3G               |            3G             |         10 ~ 50G +          |
| 6.单仓库附件总容量   | ━━━                                                          |             1G             |              1G               |            ━━━            |             ━━━             |
| 7.附件单文件大小上限 | ━━━                                                          |            100M            |             100M              |            ━━━            |             ━━━             |

```中文
ps: gitee下的 ━━━ 仅代表没找到相关数据,不表示没有限制
```

## 一、关于GitHub的总仓库/单仓库/单文件大小限制  
  (以下为百度翻译结果,原文地址: [https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github) )  
#### &emsp;&emsp;1.关于GitHub的大小限制(总仓库)  
&emsp;&emsp;&emsp;&emsp;GitHub试图为所有Git存储库提供充足的存储，尽管文件和存储库大小有严格限制。   
&emsp;&emsp;&emsp;&emsp;为了确保用户的性能和可靠性，我们积极监控整个存储库运行状况的信号。  
&emsp;&emsp;&emsp;&emsp;存储库健康状况是各种交互因素的函数，包括大小、提交频率、内容和结构。  
#### &emsp;&emsp;2.文件大小限制(单文件大小限制)  
&emsp;&emsp;&emsp;&emsp;**GitHub限制存储库中允许的文件大小。  
&emsp;&emsp;&emsp;&emsp;如果您试图添加或更新**大于50 MB** 的文件，您将收到Git的**警告**。这些更改仍将成功地推送到您的存储库中，但您可以考虑删除提交以将性能影响降至最低。  
&emsp;&emsp;&emsp;&emsp;注：如果通过 **浏览器** 将文件添加到存储库中，则文件大小不能超过**25 MB**  。  
&emsp;&emsp;&emsp;&emsp;**GitHub阻止大于100 MB的文件。**  
&emsp;&emsp;&emsp;&emsp;要跟踪超出此限制的文件，必须使用Git大文件存储（Git LFS）。有关详细信息，请参阅 关于Git大文件存储  
&emsp;&emsp;&emsp;&emsp;如果需要在存储库中分发大型文件，可以在GitHub.com上创建版本，而不是跟踪文件。有关详细信息，请参阅 分发大型二进制文件  
&emsp;&emsp;&emsp;&emsp;**Git不是为处理大型SQL文件而设计的。** 要与其他开发人员共享大型数据库，我们建议使用 升降箱  
#### &emsp;&emsp;3.存储库大小限制
&emsp;&emsp;&emsp;&emsp;我们建议存储库保持较小，理想情况下小于1 GB，强烈建议小于5 GB。较小的存储库克隆速度更快，使用和维护更容易。    
&emsp;&emsp;&emsp;&emsp;如果您的存储库过度影响我们的基础架构，您可能会收到GitHub支持部门的电子邮件，要求您采取纠正措施。  
&emsp;&emsp;&emsp;&emsp;我们努力保持灵活性，尤其是对于有许多合作者的大型项目，我们将尽可能与您合作，以找到解决方案。  
&emsp;&emsp;&emsp;&emsp;通过有效管理存储库的大小和总体运行状况，您可以防止存储库影响我们的基础架构。您可以在中找到用于存储库分析的建议和工具github/git-sizer存储库  
&emsp;&emsp;&emsp;&emsp;外部依赖性可能会导致Git存储库变得非常大。为了避免使用外部依赖项填充存储库，我们建议您使用包管理器。  
&emsp;&emsp;&emsp;&emsp;常见语言的流行包管理器包括捆扎机 ,节点的包管理器、和马文这些包管理器支持直接使用Git存储库，因此您不需要预先打包的源。  
&emsp;&emsp;&emsp;&emsp;**Git不是作为备份工具设计的。** 然而，有许多专门为执行备份而设计的解决方案，例如Arq公司 ,碳酸盐岩、和碰撞计划 .  
## 二、关于Gitee的总仓库/单仓库/单文件大小限制  
(以下为gitee官方文档数据链接:  
[https://gitee.com/help/articles/4125#article-header0](https://gitee.com/help/articles/4125#article-header0)
)

#### &emsp;&emsp;1. 社区版配额说明

|   类型   | 说明                                                         |
| :------: | ------------------------------------------------------------ |
| 仓库数量 | 创建 1000 个仓库，不限制公私有。                             |
| 仓库容量 | 单仓库大小上限为 500M 单文件最大 50M 用户总仓库容量为 5G 注：总仓库定义为用户名下以及所创建的组织下面的所有仓库。 |
| 附件容量 | 附件单文件大小上限为 100MB 单仓库附件总容量 1G               |
| 成员人数 | 公有仓库成员数量不限。 个人账号下所有私有仓库总的协作人数为 5人 |

#### &emsp;&emsp;2.企业版和社区版服务对比

|   功能特性   |  社区版  |    社区版    | 企业版 |    企业版    |
| :----------: | :------: | :----------: | :----: | :----------: |
|   使用场景   | 开源项目 | 个人私有仓库 | 免费版 |   协作开发   |
| 总计协作人数 |   不限   |    ≦ 5 人    | ≦ 5 人 | 20 ~ 100 人+ |
|  仓库总容量  |    5G    |      5G      |   5G   |  20 ~ 100G   |
|  单仓库大小  |    1G    |     500M     |  500M  |    1 ~ 3G    |
|  单文件大小  |   50M    |     50M      |  100M  |  100 ~ 300M  |
|  附件总容量  |    3G    |      3G      |   3G   |  10 ~ 50G +  |

