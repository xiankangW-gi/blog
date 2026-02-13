---
title: Reconciling Capital-Embodied Progress with Uzawa on a BGP
date: 2026-02-13
tags: [macro, growth, solow, uzawa, automation, task-based]
---

When I was listening to the Solow model in a graduate-level macroeconomics class taught by my advisor, Professor Feng, I noticed something a bit puzzling:

At the micro level, most technological progress seems **embodied in capital goods**. But when the elasticity of substitution is **not** one, the **Uzawa theorem** tells us that a balanced growth path (BGP) requires technical change to be **purely labor-augmenting** in the aggregate. That seems at odds with micro-level, capital-augmenting technological progress.

Of course, recent literature has developed different ways to deal with this tension. This paper gives a more natural way to think about it.

## The key move: split capital-embodied progress into two margins in a task-based economy

The key move in this paper is to split capital-embodied progress into two margins inside a task-based economy:

1. **Horizontal margin (extensive): capital takes over tasks previously done by labor**  
   Controlled by the automated task share, denoted by **beta**:
   $$\beta$$

2. **Vertical margin (intensive): capital becomes more productive at already-automated tasks**  
   Controlled by aggregate capital productivity:
   $$Z$$

So “capital-embodied progress” is not one-dimensional: it can mean **doing more tasks** (higher $\beta$) and/or **doing automated tasks better** (higher $Z$).

## Complementarity creates a tug-of-war in factor shares

When the elasticity of substitution is smaller than 1—often implemented via strong complementarity across tasks—we get a tug of war:

- As $\beta$ becomes larger, it tends to **raise capital’s income share**, because capital performs more tasks.
- However, higher $Z$ can **reduce capital’s income share**, because prices of the improved input fall fast in a complementary structure: high-productivity components become cheaper and their GDP share shrinks.

A quick summary:

- Higher $\beta$ changes *how many* tasks capital does → pushes capital share **up**.  
- Higher $Z$ changes *how cheap* automated tasks become → can pull capital share **down**.

## Balanced growth: stabilize the capital share via an offsetting condition

Balanced growth requires a stable capital share. The paper shows that if the “task takeover” force and the “productivity in automated tasks” force offset each other—specifically, if

$$\frac{\beta}{Z}=\text{constant},$$

then the economy converges to a BGP.

## Why Uzawa holds in the aggregate, even if innovation is capital-embodied

Under this condition, at the macro level it *looks as if* growth is driven by **labor-augmenting** technical change—satisfying Uzawa—even though all innovation is capital-embodied at the micro level.

The intuition is:

- Automation (higher $\beta$) **shrinks the set of tasks done by labor** (labor concentrates on fewer tasks).
- Rising capital productivity (higher $Z$) makes automated tasks **cheaper**, so their GDP share becomes **smaller**.
- The two forces offset in income shares, keeping the capital share stable along the BGP.