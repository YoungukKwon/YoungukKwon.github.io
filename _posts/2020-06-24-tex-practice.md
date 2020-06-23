---
title:  "LaTex practice"

#categories:
#  - Blog
#tags:
#  - Blog
#last_modified_at: 2019-04-13T08:06:00-05:00
---

$e^{i \pi} = -1$

$\begin{align}
  \mathrm{Var}(S_n) &= \mathrm{E}(S_n^2) \geq \mathrm{E}(S_n^2; \cup_{k=1}^n A_k)\\
                                &= \sum\limits_{k=1}^n \int_{A_k} S_n^2 \: dP \\
                                &= \sum\limits_{k=1}^n \int_{A_k} (S_n - S_k + S_k)^2 \: dP \\
                                &= \sum\limits_{k=1}^n \int_{A_k} (S_n - S_k)^2 + S_k^2 + 2S_k (S_n - S_k) \: dP \\
                                &\geq \sum\limits_{k=1}^n \big\{ \int_{A_k} S_k^2 + 2\int_{\Omega}S_k\boldsymbol{1}_{A_k}\: dP \int_{\Omega}(S_n - S_k) \: dP \big\}\\
                                &= \sum\limits_{k=1}^n \int_{A_k} S_k^2 \: dP \\
                                &\geq \sum\limits_{k=1}^n \int_{A_k} x^2 \: dP \\
                                &= x^2P(\cup_{k=1}^n A_k) \\
                                &= x^2 P(\max_{1 \leq k \leq n} |S_k| > x)
\end{align}$
