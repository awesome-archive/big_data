## 通用技巧

[**过拟合**](#过拟合)

[**不平衡数据**](#不平衡数据)


### 过拟合
解决方法：<br>
1. 增加数据量<br>
2. 对W进行L1，L2正则<br>
3. 对于tree来说可以限制树的深度、leaf number、可以生成完完整的树以后进行trim；<br>
对于神经网络可以加dropout（input 0.8，hidden 0.5）

### 不平衡数据
解决方法：<br>
1. 尝试获取更多的数据（有时候只是因为前段时期的数据多半呈现的是一种趋势, 等到后半时期趋势又不一样了）<br>
2. 更换评判方式（不用accuracy和cost，用P&R即通过confusion matrix来计算precision和recall，然后通过precision和recall再计算f1分数）<br>
3. 重组数据（欠采样或过采样）<br>
4. 使用其他机器学习方法（比如不用神经网络，用决策树）
5. 修改算法



