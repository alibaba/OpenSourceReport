2020 年微服务领域开源数字化报告

# 摘要
微服务体系就像是一剂催化剂，可以加速数据和业务结合的过程，更好地提升生产力，从而实现业务的提升。本项目旨在通过建立一份建立在微服务领域的相对完整、可以反复进行推演的数据报告（报告、数据、算法均开源），分析微服务框架项目以及 Spring Cloud 项目的 GitHub 开发者行为日志，通过多维度数据分析的视角，来观察微服务领域的开源现状、进展趋势、演化特征等问题。

本报告根据 2020 年 1 月到 6 月的 GitHub 日志进行统计。值得一提的是，报告显示 Apache Dubbo 作为中国本土开源的项目，在微服务框架中排名第5，全球排名跻身 693； Spring 社区第一个国产 Spring Cloud 项目 Spring Cloud Alibaba 作为开源的微服务全家桶，在 Spring Cloud 榜单中居于榜首。

关键词：微服务、开源、行为数据、GitHub

# 1.背景
随着业务的扩张，单体应用架构的开发、部署和运维都会越来越慢，越来越复杂，甚至在单体架构应用开发中敏捷模式无法施展开。基于此，具有更高独立性、可用性和弹性的微服务应运而生。从结构上看，微服务架构将一个应用拆分成多个松耦合的服务，这些服务之间通过某种协议（REST、rpc等）进行互相协作，完成原单体架构功能，但提供更灵活的部署模式，更容易扩展，降低了开发、运维上的复杂度。微服务的核心思想就是分而治之。微服务是商业应用程序发中最热门的新事物。微服务这个词取代了敏捷、DevOps 和 RESTful。

2020 年 7 月 O’Reilly 公布了一份关于企业微服务市场现状的数据调研。报告显示，在访问了全球 1,502 名软件工程师、系统和技术架构师、工程师以及决策者后，有 77％ 的组织反馈采用了微服务，其中 92％ 的组织成功使用了微服务。了解并分析微服务领域开源项目的发展，有助于掌握该领域的发展趋势，从而帮助提高企业的竞争力。

因此，进一步深入研究微服务领域的开源数字化现状具有非常重大的意义。

# 2.总体宏观统计结果
##Key Takeaways

- Quarkus 作为云原生微服务框架，在微服务框架中活跃度排名第一，全球 GitHub 开源项目活跃度中排名 40
- Spring 作为 Java 微服务框架事实标准，Spring Cloud 和 Spring Boot 项目在微服务框架中活跃度分别位列第二和第三
- Apache Dubbo 作为中国本土开源的项目，微服务框架活跃度排名第五，全球 GitHub 开源项目活跃度中排名跻身 693
- 在厂商 Spring Cloud 项目中，Spring Cloud Alibaba 活跃度排名第一

## 微服务框架榜单
根据附录中给出的项目活跃度定义，我们使用 2020 年 1 月～6 月的数据对微服务框架相关的项目及社区进行了活跃度的统计与排名，结果如下表所示，quarkusio/quarkus 项目、spring-cloud 社区、spring-projects/spring-boot 项目分别位于 Top1，Top2，Top3。需要注意的是，global_rank 是指该项目在全球 GitHub 开源项目中的活跃度排名。
![微服务.jpg](http://ww1.sinaimg.cn/large/7231c228ly1ghuszwy9b3j20ys0bamzs.jpg)
注： 表格中的developer是指执行了五种动作：Issue comment、Open issue、Open pull request、Pull reuqest review comment 和 Pull request merged的开发者

## Spring Cloud 榜单
根据附录中给出的项目活跃度的定义，我们使用 2020 年 1 月～6 月的数据对 Spring Cloud 项目进行了活跃度的统计与排名，结果如下表所示：
![spring cloud.jpg](http://ww1.sinaimg.cn/large/7231c228ly1ghuszjciihj210i07uwgc.jpg)

注： 表格中的developer是指执行了五种动作：Issue comment、Open issue、Open pull request、Pull reuqest review comment 和 Pull request merged的开发者

#3.展望
此次开源项目数据报告针对微服务领域的项目进行了研究，主要是提供了一些统计数据。未来，会对社区协作关系做可视化的呈现；在数据挖掘的层面，会基于真实数据挖掘数据背后的价值。希望报告所倡导的开源开放的业态有助于推动中国微服务领域的开源走向更深层次。

#4.致谢
本次报告由 X-lab 开放实验室撰写。
![xlab.png](http://ww1.sinaimg.cn/large/7231c228ly1ghusrgng3bj218x0jz3yn.jpg)
X-lab 开放实验室是由来自华东师范大学、同济大学的师生所构成的开放创新共同体，专业背景包括计算机科学、数据科学及其相关跨学科，长期思考并实践教育与开源两大主题。

#附录：数据集及方法
##数据集
时间
2020 年 1 月～2020 年 6 月
微服务框架数据
spring-cloud数据集
##活跃度计算方式
###（1）开发者活跃度
开发者活跃度，其定义为某特定 GitHub 账号在一段时间内在某特定 GitHub 项目中的活跃评价指标。其活跃度由该账号在该项目中的行为数据决定。本报告中所关心的行为包含如下几种：

- Issue comment：在 issue 中参与讨论是最基本的行为，每个评论计入 1 次。

- Open issue：在项目中发起一个 issue，无论是讨论、Bug 报告或提问，对项目都是带来活跃的，每个发起的 issue 计入 1 次。
- Open pull request：为项目提交一个 PR，表示已对该项目进行源码贡献，则每次发起一个 PR 计入 1 次。
- Pull reuqest review comment：对项目中的 PR 进行 review 和讨论，需要对项目有相当的了解，并且对项目源码的质量有极大帮助，每个评论计入 1 次。
- Pull request merged：若有 PR 被项目合入，即便是很小的改动，也需要对项目有较为深入的理解，是帮助项目进步的真切贡献，则每有一个 PR 被合入计入 1 次。
以上 5 个种行为在该报告模型中，具有不一样的权重，其加权值逐级增加，加权值分别为 1、2、3、4、5，即：

![开发者活跃度.png](http://ww1.sinaimg.cn/large/7231c228ly1ghusq7xbgdj215003wwel.jpg)


###（2）项目活跃度
项目活跃度，其定义为某特定项目在一段时间内的活跃评价指标。其活跃度由该段时间内在本项目中产生活跃的开发者活跃度加权计算得到，即：
![项目活跃度.png](http://ww1.sinaimg.cn/large/7231c228ly1ghusr513q2j20di04o3yb.jpg)
使用开方的加权方式，用于抹平因核心开发者活跃度过高而导致项目活跃度过高，在该计算方式下，活跃度计算方式对参与人数较多而活跃情况平均的项目更加友好。

本报告将周期性地更新，PDF版稍后将在公众号发布，欢迎关注
![云原生公众号.jpg](http://ww1.sinaimg.cn/large/7231c228ly1ghut7fegjbj206h06hjt0.jpg)
