---
layout: default
title: Sannsynlighets Fordelinger
parent: Kapittel 14
nav_order: 2
---

# Sannsynlighets Fordelinger
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Binomial fordeling
{: .text-green-000 }

Binomialfordelingen er en fordeling av tilfeldige forsøk med tilbakelegging, hvor $$n$$ er antall trekk, og $$p$$ er sjansen for trekk.

$$X \sim Bin(n,p)$$

### Forventing
{: .text-green-200 }

$$E(X) = n\cdot p$$

### Varians
{: .text-green-200 }

$$Var(X) = n\cdot p \cdot (1-p)$$

### $$P(X=x)$$, sjanse for x
{: .text-green-200 }

$$P(X=x) = \binom{n}{x}p^x(1-p)^{n-x}$$

### Binomial Koeffisient
{: .text-green-200 }

La $$k$$ og $$n$$ være heiltall der $$0\leq k \leq n$$, da er binomial koeffesienten $$\binom{n}{k}$$ gitt ved

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

---

## Hypergeometrisk fordeling
{: .text-green-000 }

Den Hypergeometriske fordelingen er en fordeling av tilfeldige forsøk uten tilbakelegging, hvor $$N$$ er totalt antall element, $$M$$ er antall positive forsøk, og $$n$$ er antall forsøk.

$$X \sim hypergeom(N,M,n)$$

### $$P(X=x)$$, sjanse for x
{: .text-green-200 }

$$P(X=x) = \frac{\binom{M}{x}\binom{N-M}{n-x}}{\binom{N}{n}}$$

### Forventning
{: .text-green-200 }

$$E(X) = n \cdot \frac{M}{N}$$

### Varians
{: .text-green-200 }

$$Var(X) = n \cdot \frac{M}{N}\bigg(1-\frac{M}{N}\bigg)\cdot\frac{N-n}{N-1}$$

---

## Poisson fordeling
{: .text-green-000 }

Poisson fordelingen beskriver tilfeller der vi har et endelig antall positive utfall i en kontinuerlig mengde, hvor $$\lambda$$ er frekvenskonstant og $$t$$ er antall enheter.

$$X \sim Po(\lambda t)$$

### Forventning og Varians
{: .text-green-200 }

$$E(X) = Var(X) = \lambda t$$

### Sannsynlighet for $$x$$ utfall
{: .text-green-200 }

$$P(X=x) = \frac{(\lambda t)^x}{x!}e^{-\lambda t}$$

---

## Eksempler
{: .text-green-000 }

### Poisson Fordeling
{: .text-green-200 }

Vi måler antall sms mottatt på en basestasjon over 20 sekunder. En basestasjon mottar i snitt 4 sms pr. minutt. Hva er sannsynligheten for at vi får nøyaktig 2 sms? Hva er sannsynligheten for at vi får minst 1 sms?

La $$X=\{\text{antall sms på 20 sekund}\}$$, og $$\lambda = 4 \text{ sms/min}$$, og $$t = 20 \text{ sek} = \dfrac{1}{3} \text{ minutt}$$.

Da er

$$X \sim Po(4\cdot \dfrac{1}{3})$$

*Hva er sannsynligheten for å få nøyaktig 2 sms?*

$$P(\text{nøyaktig 2 sms}) = \dfrac{(\frac{4}{3})^2}{2!}e^{-\dfrac{4}{3}} = \underline{\underline{0.234}}$$

*Hva er sannsynligheten for å få minst 1 sms?*

$$P(\text{minst 1 sms}) = 1 -  \dfrac{(\frac{4}{3})^0}{0!}e^{-\dfrac{4}{3}} = \underline{\underline{0.736}}$$

---
