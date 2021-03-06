# 温度、降水量与湿度系统

**温度、降水量与湿度系统（Environment System）**
是模组依于原版数据，引入的一套用于生存的数据系统。

![温度计、雨量计与湿度计](../.gitbook/assets/blocks-items/environment.png)

## 温度

在本系统中，根据原版生物群系数据，将温度划分为以下六个级别。（各群系默认温度数据在Minecraft Wiki中均可查询。）

| 编号 | 温度分级 | 英文 | 范围 |
|------|----------|------|------|
| 1 | 冰冻 | Freezing | (-∞, 0.15F] |
| 2 | 寒冷 | Cold | (0.15F, 0.3F] |
| 3 | 凉爽 | Cool | (0.3F, 0.5F] |
| 4 | 温暖 | Warm | (0.5F, 0.75F] |
| 5 | 炎热 | Hot | (0.75F, 1.5F] |
| 6 | 炙烤 | Heat | (1.5F, +∞) |

以上每一项与温度计的格子相对应，但温度计测量的是该区域的当前实际温度（随时间变化），而非群系默认温度数据。

## 降水量

在本系统中，根据原版生物群系数据，将降水量划分为以下五个级别。

| 编号 | 降水量分级 | 英文 | 范围 |
|------|----------|------|------|
| 1 | 罕见 | Rare | (-∞, 0.1F] |
| 2 | 稀少 | Scarce | (0.1F, 0.3F] |
| 3 | 适中 | Moderate | (0.3F, 0.6F] |
| 4 | 充足 | Adequate | (0.6F, 0.8F] |
| 5 | 丰沛 | Abundant | (0.8F, +∞) |

当前地区降水量可以使用雨量计获取，但只能定性分析。

## 湿度

在本系统中，根据该地区温度与湿度关系，将湿度划分为以下五个级别。

| 编号 | 湿度分级 | 英文 |
|------|----------|------|
| 1 | 干旱 | Arid |
| 2 | 干燥 | Dry |
| 3 | 一般 | Moderate |
| 4 | 湿润 | Moist |
| 5 | 潮湿 | Humid |

**湿度分级标准**：

以降水量编号为基准，其编号与温度编号每相差2，得到的湿度降1。

详细对应如下表：（两位数字，前一位表示降水量，后一位表示温度）

| 湿度分级 | 对应降水量与温度 | 备注 |
|------|------------------------|------|
| 干旱 | 11，12，13，14，15，16，24，25，26 |  |
| 干燥 | 21，22，23，31，35，36 | 干冷，或类似我国夏天 |
| 一般 | 32，33，34，41，42，46，51 | 什么情况都有 |
| 湿润 | 43，44，45，52，53 | 湿热或湿冷 |
| 潮湿 | 54，55，56 | 高温高湿 |

游戏内大部分环境设定基本与湿度相关。

## 相关工具合成

![玻璃 * 7 + 水桶 * 1 → 温度计 * 1](../.gitbook/assets/recipes/thermometer_recipe.png)

![玻璃 * 6 + 水桶 * 1 → 雨量计 * 1](../.gitbook/assets/recipes/rain_gauge_recipe.png)

![温度计 * 1 + 雨量计 * 1 → 湿度计 * 1](../.gitbook/assets/recipes/hygrometer_recipe.png)