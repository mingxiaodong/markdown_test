> 微信公众号：**[HEMLab]**
> 关注水灾害、山地灾害模拟及风险评估。问题或建议，请公众号留言。
HEMLab团队在Water Resources Research发表新成果：基于二维高性能水动力模型和数值天气预报的实时洪水预报系统
![封面图片](https://github.com/mingxiaodong/markdown_test/blob/master/Paper_preview.png)

### HEMLab 出品：全流域-高精度-实时洪水预报系统
洪水预报系统一般至少包括天气预报和洪水模拟两个模块。当前大部分预报系统的洪水模拟模块依赖于水文模型或者水文与水动力耦合模型，往往简化或者不考虑洪水演进的动力过程。当面对极端降雨导致、伴随着高速地表径流的洪水时，忽视洪水动力机制而过多依赖经验参数可能会使模拟失准。本研究基于最新开发的高性能二维水动力学模型HiPIMS模型，结合英国气象局提供的数值天气预报，开发出一套实时洪水预报系统（图1），能够提供高精度、长预报时间和全流域的洪水水深和淹没范围预报结果。
![图一](https://github.com/mingxiaodong/markdown_test/blob/master/Figure%201.png)
图1. 洪水预报系统框架

该系统应用于流域面积为2500平方公里的英国Eden流域，以2015年12月的一次极端洪水事件为例，成功验证了其提前34小时发布10m精度的精确洪水淹没预报的能力*。该预报包含覆盖洪水事件全时段和整个流域空间的淹没深度（图2）和水流流速，并与观测数据进行了对比（表1），具有较高的准确度和时效性。
*采用服务器 8×NVIDIA Tesla K80 GPU

![图二](https://github.com/mingxiaodong/markdown_test/blob/master/CA1_4map.png)
图2. 不同时段的洪水淹没深度及范围预报

表1. Carlisle市中心区域的淹没范围预报表现（基于2m×2m网格）
Total cells|Hits|Misses|False alarms|Correct negatives|POD|FAR|CSI
-----------|----|------|------------|-----------------|---|---|---
105583|24369|249|9644|71321|0.99|0.28|0.71

本研究具有以下亮点：
* 基于全水动力学模拟和数值天气预报的高精度实时预报系统
* 通过多GPU加速技术实现流域级别的二维水动力学洪水模拟
* 该系统应用于流域面积为2500平方公里的英国Eden河流域，以2015年12月的一次极端洪水事件为例，成功验证了提前34小时发布精确洪水淹没预报的能力。

该论文由HEMLab研究团队明晓东博士、梁秋华教授和夏熙临博士联合发表在水资源顶级期刊**Water Resources Research**上：
Ming, X., Liang, Q., Xia, X., Li, D., & Fowler, H. J. (2020). [Real‐time flood forecasting based on a high‐performance 2D hydrodynamic model and numerical weather predictions.](https://doi.org/10.1029/2019wr025583) Water Resources Research.

敬请登陆我们的网站[https://www.hemlab.org], 或者通过我们的微信公众号，关注我们的最新研究。
![qrcode](https://github.com/mingxiaodong/markdown_test/blob/master/HEMLab_Wechat_QRcode.jpeg)
