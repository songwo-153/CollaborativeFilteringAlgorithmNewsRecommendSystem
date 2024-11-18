# 基于协同过滤算法的个性化新闻推荐系统
# Collaborative Filtering News Recommend System Online
 基于协同过滤算法的个性化新闻推荐系统的设计与实现（采用Java语言的SSM框架实现基于用户、物品的协同过滤推荐算法）实现了UserCF和ItemCF的协同过滤推荐算法。
Java语言（SSM框架）实现协同过滤算法新闻推荐系统，使用**基于用户、物品的协同过滤推荐算法**通过**python爬虫**爬取环球日报新闻实现**实时计算推荐**。
**源码获取**：[基于协同过滤算法新闻推荐系统源码.zip](https://github.com/songwo-153/CollaborativeFilteringNewsRecommendSystem/files/13557079/default.zip)
**开发工具**：IDEA，jdk1.8，Mysql8，navicat数据库管理工具，Tomcat，Maven.
**后端使用**：SSM(Spring+SpringMVC+Mybatis)开发框架。
**前端使用**：javascript脚本，jquery脚本，用户端使用bootstrap前端框架，管理员端使用layui前端框架，layer弹窗组件等。
# 功能实现
**系统前台**：用户具有注册、登录、注销、浏览新闻、搜索新闻、信息修改、密码修改、喜好标签、新闻评分、新闻收藏、新闻评论、排行榜、热点推荐、个性化推荐新闻等功能；
**后台管理系统**：管理员可以查看数据统计、用户管理、新闻管理、新闻类型管理、评分管理、收藏管理、评论管理、浏览记录管理、用户喜好标签等。
**协同过滤推荐功能**：
 1. **热点榜单**
	 根据数据库的新闻数据查询浏览数量最多的新闻进行推荐，同时查询出来的是不包括当前登录用户已经浏览过的新闻（过滤当前用户已经浏览过的新闻）；
 2. **个性化推荐**
    2.1. 游客：根据新闻总评分和总收藏数量降序查询输出向游客推荐。
    2.2. 登录用户：
    **基于用户的协同过滤推荐算法**：根据新闻的评分数据采用基于用户的协同过滤推荐算法实时计算向用户进行新闻推荐；如果没有推荐结果，采用根据登录用户选择的喜好标签下的新闻的总评分降序推荐，同时推荐的新闻是过滤掉当前登录用户已经评分过的新闻；
   **基于项目的协同过滤推荐算法**：根据新闻的收藏数量采用基于项目的协同过滤推荐算法从高到低降序向用户进行推荐；如果没有推荐结果，采用根据登录用户喜好标签下的新闻的收藏数量降序推荐，同时推荐的是当前登录用户没有收藏过的新闻。
 3. **相关推荐**：
     推荐当前登录用户正在浏览的新闻相同类型下评分较高的新闻，同时推荐的是当前用户没有评分的新闻。
**新闻数据来源**：
     爬取环球日报新闻数据  

**源码获取：**[基于协同过滤算法新闻推荐系统源码.zip](https://github.com/songwo-153/CollaborativeFilteringNewsRecommendSystem/files/13557079/default.zip)
![image](https://github.com/user-attachments/assets/bfcbe910-6127-45ce-97c3-59a16cc3b36a)

**项目结构**

**前台系统**
![输入图片说明](%E6%96%B0%E9%97%BB%E9%A6%96%E9%A1%B5.jpg)
![输入图片说明](Inked%E6%96%B0%E9%97%BB%E6%9F%A5%E7%9C%8B.jpg)
![输入图片说明](%E6%B3%A8%E5%86%8C.jpg)
![输入图片说明](%E9%80%89%E6%8B%A9%E5%85%B4%E8%B6%A3%E6%A0%87%E7%AD%BE.jpg)
![输入图片说明](%E4%B8%AA%E4%BA%BA%E4%B8%AD%E5%BF%83.jpg)
**后台管理系统**
![输入图片说明](Inked%E6%96%B0%E9%97%BB%E7%AE%A1%E7%90%86.jpg)
**协同过滤推荐算法**
![输入图片说明](%E5%8D%8F%E5%90%8C%E8%BF%87%E6%BB%A4%E6%8E%A8%E8%8D%90.jpg)
**Python爬取环球网新闻**
![输入图片说明](Pythom%E7%88%AC%E5%8F%96%E7%8E%AF%E7%90%83%E7%BD%91%E6%96%B0%E9%97%BB%E6%95%B0%E6%8D%AE.png)           
**源码获取**：[基于协同过滤算法新闻推荐系统源码.zip](https://github.com/songwo-153/CollaborativeFilteringNewsRecommendSystem/files/13557079/default.zip)



