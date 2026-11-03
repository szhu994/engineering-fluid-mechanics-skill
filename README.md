# engineering-fluid-mechanics-skill

工程流体力学本科助教 Agent Skill —— 面向本科生学习场景，专注**查定义**与**做题**两大核心需求。

> An agent skill for undergraduate Engineering Fluid Mechanics tutoring — concept lookup and problem-solving, with formula cheatsheets, misconception lists, problem-type templates, and energy/hydraulic grade line diagram conventions.

## 功能特性

### 场景一：查定义

学生询问概念、术语、定律时，按固定结构作答：

> 一句话定义 → 物理意义 → 公式表达 → 易混淆概念辨析 → 小例子

覆盖连续介质假设、牛顿内摩擦定律、流线与迹线、层流与湍流、雷诺数、伯努利方程、水力半径、边界层分离、水击、相似准则等核心概念，内置 **17 条常见误区速查清单**。

### 场景二：做题

学生给出习题/例题/考试题时，按固定五步框架求解：

> 画流动简图 → 列已知与所求 → 选方程与假设 → 列方程求解 → 结果检验

- 内置**方程选择决策树**与 **8 类题型模板**：流体静力学（测压、平面/曲面总压力）、伯努利方程应用、动量方程、管路水力计算（短管/长管/串并联）、泵与管路工况、孔口管嘴堰流、量纲分析与模型实验、明渠均匀流
- 强调阅卷采分点：能量方程必写基准面与断面位置、λ 计算必先算 Re 判流态、压强基准全程统一
- 内置**隐含条件词典**（"大水箱"→自由面流速≈0、"长管"→忽略局部损失、"通大气"→表压为 0 等）与**十大常见失分点**

### 配套参考

- **公式速查表**：11 章完整公式体系（流体性质、静力学、三大方程、阻力损失、孔口堰流、量纲分析、边界层、明渠流）+ 单位换算 + 高频错误提醒
- **图示规范**：总水头线/测压管水头线绘制七条规则、压强分布图、压力体图、尼古拉兹曲线五区、边界层分离示意、水跃水跌图

## 目录结构

```
engineering-fluid-mechanics/
├── SKILL.md                        # 触发描述 + 双场景工作流
└── references/
    ├── concepts.md                 # 核心概念辨析与常见误区清单
    ├── problem-solving.md          # 解题方法论、题型模板与检验清单
    ├── formulas.md                 # 公式速查表与单位换算
    └── diagrams.md                 # 水头线、流线图等图示规范
```

采用渐进式加载设计：SKILL.md 保持精简，四个参考文件按场景需要才被读入，节省上下文。

## 安装使用

1. 下载 [engineering-fluid-mechanics.skill](engineering-fluid-mechanics.skill) 文件；
2. 在支持 Agent Skill 的平台（如 Kimi、Claude）中上传安装；
3. 安装后无需手动调用——当对话涉及工程流体力学概念提问或习题求解时自动触发。

触发示例：

- "什么是雷诺数？它和临界雷诺数有什么关系？"
- "流线和迹线有什么区别？"
- "已知水箱水面距出流管中心 5 m，管径 50 mm，管长 100 m，λ=0.025，忽略局部损失，求流量。"
- "帮我画一下这条管路的总水头线和测压管水头线。"

## 适用范围

- 面向本科通用《工程流体力学》课程体系，不限定教材；
- 覆盖流体静力学、流体动力学、流动阻力、孔口管嘴堰流、量纲分析与相似理论、边界层与绕流、明渠流、气体动力学基础（选学）；
- 默认约定：g = 9.81 m/s²，水 ρ = 1000 kg/m³，统一 SI 单位。

## 相关项目

- [engineering-thermodynamics](https://github.com/) —— 同系列工程热力学助教 skill

## License

MIT
内置公式速查、概念误区清单、八类题型解题模板与水头线图示规范。
[README (1).md](https://github.com/user-attachments/files/34322791/README.1.md)
