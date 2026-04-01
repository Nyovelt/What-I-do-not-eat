# What-I-do-not-eat

A repo which records my dietary habits

## Canarypwn's First Law of Food (食物第一定律)

如果一个东西很难吃，那么就不会流行。

Foods with poor taste do not achieve widespread prevalence.

## Canarypwn's Second Law of Food (食物第二定律)

当一个人年龄足够大的时候，他尝过大部分流行的食物。

A sufficiently aged individual has encountered the majority of prevalent foods.

## Theorem 1: Unfamiliar Foods Are Likely Unpalatable

推论一: 如果一个食物你没有见过，那么它大概率是不好吃的。

**Theorem.** Given the First and Second Laws, the posterior probability that an unfamiliar food is bad-tasting is high.

**Proof:**

Let $A$ denote the event that a randomly selected food is bad-tasting, and let $B$ denote the event that the individual has not previously encountered that food.

By Bayes' theorem:

$$P(A \mid B) = \frac{P(B \mid A) \cdot P(A)}{P(B)}$$

By the _First Law_, bad-tasting foods are not prevalent. Combined with the _Second Law_, an individual has encountered most prevalent foods. Therefore, bad-tasting foods are disproportionately represented among those not yet encountered, i.e., $P(B \mid A)$ is large.

Conversely, $P(B)$ is relatively small, since by the _Second Law_, the set of foods not yet encountered is a small fraction of all foods.

It follows that the ratio $\frac{P(B \mid A)}{P(B)}$ is large, and thus $P(A \mid B)$ is high. $\blacksquare$

**Remark (Exploration-Exploitation Tradeoff):**

为了避免错失美食，应该以适当的概率 $\varepsilon$ 来尝试未出现过的食物。

To avoid converging on a local optimum and missing undiscovered palatable foods, one should adopt an $\varepsilon$-greedy strategy: with probability $\varepsilon \in [0, 1]$, explore an unfamiliar food rather than exploiting known preferences. The parameter $\varepsilon$ may be tuned adaptively via reinforcement learning methods, e.g., [Monte Carlo Tree Search (MCTS)](https://en.wikipedia.org/wiki/Monte_Carlo_tree_search).

## What-I-do-not-eat

- 内脏 internal organs
  - 包括但不限于: 肠子, 心, 胃, 肾脏, 黄喉，脑子
  - including but not limited to: intestines, heart, stomach, kidney, pork aorta, brain
  - 例外 Exception: 血 Blood,
- 烤麸 baked wheat gluten (kaofu)
- 完整的芹菜 whole celery
  - 饺子馅豁免 exempt when used as dumpling filling
- 软体动物 mollusk
- 皮 skin
- 舌头 Tongue
- 仙人掌 cactus
- 杂碎 offal and miscellaneous trimmings
  - 牛筋 beef tendon
  - 淋巴 lymph node
- 爪子与蹄膀 feet and trotters
- 胶 gelatin / collagen
- 生殖器 genitals
- 秋葵 Okra
- 肥肉 fat
- 木耳 wood ear mushroom
- 难吃的粥 bad-tasting porridge
- 螺蛳粉 snail noodles
- 螺蛳 snail
- 莲 lotus
- 豆汁 soybean juice
- 炒肝 fried liver
- 苦瓜 bitter melon
- 毛蛋 fertilized duck egg

## What-I-prefer-not-to-have

- 骨骼惊奇的鱼, 复杂度超过鲫鱼的就算 fish with extraordinarily complex bones (anything worse than crucian carp)
- 除了面条以外的面条 non-wheat noodles (rice noodles, rice vermicelli, etc.)
  - 粉丝没问题 OK with fensi (glass noodles)
- 藕 lotus root
- 酸的水果 sour fruits

## Do not feed me with

- 大于10%酒精的饮料 beverages with over 10% alcohol

## About flavor

- 不能接受比`那么大鸡排`更辣的东西 cannot handle anything spicier than "Na Me Da Ji Pai" (a fried chicken cutlet brand)
