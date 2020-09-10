# used_car
二手车交易价格预测
一、数据清洗
1、时间数据转换成：天/年
2、缺失值处理：使用XGT模型来预测缺失值
3、对非正态分布的数据进行log转换
4、对部分分类数据进行ONE-HOT转换
5、对异常值进行数据缩放
6、删除一些相关性低的指标
7、生成新特征：
8、标准化：由于部分数据已经进行了标准化处理，所以只能对个别指标单独处理
二、模型选择
1、lightgbm 单项得分最高
2、catboost
3、xgb效果不好
四、集成：
取Lgbm和catboost合成数，得分有提升
