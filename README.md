# 构建可信软件系统的 10 要素【草稿】

上周，我听公司的咨询同事讲到一个非常有趣的观点：

 - 为什么微服务成本很高，要将单体应用改成微服务？
 - 为什么中台并不能解决问题，但是还是要做中台？
 - 为什么微前端不是银弹，但是我们仍然想做微服务？
 - ……

『因为代码写得烂吧，质量上不去，自然需要找个**好的理由**来重写应用』。旧的代码不好维护，只是其中的一个理由。现在，加上了新的技术、新的架构，已然变成了两个理由了，也就是一个好的理由。

所以，我又想重新思考一下，如何在这方面做得更好。

## 1. 清晰明确的架构远景

白板 + C4Model


相关资源：

 - 《[如何做技术规划？](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652976331&idx=1&sn=cb60a2b5eee408a509457ff1904da3c9&chksm=bd4ae7e88a3d6efe8457ee4f7df49744a0ba4c9dfdc62d37a52468ce96a7f7ad4a1fd42afd90&token=2048156466&lang=zh_CN#rd)》

## 2. 风格受限的代码规范

清晰整洁的软件代码

我们使用各种 Lint 各种工具

但是我们并没有使用全部力气来做这样的事情，短的函数（如 30 行内，Java 这一类繁琐的语言另说）

相关资源：

 - 《[技巧 - 如何好一个 Git 提交信息及几种不同的规范](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652975108&idx=1&sn=a07a27fd79b309b28a3d9ca78066699b&chksm=bd4ae3278a3d6a31570e7330278998b3864db5314e291abb037945e9b5227c5cf2c3cee5d440&token=2048156466&lang=zh_CN#rd)》
 - 《[五个简单的原则，带你写出整洁代码](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652976116&idx=1&sn=18246a013bce2fbe5fdd1471ef0588c0&chksm=bd4ae0d78a3d69c1850b862f270a6b19c659a46aeff3fe080f4d55b759b7d12eb0ada41746d0&token=2048156466&lang=zh_CN#rd)》

## 3. 自动守护的分层架构

 - ArchUnit

架构守护，


## 4. 人机共存的代码检视

人都是不靠谱的。而对于 Code Review 这种团体活动来说，人越是多，那么反而 review 的效果就不上去。


相关资源：

 - 《[软件工程在工作中的作用](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=404975336&idx=2&sn=d6a07bbfcf12059272ab50a7c7e4e787&chksm=3b48bdcb0c3f34dde39fd77e24bf64bd03573ef720bf0ceb9f5304a9ebd404ac10a193dddb9f&token=2048156466&lang=zh_CN#rd)》


## 5. 测试保证的关键逻辑

测试会带来成本，但是会提升软件质量。

相关资源：

 - 《[如何用测试驱动出100%测试覆盖率的代码](https://www.phodal.com/blog/use-tdd-drive-100-percent-test-coverage/)》
 - 《[【架构拾集】——移动应用的自动化测试（BDD 方式）](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652976100&idx=1&sn=748bc637621781fcb7d2ddb7e69bb722&chksm=bd4ae0c78a3d69d12f523cf57d636eefabdc0ae8def2c943df3533036ac397f0d9ebbc2d86fc&token=2048156466&lang=zh_CN#rd)》
 - 《[哪个才是最适合你的 Web UI 自动化测试框架](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652975411&idx=1&sn=112197e48b560280813f09a534db3420&chksm=bd4ae2108a3d6b068099f230f775571d0760efae10261e16a818ee251a76f3c5666fd5880bc3&scene=21#wechat_redirect)》
 - 《[如何提升 Web 应用的代码质量](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652975940&idx=1&sn=434fdeafef4fbee7047a3dfae7f8dee9&chksm=bd4ae0678a3d6971cf992fdfd2125a11a7f5f7d80d5bfabf529a7ba545e9a74550bffb11807a&token=2048156466&lang=zh_CN#rd)》

## 6. 工具约束的开发流程

人都是不可信的。所以，在我最近经历的项目中，都无一例外地引入  pre-push，pre-commit 这样的流程，但是它仍然是可以跳过的。

## 7. 动态更新的文档策略

文档是最

Path to Production + ADR + Wiki 


相关资源：

 - 《[如何优化上线流程——Path to Production](https://www.phodal.com/blog/tech-lead-tools-path-to-production/)》
 - 《[使用 adr 轻松创建 “程序员友好” 的轻量级架构决策记录](https://www.phodal.com/blog/use-adrjs-create-documenting-architecture-decisions/)》
 - 《[【架构拾集】基于 Markdown 文档展示系统设计](https://www.phodal.com/blog/architecture-in-realworld-markdown-based-document-system-design/)》

## 8. 独立巧妙的系统划分

单体应用正在杀死

我本是想说微服务，可微服务只是划分方式的一种，

## 9. 持续偿还的技术债务

相关资源：

 - 《[从遗留技术栈升级里，我学到的八件事](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652975728&idx=1&sn=1d897c401be9e9b213abdae933a4e913&chksm=bd4ae1538a3d6845b338364d89e2857a0e5d6376f13eb81bf5786b5011ee850dc2e7689fc638&token=2048156466&lang=zh_CN#rd0)》
 - 《[【代码范式集】：使用 “IDE 重构” 改善代码质量](https://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652976179&idx=1&sn=c0a2b647341d1c4310f887a2d22fc265&chksm=bd4ae7108a3d6e061dd17c059e120d2506fb06e657140157c2b6684c4f01a6a69b2f286c0c02&token=2048156466&lang=zh_CN#rd)》
 - 《[管理依赖的 11 个策略](https://www.phodal.com/blog/dependency-management-strategy/)》

### 与时俱进的依赖更新

## 10. 强有力的个人 & 愿意改进的团队

虽然我想说 KPI，但是 KPI 反而是有害的——上有政策，下有对策。只要了解或者是熟悉评分的标准，那么就可以有针对性的进行**负优化**，比如说用代码行数来评定绩效。

相关资源：

 - 《[迈向 Tech Lead 之路](https://www.phodal.com/blog/path-to-tech-lead/)》
 
## 其它

### 如何启动项目

相关资源：

 - [新项目检查清单](https://www.phodal.com/blog/new-project-check-lists/)
 - [如何创建你的应用脚手架](https://www.phodal.com/blog/how-to-create-application-boilerplate/)


## 结论

不过，话说回来，国内的程序员便宜，所以架构并不是考量因素——并且找 10 个程序员来重写，反而比找一个优秀的程序员更加容易。可维护的架构也就没有成为国内程序员的挑战，业务的快速推进才是重中之中。但是呢，这个情况并不会再持续太久。

而无论怎样，好的架构都需要强有力的个人和愿意改进的团队。

