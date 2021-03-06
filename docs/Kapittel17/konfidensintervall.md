---
layout: default
title: Konfidensintervall
nav_order: 2
parent: Kapittel 17
---

# Konfidensintervall
{: .no_toc}
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Konfidensintervall
{: .text-green-000 }

Målet med et konfidensintervall er å finne et intervall $$[a,b]$$ der en med $$(1-\alpha)$$ % sikkerhet vet at gjennomsnittet ligger i intervallet.

### Hvilke faktorer påvirker resultatet?
{: .text-green-200 }

- Antall målinger
- Hvor sikker en vil være, $$95$$ %? $$99%$$ %?

### Framgangsmåte
{: .text-green-200 }

Bakgrunn:

- Anta at $$X_1,X_2,...,X_n$$ er et sett med normalfordelte stokastiske variabler. $$X_i \sim N(\mu,\sigma^2)$$.
- Anta at $$\mu$$ er ukjent.
- Anta at $$\sigma^2$$ er kjent.

La estimatoren $$\hat{\mu} = \frac{1}{n}\sum X_i$$, og er normalfordelt $$\hat{\mu}\sim N(\mu,(\frac{\sigma}{\sqrt{n}})^2)$$.

Da er $$(1-\alpha)$$ - konfidensintervallet for $$\mu$$ gitt ved

$$\hat{\mu} \pm u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}}= \bigg[\hat{\mu}-u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}},\hat{\mu}+u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}}\bigg]$$

Hvor $$u_\alpha$$ er en konstant.

### Lengde av konfidensintervall
{: .text-green-200 }

Formel for å finne antall forsøk som trengs for at lengden av intervallet skal være $$\leq k$$

$$\begin{align*}
\hat{\mu}+u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}} - (\hat{\mu}-u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}}) &\leq k\\
2u_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}} &\leq k \\
2u_{\alpha/2} \cdot \sigma &\leq k\sqrt{n} \\
\bigg(2\frac{u_{\alpha/2} \cdot \sigma}{k}\bigg)^2 &\leq n
\end{align*}$$

---

## Student-t Fordeling
{: .text-green-000 }

La $$\hat{\mu} = \overline{X}$$ være estimat for forventningsverdi.

La $$S^2$$ være estimat for variansen.

$$S^2= \frac{1}{n-1} \sum \bigg( X_i - \overline{X} \bigg)^2$$

$$(1-\alpha)$$ konfidensintervallet for $$\mu$$ er:

$$\overline{X} \pm t_{\alpha/2,n-1} \cdot \frac{S}{\sqrt{n}}$$

---
## $$u_{\alpha/2}$$ tabell
{: .text-green-000 }

| $$u_\alpha$$ | $$\alpha$$ | Sikkerhet |
|:-------------|:-----------|:----------|
| $$1.960$$ | $$0.025$$ | $$97.5$$ % konf. int.|
| $$1.645$$ | $$0.05$$ | $$95$$ % konf. int.|
