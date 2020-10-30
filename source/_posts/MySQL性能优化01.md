---
uuid: 6465a74d-5386-faca-2d5f-6988c2244af8
title: MySQL性能优化01：主题和目标
author: Lampkins
qrcode: true
share_menu: true
toc: true
donate: true
comments: true
date: 2020-10-23 17:32:30
categories:
- 数据库
- MySQL性能优化
tags:
- MySQL
- 索引
---

MySQL课程主题和目标

## 主题：

你真的会使用MySQL索引进行性能优化吗?

-----

## 目标

1. 性能分析要从三驾马车开始(慢查询日志、**explain执行计划**、 show profile )

2. 有了性能分析报告，接下来如何对性能进行优化呢？

3. **我们一定要搞清楚通过explain显示查询计划中关于索引是否被用到**

   ```sql
   -- id是主键
   -- name是非唯一索引
   -- MySQL在执行查询时一般只会用到一个索引（优化器去进行选择）
   select * from user where id = 1 and name= 'zhangsan'
   ```

   

4. **你知道MySQL的索引在执行过程中是如何被使用的吗？**

5. **你知道MySQL中的表数据和索引在底层是如何存储的吗？**

6. 你了解聚集索引（ IOT索引组织表）和非聚集索引（堆组织表）的存储方式的不同吗？

7. 你知道聚集索引中的主键索引和辅助索引是如何存储索引和数据的吗？

8. 你会正确使用组合索引吗？

9. 你明白最左前缀原则是怎么回事吗？

10. 你明白什么是索引覆盖吗？索引覆盖如何优化检索性能？

11. **如何正确使用索引，才不会引起索引失效？**

---

> [MySQL性能优化01：主题和目标](http://lampkins.gitee.io/2020/10/26/MySQL性能优化01/)
>
> [MySQL性能优化02：MySQL架构篇](http://lampkins.gitee.io/2020/10/26/MySQL性能优化02/)
>
> [MySQL性能优化03：MySQL性能分析篇](http://lampkins.gitee.io/2020/10/26/MySQL性能优化03/)
>
> [MySQL性能优化04：MySQL索引篇01索引讲解](http://lampkins.gitee.io/2020/10/26/MySQL性能优化04/)
>
> [MySQL性能优化05：MySQL索引篇02查看执行计划](http://lampkins.gitee.io/2020/10/26/MySQL性能优化05/)
>
> [MySQL性能优化06：MySQL索引篇03索引失效分析](http://lampkins.gitee.io/2020/10/26/MySQL性能优化06/)
>
> [MySQL性能优化07：性能优化篇](http://lampkins.gitee.io/2020/10/26/MySQL性能优化07/)