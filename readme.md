# Alpha Stack -- Structure-Driven Trading System

## 🧠 Core Idea

Alpha Stack 是一个基于市场结构（Structure）的多模式交易系统。
系统不预测价格，而是识别市场状态（regime），并动态决定策略、仓位和风险。

------------------------------------------------------------------------

## ⚙️ System Architecture

S1 → S2 → S3 → S4 → S5 → S6

  Layer   Name        Role
  ------- ----------- -------------------
  S1      Structure   市场结构表达
  S2      Regime      模式识别 + gating
  S3      Signal      交易意图
  S4      Position    仓位决策
  S5      Risk        风控覆盖
  S6      Decision    最终执行

------------------------------------------------------------------------

## 🔍 Core Principle

-   不预测，只分类
-   Structure \> Signal
-   allow_trade \> signal
-   最大风险来自错误的策略匹配

------------------------------------------------------------------------

## 🧩 Layer Logic

### S1 -- Structure

表达市场状态（trend / range / risk）

### S2 -- Regime

压缩结构 → 决定是否参与交易

### S3 -- Signal

Signal = f(S2 gating, S1 detail)

### S4 -- Position

决定仓位大小

### S5 -- Risk

风险覆盖（override）

### S6 -- Decision

最终执行

------------------------------------------------------------------------

## 🔁 Data Flow

Market → Indicators → Factors → Structure → S1 → S2 → S3 → S4 → S5 → S6

------------------------------------------------------------------------

## 🧠 Summary

不是用一个策略应对市场， 而是用结构驱动策略、仓位和风险的动态切换。
