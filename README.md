# DM_Anomaly-Detection

目標：實現一個異常檢測模型，使用Letter Image Recognition Data Set中的特徵數據，識別測試集中隨機加入的異常樣本

模型：KNN

準確度：97.9%

input(training.csv)：
- lettr: 字母標籤（A到Z）
- x-box: 矩形框的水平位置（整數）
- y-box: 矩形框的垂直位置（整數）
- width: 矩形框的寬度（整數）
- high: 矩形框的高度（整數）
- onpix: 矩形框內的on像素總數（整數）
- x-bar: 矩形框內on像素的x坐標均值（整數）
- y-bar: 矩形框內on像素的y坐標均值（整數）
- x2bar: x方向方差（整數）
- y2bar: y方向方差（整數）
- xybar: x和y的相關性（整數）
- x2ybr: xxy的均值（整數）
- xy2br: xyy的均值（整數）
- x-ege: 左到右的邊緣計數均值（整數）
- xegvy: x-ege與y的相關性（整數）
- y-ege: 底到頂的邊緣計數均值（整數）
- yegvx: y-ege與x的相關性（整數）

測試數據（test_X.csv）：
- 列名：與訓練數據相同，但不包含字母標籤
- 數據特徵：包含600個來自訓練集中6個字母的樣本，另外再隨機加入400個其他字母的樣本，共1000個樣本
