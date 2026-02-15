## 🕵️ 图论案例分析：从《亚人》看隐藏节点的聚类问题

### 1. 初始状态：Disconnected Graph (离散图)
- **特征：** $G = (V, E)$，其中 $E = \emptyset$。
- **现象：** 社会原子化。由于生存成本 $C \rightarrow \infty$，节点选择屏蔽所有 Edges。
- **困境：** 外部监控者无法通过广度优先搜索 (BFS) 进行追踪，因为不存在路径 (Path)。

### 2. 佐藤算法：Hub-based Clustering (基于枢纽的聚类)
- **核心操作：** Create a High-Degree Node (Sato himself).
- **连接机制：** - 通过公共信号（Broadcast）降低连接的感知成本。
  - 诱导隐藏节点主动请求建立边 (Request an Edge)。
- **拓扑演变：** 从零散节点演变为 **星型拓扑 (Star Topology)**，佐藤作为中心点 (Centrality)。

### 3. 风险评估：连通度与脆弱性
- **逻辑：** 连通度 (Connectivity) 越高，组织力越强，但系统的 **节点删除脆弱性** 也越高。
- **反思：** 如果佐藤（中心节点）被端掉，整个亚人网络将再次坍缩回原子化状态。

## 🏥 HEOR 专题：罕见病患者的“显性化”障碍

### 1. 识别障碍 (Identification Barriers)
- **逻辑错误：** 节点属性误读（误诊）。
- **图论映射：** 节点存在但标签 (Label) 错误，导致无法通过属性筛选器筛选。

### 2. 激励不兼容 (Incentive Incompatibility)
- **公式：** 当 $E(\text{Stigma}) > E(\text{Treatment})$ 时，个体选择保持孤立。
- **策略：** 必须通过政策干预（如孤儿药法案）来降低连接成本，提高连接收益。

### 3. 连通性难题 (Connectivity Issues)
- **数据孤岛：** 缺乏跨机构的共同知识 (Common Knowledge)。
- **解决方案：** 建立全球性的中心枢纽（Hubs），类似于佐藤的信号塔，但目的是科研协作。
