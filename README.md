# engineering-fluid-mechanics-skill

工程流体力学本科助教 Agent Skill —— 对齐扬州大学电能学院《工程流体力学（双语）》2025 版教学大纲（能源动力类专业，72 学时），专注**查定义**与**做题**两大核心场景，内置中英术语对照，覆盖实验指导。

> An agent skill for undergraduate Engineering Fluid Mechanics tutoring, aligned with a bilingual course syllabus (72 hours: 56 theory + 16 lab) — concept lookup and problem-solving, with formula cheatsheets, misconception lists, problem-type templates, a bilingual (Chinese–English) glossary, and lab report guidance.

## 功能特性

### 场景一：查定义

学生询问概念、术语、定律时，按固定结构作答：

> 一句话定义 → 物理意义 → 公式表达 → 易混淆概念辨析 → 小例子

内置 **26 条常见误区速查清单**，覆盖连续介质假设、流线与迹线、系统与控制体、速度势与流函数、达朗贝尔悖论、激波不可逆性等高频混淆点。

### 场景二：做题

学生给出习题/例题/考试题时，按固定五步框架求解：

> 画流动简图 → 列已知与所求 → 选方程与假设 → 列方程求解 → 结果检验

- 内置**方程选择决策树**与 **11 类题型模板**：流体静力学（测压、平面/曲面总压力、相对平衡）、伯努利方程应用、动量方程、管路水力计算（短管/长管/串并联）、泵与管路工况、量纲分析与模型实验、**平面势流叠加与绕圆柱升力**、**可压缩流动与正激波**、**实验数据处理与报告**
- 强调阅卷采分点：能量方程必写基准面与断面位置、λ 计算必先算 Re 判流态、势流题先验证无旋/不可压缩再积分、激波题必校核 Ma₂ < 1 等物理约束
- 内置**隐含条件词典**与 **14 条常见失分点**

### 配套参考

- **公式速查表**：12 章完整公式体系，含势流基本流动表、哈根-泊肃叶解析解、正激波公式组（γ=1.4 特化）+ 单位换算 + 高频错误提醒
- **中英术语对照表**：按十章组织约 200 条术语（对齐 Frank M. White《Fluid Mechanics》用词），直接服务于双语测验与考试
- **图示规范**：总水头线/测压管水头线绘制规则、势流图谱（流线与等势线正交）、压强分布图、尼古拉兹曲线五区、边界层分离示意

## 课程大纲对齐

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
- "velocity potential 和 stream function 有什么区别？"
- "已知水箱水面距出流管中心 5 m，管径 50 mm，管长 100 m，λ=0.025，忽略局部损失，求流量。"
- "均匀流 + 点源叠加，求驻点位置和物面方程。"
- "正激波前 Ma₁=2.5，求波后压强比和马赫数。"
- "帮我整理雷诺实验的数据并分析误差来源。"

## 适用范围

- 面向本科通用《工程流体力学》课程体系，（能源与动力工程、新能源科学与工程、建筑环境与能源应用工程等专业）；
- 覆盖流体静力学、流体动力学、流动阻力、孔口管嘴堰流、量纲分析与相似理论、边界层与绕流、明渠流、气体动力学基础（选学）；
- 默认约定：g = 9.81 m/s²，水 ρ = 1000 kg/m³，统一 SI 单位。

## 相关项目

- [engineering-thermodynamics](https://github.com/) —— 同系列工程热力学助教 skill

## License

MIT
