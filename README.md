# userguide

上传论文的格式说明

## Step1. 创建仓库

1. 仓库创建到组织 CISLC-Paper 名下
2. 仓库名为：`{论文负责人姓名简写}-{论文题目简写}`，例如：`mcz-tpcs-vul`，`mcz-parallel-sim`
3. 仓库可见性选 **私有**
4. 创建后，为组织成员添加可见性：打开仓库 - `Settings` - `Collaborators and teams` - `Add teams` - 选择 `cislc` - 选择 `Read` 权限 - 点击 `Add selection` 按钮

## Step2. README.md 文件内容

模板如下：

```markdown
<!-- 标题为 {负责人}。{论文概述}。{当前状态}。仓库描述同此标题 -->
# 孟成真。TPCS（VUL）语法、执行语义、RTL生成。TC Rev 1

> **论文标题：** TPCS: A Cycle-Level Simulation Paradigm with Native Execution Semantics for RTL Modeling and Generation

## 基本信息

| 项目 | 内容 |
|---|---|
| **当前状态** | 第二轮审稿中 |
| **目标会议/期刊** | TC |
| **主要负责人** | 孟成真 |
| **指导老师** | 戴鸿君 |
| **其他作者** | 李潇宇，张真瑜，白晨 |
| **当前版本** | Revision 1 |
| **最近更新** | 2026-10-05 |

## 当前进度

- [-] Introduction / 引言
- [-] Background & Related Work / 背景与相关工作
- [-] Method / Design / 方法与设计
- [-] Implementation / 实现
- [-] Evaluation / 实验评估
- [-] Conclusion / 总结
- [ ] 图表检查
- [ ] 引用检查
- [ ] 内部审阅
- [ ] 投稿准备

### 当前主要任务

- [-] 已完成的任务
- [ ] `<任务 2>`
- [ ] `<任务 3>`
```

## Step3. 仓库组织结构

1. 仓库描述同 README.md 文件标题
2. 仓库根目录下必须有：
   - `README.md`：论文的基本信息和说明
   - `*.tex`：论文的唯一 LaTeX 入口文件
   - `Makefile`：编译论文的 Makefile 文件
3. 推荐结构如下：
   - `figures/`：存放论文中使用的图文件
   - `sections/`：如果需要多个 tex 文件组织论文内容，可以放在此目录下
   - `references/`：存放论文中使用的 .bib 参考文献文件

## Step4. Release 版本管理

1. 在每次投稿节点（或更新修改稿）时，创建一个 Release 版本
2. Release 版本命名为 `{期刊/会议简称}-{提交版本}`，例如：`TCAD-Submit`，`TCAD-Rev1`，`TCAD-Accepted`, `TCAD-Final`
3. Release 发布中额外包含的内容：
   - 最终的 PDF 文件
   - 实验代码与数据打包
   - 原始数据文件（如果有）
   - Cover Letter 文件（如果有）
   - Reviewer Response Letter 文件（如果有）
   - 修改稿差异版文件（如果有）
4. Release 版本的 PDF 文件同步更新 Arxiv 版本
