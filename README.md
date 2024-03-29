# -鸡蛋反向3,3模型合约

那因为要介绍反向3.3，所以我们先介绍一下什么是正向3，3， 曾经爆火的 $OHM 就是最成功的例子。

<h3>1：正向3，3</h3>
可以简单理解为：你不卖，你手上的token数量会增多。同时，因为大家都不卖，只囤币，token的价格也不断升高。

<h3>2:那反向3，3是什么？</h3>
可以理解为如果你买了 $eggs 但是什么也不做，你手上token的数量会越来越少。除非把它存在金库里保管起来也能保护数量不变。

我们来看一下 $OHM 巅峰时期的形态，就可以看到这种ponzi模型的力量所在。
![image](https://user-images.githubusercontent.com/75075562/222878222-eacb4481-d366-458a-b5eb-4dd71e4f336e.png)

初始代币数量为： 3,324,324,324,357（已经燃烧了一半左右）

每区块都会0.001% 的Eggs都会被debase，也就是一天减少7% . 但是存LP的奖励，每个区块有10,000,000 EGGS 的奖励。


<h3>风险提示和反思</h3>
其实本质上，项目还是采取减少流通量、锁仓和吸引新人拉高币价来吸引更多人玩这个游戏。

这样一看就是一个击鼓传花的游戏。不过因为最初我也是这么看待 $OHM 而错过千倍项目，这次决定把它当作一个社会性实验，看看他能走到何方。

# Eggs.sol  鸡蛋代币合约


# EggsFullProtec.sol  质押合约
Full protec vault ：有7天的锁仓期，但是可以完整保护你蛋的数量不变。

# EggChef.sol  质押合约
1：Big protect vault earns ：从Eggs/ETH 的LP收益中提取9/10的收益补偿
2：Smol proect vault earns ：从Eggs/ETH 的LP收益中提取1/10的收益补偿

#简介
一个通缩的模型产生了。我们假设有一部分人不存进 Full protec vault，那 $Eggs 的数量就会不断减少。
