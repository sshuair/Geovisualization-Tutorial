本实践中，我们将复现[Wikipedia 2016年美国大选](https://en.wikipedia.org/wiki/2016_United_States_presidential_election)的一幅插图:

![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/ElectoralCollege2016.svg/1600px-ElectoralCollege2016.svg.png)


### 文件说明
- USA-election-2016.geojson: 数据文件
- USA-election-2016.qgz: QGIS3的工程文件
- USA-election-2016.qgs: QGIS2的工程文件

### 样式配置
1. 符号化：分类图
   1. 列：winner
   2. 边线颜色：白色  #ffffff  (R:255 G:255 B:255)
   3. 颜色
       - Clinton: #6a8ec3 ( R:106 G:142 B:195 )
       - Trump:   #ee7867 ( R:238 G:120 B:103 )
2. 标签(label)
   1. 字段: electoral_votes
   2. 标签大小：15
   3. 标签颜色：黑色
3. 投影: EPSG:102008(North_america_Albers_Equal_Area_Conic)
