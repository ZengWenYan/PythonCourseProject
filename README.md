## 项目名称：中国企业招聘教育岗位数据分析
谁能分得国内企业教育岗位的一杯羹？通过对中国猎聘网爬取的数据分析国内应聘教育岗位的市场环境及对于应聘能力的研究，为有意向从事教育岗位或者正在从事教育岗位的人员提供参考。
* [项目pythonanywhere部署报告](http://littlelucaszy.pythonanywhere.com/)

## 问题表述：
### 1.项目为啥要做？
随着国家发展对于教育的越发重视，企业中教育岗位的也正更新发展，在这样的大环境发展下，人才市场对于从事企业中的教育岗位有了更为强烈的需求。
### 2.是谁有需要解决的问题？
想要应聘国内教育岗位的人、需要了解国内企业教育岗位数据趋向的人（用户画像）
### 3.用户需求：
* 使用场景：高校师范类应届毕业生需要找第一份正式工作，希望能得到一份可靠的教育岗位分析数据
* 任务：快速得到一份国内企业应聘教育岗位的分析报告
* 痛点：网络相关讯息众多复杂，缺少了一份清晰简洁又专业的报告书
* 增长/益点：找到个城市教育岗位的数据情况、应聘要求
### 4.用户画像
![](https://images.gitee.com/uploads/images/2020/0723/231633_179c98b2_2230708.png)

## 解决方案表述
### 1.项目如何做分析？
* 先通过[中国猎聘网](https://www.liepin.com/city-gz/zhaopin/?init=1)收集相关的国内企业教育岗位的信息，并且收集到的数据做好数据清洗
* 首先从全局观出发做出大的教育岗位数量分布地区图，然后再通过同样的办法做出教育岗位相关的要求对比图，例如：学历要求、经验要求、语言要求、具体的职位要求。
* 最后结合数据呈现结果，综合从总体到局部去进行分析国内环境下应聘教育岗位的要求
### 2.项目结果解决了谁的问题？
解决了想要应聘国内教育岗位环境的人或者需要了解国内企业教育岗位人才需求数据趋向的人的问题
### 3.项目结果的设计思维部分：
* 商业可行性：企业/投资者可以为教育岗位市场与教育人才市场的关系进行战略调整；应聘者可以通过这一份数据进行自我未来规划和应聘策略。
* 技术可行性：利用中国猎聘网给予的开放数据进行挖掘后，可利用panadas、pyecharts完成数据清洗和图表制作。
* 用户可欲性：能够帮助该类用户解决实际应聘需求、招聘市场分析的考察。 

## 数据分析思路及方法
* 读出“猎聘教育相关岗位详情页.xlsx”表格

![](https://images.gitee.com/uploads/images/2020/0719/064847_233e3dcc_2230708.png)

* 清洗数据（工作城市栏位处理：筛选出包含下级区域城市-生成列表准备处理-利用for循环处理数据-数据原表替换-数据更新-进行分进合击）

![](https://images.gitee.com/uploads/images/2020/0719/064913_b5f443e9_2230708.png)

## 数据分析流程及成果
* 在分进合击之后，为了让求职者直观地了解到公司主要在哪些城市招聘，也可以了解到哪些城市缺乏教育的人才，同时也能查看到里边是否有自己的心仪的城市，甚至也能知道在教育这方面竞争的激烈程度制作了地图可视化。
![](https://images.gitee.com/uploads/images/2020/0719/070256_df44aefb_2230708.png)
* 在了解大环境后，为了让用户了解到不同因素（学历、经验、语言）对于国内应聘教育岗位的影响，分别制作了饼状图、玫瑰图、水滴图。
![](https://images.gitee.com/uploads/images/2020/0719/070309_169b70ee_2230708.png)
* 最后为了让用户对于应聘要求有更细节的了解，就运用主题建模的方式对其做了主题建模可视化。
![](https://images.gitee.com/uploads/images/2020/0719/070323_2fd2c043_2230708.png)


## 学习/实践心得总结及感谢
通过本次python语言课程的学习以及项目的实践，我意识到了对科学思维培养的重要性，并且学习到了有关python语言的一些基本运用。在此由衷感谢许智超老师的教学与指导；感谢中国猎聘网提供的数据；感谢jupyter notebook提供的技术平台支持。
