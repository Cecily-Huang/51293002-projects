# Project 2: Airbnb爱彼迎数据分析练习

## 概述

**这个项目重点考察循环、字符串处理、数值计算。**

数据科学能够帮助我们更好地去理解线上平台服务中的用户行为。这个项目是关于爱彼迎的房间信息的。从2008年开始，游客和房主都使用爱彼迎平台来拓展旅行的可能性，并呈现出更加独特、个性化的体验世界的方式。项目中的数据集描述了2019年纽约市的上市活动和指标。这个数据文件包含了所有需要的信息，以更好地了解房主、房间地理位置信息，及进行预测和得出结论的必要指标。你将需要使用Python的各种字符串操作函数来解决项目中提出的问题。  

在这个项目中，你将会处理airbnb.csv文件中的数据。  

请下载文件test.py, airbnb.csv, airbnb.ipynb以开始这个项目。你需要用Jupyter Notebooks打开airbnb.ipynb的文件以开始你的解答。你可以通过运行命令python test.py来测试你的代码。  

这个项目需要你通过写代码的方式回答20个问题。当你在notebook中的某一个cell中作答一个问题，请在该cell首行写注释，如你回答第十题，就在cell首行写注释“#Q10”，这样老师就能很清楚这个cell是回答哪一个问题的。  

## 问题

### Q1: 在airbnb.csv文件中有多少个neighborhood groups？
生成一个包含所有neighborhood groups的Python列表。不需要对列表中的名称排序，但是必须确保列表中的名称不重复。  
注意：在数据集中，有些数据是没有neighborhood groups信息的，缺失的值会用None表示，请不要讲None包含在答案中。

### Q2: 房间的平均价格是多少？
注意：有些行是缺失价格的，请跳过那些没有房间价格的数据，不要将其纳入平均值计算。

### Q3: 请计算neighborhood为“Chinatown”的房间数量。

### Q4: 请找出房间名包含“superbowl”（忽略大小写）的所有房间名称，并将结果保存在Python list中。

### Q5: 请找出房间名包含“dream room”（忽略大小写）的所有房间名称，并将结果保存在Python list中。

### Q6: 请找出房间名包含“free wifi”（忽略大小写）的所有房间名称，并将结果保存在Python list中。

### Q7: 请找出那些是“landeyo”的anagrams（相同字母异序词）的房主名字，并将结果保存在Python list中。
Anagrams指的是具有如下特性的两个单词：在这两个单词当中，每一个英文字母（不区分大小写）所出现的次数都是相同的。例如，“Unclear”和“Nuclear”、“Rimon”和“MinOR”都是Anagrams。  
提示：不需要用循环的方式解决这个问题，可以尝试写一些简洁的代码来解决这个问题，例如通过使用字符串的排序的操作。


### Q8: 请列出那些minimum nights大于365（minimum_nights > 365）的房间id，并将结果保存在Python list中。房间id用字符串类型表示。

### Q9: 请列出那些拥有超过50间房间（calculated_host_listings_count > 50）的房主id，并将结果保存在Python list中。房主id用字符串类型表示，请确保答案中不包含重复的id。

### Q10: 请列出在Brooklyn（neighborhood_group == "Brooklyn"）最便宜的房间名称，并将结果保存在Python list中。

### Q11: 请列出在Manhattan（neighborhood_group == "Manhattan"）最便宜的房间名称，并将结果保存在Python list中。

### Q12: 请计算评论次数与可用性的平均比率？（忽略availability_365为0的房间）计算结果为float类型。
提示1：分母为房间可用性列（即：availability_365列），分子为房间的评论次数列（即：number_of_reviews列）。  
提示2：你需要计算每个房间的评论次数与可用性的比率，然后再计算这些比率的平均值。 


### Q13:  请计算在纬度为40.50和40.75之间，经度为-74.00和-73.95之间（即：40.50 <= latitude <= 40.75, -74.00 <= longitude <= -73.95）的价格最便宜的房间id，并将结果保存在Python list中。

### Q14: 请计算在纬度为40.75和41.00之间，经度为-73.95和-73.85之间（即：40.75 <= latitude <= 41.00, -73.95 <= longitude <= -73.85）的价格最便宜的房间id，并将结果保存在Python list中。

### Q15: 请计算评论数超过300（number_of_reviews > 300）的房间的平均价格，结果用float类型表示。

### Q16: 请计算房价超过1000美元（price > 1000）的房间的平均评论数，结果用float类型表示。

### Q17: 请计算房间名包含“sweet”和“home”的房间数占房间名包含“sweet”的房间数的比例，结果用float类型表示。（忽略大小写）
提示：分母为房间名包含“sweet”的房间数，分子为房间名包含“sweet”和“home”的房间数。  

### Q18: 请计算房间名包含“pool”和“gym”的房间数占房间名包含“pool”的房间数的比例，结果用float类型表示。（忽略大小写）

### Q19: 请计算房间名包含“five”和“stars”的房间数占房间名包含“five”的房间数的比例，结果用float类型表示。（忽略大小写）

### Q20: 请计算以下费用：在Manhattan最贵的房间住最低限制晚数（minimum_nights）之后再在Brooklyn最贵的房间住最低限制晚数（minimum_nights）。

