这个实战教程，我们会尝试用QGIS去复现[The Migrants’ Files: Surveying ­migrants’ deaths at Europe’s door](http://www.themigrantsfiles.com/)中的一幅图。该作品获得2014年[DATA JOURNALISM AWARDS](https://www.datajournalismawards.org/past-winners/)和2015年[European Press Prize](https://www.europeanpressprize.com/shortlists/year-2015/)两个大奖。


![migrants_photo](./assets/migrants_files.jpeg)

### 文件说明
- USA-election-2016.geojson: 数据文件
- migration.qgz: QGIS3的工程文件
- migration.qgs: QGIS2的工程文件

## 颜色配置：
## 1. world country图层
1. 渲染方式：单一符号
2. 填充样式：
    - 颜色：#fafaf8
    - 轮廓：#bdaeaf

### 2. migrants file图层
1. 渲染方式：渐进样式
2. 渐进字段（列）：deaths
3. 符号：
   - 颜色填充：#850200
   - 轮廓：无填充
4. 显示方法：size
5. 大小 从：1~18
6. 分段数量：25
7.  分段方法：手动分段
```
0~1
1~5
5~10
10~20
20~30
30~40
40~50
50~90
90~130
130~210
210~290
290~370
370~450
450~610
610~690
690~770
770~1000
1000~1250
1250~1500
1500~1750
1750~2000
2000~2500
2500~3000
3000~3840
3840~29986
```
8. 要素混合：叠层

## 背景颜色
菜单栏`项目`-->`属性`-->`通用`-->`Background color`
1. 渲染颜色：#c2c9d1