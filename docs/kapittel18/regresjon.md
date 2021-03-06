---
layout: default
title: Regresjon
nav_order: 1
parent: Kapittel 18
---

# Regresjon
{: .no_toc}
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## $$n$$-ordens regresjon
{: .text-green-000 }

Utregning av regresjon for et datasett er ikke eksamensrelevant.

### 1. ordens regresjon
{: .text-green-200 }

$$y = ax+b$$

---

### 2. ordens regresjon
{: .text-green-200 }

$$y=ax^2+bx+c$$

---

### 3. ordens regresjon
{: .text-green-200 }

$$y=ax^3+bx^2+cx+d$$

---

## Bestemmelses koeffisient
{: .text-green-000 }

$$S^2_y$$ - Varians

$$S^2_y = \sum \bigg(y_i - \overline{Y}\bigg)^2$$

$$SSE$$ - Sum of squares of errors

$$SSE = \sum \bigg(y_i - (k_{o})\bigg)^2$$

Hvor $$k_o$$ er $$ax+b$$, $$ax^2+bx+c$$ osv., bestemmeleseskoeffisienten er da

$$r^2=\frac{S^2_y-SSE}{S^2_y}$$

Tolkning av $$r^2$$

* $$ 0 \leq r^2 \leq 1$$.
* $$r^2 \approx 0$$ : Dårlig modell
* $$r^2 \approx 1$$ : God modell

---
