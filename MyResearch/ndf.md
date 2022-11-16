# Light Nuclei ratios from neutron density fluctuation

## 1. Coalescence
  In COAL-SH, the yield $N_c$ (per unit rapidity) of a cluster at mid-rapidity and consisting of $A$ constituent particles from the hadronic matter at kinetic freeze-out or emission source of effective temperature $T_{\rm eff}$ (including the effect of transversal flow), volume $V$, and number $N_i$ of the $i$-th constituent with mass $m_i$
  
$$
  \begin{equation}N_c=g_{rel}g_{size}g_cM^{3/2}\prod_{i=1}^A\frac{N_i}{m_i^{3/2}}\prod_{i=1}^{A-1}\frac{(4\pi/\omega)^{3/2}}{Vx(1+x^2)}\left(\frac{x^2}{1+x^2}\right)^{l_i}G(l_i,x)
  \end{equation}
$$

  In the above, $M=\sum\limits_{i=1}^{A}m_i$ is the rest mass of the cluster, $l_i$ is the orbital angular momentum associated with the $i$-th relative coordinate, $\omega$ is the oscillator frequency of the cluster's internal wave function and is inversely proportional to $M r_\text{rms}^2$ with $r_\text{rms}$ being the root-mean-square (RMS) radius of the cluster, and $G(l,x) = \sum\limits_{k=0}^{l}\frac{l!}{k!(l-k)!} \frac{1}{(2k+1)x^{2k}}$ with $x=\left(\frac{2T_{\rm eff}}{\omega}\right)^{1/2}$ is the suppression factor due to the orbital angular momentum on the coalescence probability. In addition, $g_c =\frac{2S+1}{\prod\limits_{i=1}^{A}(2s_i+1)}$ is the coalescence factor for constituents of spin $s_i$ to form a cluster of spin $S$, $g_{rel}$ is the relativistic correction to the effective volume in momentum space, and $g_{size}$ is the correction due to the finite size of produced cluster.

  In central A+A collisions considered, $V$ is much larger than the sizes of light nuclei, and we thus set $g_{size}= 1$. We also set $g_{rel} = 1$ because the masses of nucleons and light nuclei are much larger than the value of $T_{\rm eff}$. For light nuclei included in the present study, all the constituent nucleons are in $s$-state ($l=0$), and we thus have $G(l,x)=1$, $x=\left(\frac{2T_{\rm eff}}{\omega}\right)^{1/2}\gg 1$. The yields of light nuclei are then simply given by
$$
  \begin{align}
    N_c&=g_cM^{3/2}\prod_{i=1}^A\frac{N_i}{m_i^{3/2}}\prod_{i=1}^{A-1}\frac{(4\pi/\omega)^{3/2}}{Vx^3}=g_cM^{3/2}\prod_{i=1}^A\frac{N_i}{m_i^{3/2}}\prod_{i=1}^{A-1}\frac{(4\pi/\omega)^{3/2}}{V\left(2T_{\rm eff}/\omega\right)^{3/2}}\nonumber\\
    &=g_cM^{3/2}\prod_{i=1}^A\frac{N_i}{m_i^{3/2}}\prod_{i=1}^{A-1}\frac{1}{V}\left(\frac{2\pi}{T_{\rm eff}}\right)^{3/2}=g_c(Am_0)^{3/2}\frac{N_p^{A_p}N_n^{A_n}}{m_0^{3A/2}}\frac{1}{V^{A-1}}\left(\frac{2\pi}{T_{\rm eff}}\right)^{3(A-1)/2}\nonumber\\
    &=B_c\frac{N_p^{A_p}N_n^{A_n}}{V^{A-1}}=B_cV\int\rho_p^{A_p}(\vec{r})\rho_n^{A_n}(\vec{r})d\vec{r}
  \end{align}
$$

where $A_p,A_n$ are the number of protons and neutron in the coalescence nuclei, $A=A_p+A_n$.

$$
  \begin{equation}
    B_c=g_cA^{3/2}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3(A-1)/2}=\frac{2S_c+1}{2^A}A^{3/2}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3(A-1)/2}
  \end{equation}
$$

For $p$ and $n$,
$$
\begin{align}
  N&=V\int \rho(\vec{r}) d\vec{r}=V\langle\rho\rangle+V\int[\rho(\vec{r})-\langle\rho\rangle]d\vec{r}\nonumber\\
  &=V\langle\rho\rangle+V\int\delta\rho(\vec{r}) d\vec{r}=V(\langle\rho\rangle+\langle\delta\rho\rangle)=V\langle\rho\rangle
\end{align}
$$

$$ 
  \begin{align}
    N_c&=B_cV\int[\langle\rho_p\rangle+\delta\rho_p(\vec{r})]^{A_p}[\langle\rho_n\rangle+\delta\rho_n(\vec{r})]^{A_n}d\vec{r}\nonumber\\
    &=B_cV\int\sum_{i=0}^{A_p}\sum_{j=0}^{A_n}C_{A_p}^i\langle\rho_p\rangle^{A_p-i}[\delta\rho_p(\vec{r})]^iC_{A_n}^j\langle\rho_n\rangle^{A_n-j}[\delta\rho_n(\vec{r})]^jd\vec{r}\nonumber\\
    &=B_cV\sum_{i=0}^{A_p}\sum_{j=0}^{A_n}C_{A_p}^iC_{A_n}^j\langle\rho_p\rangle^{A_p-i}\langle\rho_n\rangle^{A_n-j}\langle\delta\rho_p^i\delta\rho_n^j\rangle\nonumber\\
    &=B_cV\langle\rho_p\rangle^{A_p}\langle\rho_n\rangle^{A_n}\sum_{i=0}^{A_p}\sum_{j=0}^{A_n}C_{A_p}^iC_{A_n}^jC_{n^jp^i}
  \end{align}
$$

where $C_{n^jp^i}=\frac{\langle\delta\rho_p^i\delta\rho_n^j\rangle}{\langle\rho_p\rangle^i\langle\rho_n\rangle^j}$ is the $j$-neutrons and  $i$-protons correlation. $C_{n^0p^0}=1, C_{n^1p^0}=0, C_{n^0p^1}=0$. Relatively density fluctuation $C_{n^0p^2}=\frac{\langle\delta\rho_p^2\rangle}{\langle\rho_p\rangle^2}=\Delta\rho_p, C_{n^2p^0}=\frac{\langle\delta\rho_n^2\rangle}{\langle\rho_n\rangle^2}=\Delta\rho_n$

Used the symbols in statistics, 

$$
  \begin{equation}
    C_{np}=\frac{\text{Cov}(\rho_n,\rho_p)}{\langle\rho_n\rangle\langle\rho_n\rangle}=\frac{r_{\rho_n,\rho_p}\sigma_{\rho_n}\sigma_{\rho_p}}{\langle\rho_n\rangle\langle\rho_n\rangle}
  \end{equation}
$$

so 
$$
  \begin{align}
    N_d&=B_dV\langle\rho_p\rangle\langle\rho_n\rangle\sum_{i=0}^{1}\sum_{j=0}^{1}C_{n^jp^i}=B_dV\langle\rho_p\rangle\langle\rho_n\rangle(1+C_{np})\\
    N_t&=B_tV\langle\rho_p\rangle\langle\rho_n\rangle^{2}\sum_{i=0}^{1}\sum_{j=0}^{2}C_{2}^jC_{n^jp^i}=B_tV\langle\rho_p\rangle\langle\rho_n\rangle^{2}(1+\Delta\rho_n+2C_{np}+C_{n^2p})\\
    N_{^3\text{He}}&=B_tV\langle\rho_p\rangle^2\langle\rho_n\rangle\sum_{i=0}^{2}\sum_{j=0}^{1}C_{2}^iC_{n^jp^i}=B_tV\langle\rho_p\rangle^2\langle\rho_n\rangle(1+\Delta\rho_p+2C_{np}+C_{np^2})\\
    N_{\alpha}&=B_{\alpha}V\langle\rho_p\rangle^{2}\langle\rho_n\rangle^{2}\sum_{i=0}^{2}\sum_{j=0}^{2}C_{2}^iC_{2}^jC_{n^jp^i}\nonumber\\
    &=B_{\alpha}V\langle\rho_p\rangle^2\langle\rho_n\rangle^2(1+\Delta\rho_n+\Delta\rho_p+4C_{np}+2C_{n^2p}+2C_{np^2}+C_{n^2p^2})
  \end{align}
$$

## 2. Light nuclei ratio

To extract the $\Delta\rho_p$ or $\Delta\rho_p$,

$$
  \begin{align}
  B_d&=\frac{2S_d+1}{2^2}2^{3/2}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3/2}=\frac{3}{2^{1/2}}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3/2}\\
  B_t&=\frac{2S_t+1}{2^3}3^{3/2}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3}=\frac{3^{3/2}}{4}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{3}=B_{^3\text{He}}\\
  B_{\alpha}&=\frac{2S_{\alpha}+1}{2^4}3^{3/2}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{9/2}=\frac{3^{3/2}}{4}\left(\frac{2\pi}{m_0T_{\rm eff}}\right)^{9/2}
  \end{align}
$$

$$
  \begin{align}
    \frac{N_tN_p}{N_d^2}&=\frac{B_tV^2\langle\rho_p\rangle^2\langle\rho_n\rangle^{2}(1+\Delta\rho_n+2C_{np}+C_{n^2p})}{B_d^2V^2\langle\rho_p\rangle^2\langle\rho_n\rangle^2(1+C_{np})^2}=\frac{B_t(1+\Delta\rho_n+2C_{np}+C_{n^2p})}{B_d^2(1+C_{np})^2}\nonumber\\
    &=\frac{1}{2\sqrt{3}}\frac{1+\Delta\rho_n+2C_{np}+C_{n^2p}}{(1+C_{np})^2}
  \end{align}
$$

$$
  \begin{equation}
    \frac{N_{^3\text{He}}N_n}{N_d^2}=\frac{1}{2\sqrt{3}}\frac{1+\Delta\rho_p+2C_{np}+C_{np^2}}{(1+C_{np})^2}
  \end{equation}
$$

## 3. Multi-particle correlations

$$
  \begin{align*}
    \langle\delta\rho_p^i\delta\rho_n^j\rangle&=\langle(\rho_p-\langle\rho_p\rangle)^i(\rho_n-\langle\rho_n\rangle)^j\rangle=\left\langle\sum_{r=0}^iC_i^r(-1)^r\rho_p^{i-r}\langle\rho_p\rangle^r\sum_{s=0}^jC_j^s(-1)^s\rho_n^{j-s}\langle\rho_n\rangle^s\right\rangle\\
    &=\sum_{r,s=0}^{i,j}(-1)^{r+s}C_i^rC_j^s\langle\rho_p\rangle^r\langle\rho_n\rangle^s\left\langle\rho_p^{i-r}\rho_n^{j-s}\right\rangle
  \end{align*}
$$

$$
  \langle\delta\rho_p\delta\rho_n\rangle=\left\langle\rho_p\rho_n\right\rangle-\langle\rho_p\rangle\left\langle\rho_n\right\rangle=C_{np}\langle\rho_p\rangle\langle\rho_n\rangle
$$

so
$$
  \begin{equation}
    C_{np}=\frac{\left\langle\rho_p\rho_n\right\rangle}{\langle\rho_p\rangle\langle\rho_n\rangle}-1
  \end{equation}
$$

$\left\langle\rho_p\rho_n\right\rangle=(1+C_{np})\langle\rho_p\rangle\langle\rho_n\rangle$

$$
\begin{align*}
  \langle\delta\rho_p\delta\rho_n^2\rangle&= \left\langle\rho_p\rho_n^2\right\rangle-2\langle\rho_n\rangle\left\langle\rho_p\rho_n\right\rangle+\langle\rho_n\rangle^2\left\langle\rho_p\right\rangle-\langle\rho_p\rangle\left\langle\rho_n^2\right\rangle+2\langle\rho_p\rangle\langle\rho_n\rangle^2-\langle\rho_p\rangle\langle\rho_n\rangle^2\\
  &=\left\langle\rho_p\rho_n^2\right\rangle-2\langle\rho_n\rangle\left\langle\rho_p\rho_n\right\rangle+\langle\rho_p\rangle\langle\rho_n\rangle^2\\
  &=\left\langle\rho_p\rho_n^2\right\rangle-(1+2C_{np})\langle\rho_p\rangle\langle\rho_n\rangle^2=C_{n^2p}\langle\rho_p\rangle\langle\rho_n\rangle^2
\end{align*}
$$

so
$$
  \begin{equation}
    C_{n^2p}=\frac{\left\langle\rho_p\rho_n^2\right\rangle}{\langle\rho_p\rangle\langle\rho_n\rangle^2}-(1+2C_{np})
  \end{equation}
$$

$\left\langle\rho_p\rho_n^2\right\rangle=(C_{n^2p}+1+2C_{np})\langle\rho_p\rangle\langle\rho_n\rangle^2$

$$
  \langle\delta\rho_p^2\delta\rho_n\rangle=\left\langle\rho_p^2\rho_n\right\rangle-2\langle\rho_p\rangle\left\langle\rho_p\rho_n\right\rangle+\langle\rho_p\rangle^2\langle\rho_n\rangle
$$

$$
  \begin{equation}
    C_{np^2}=\frac{\left\langle\rho_p^2\rho_n\right\rangle}{\langle\rho_p\rangle^2\langle\rho_n\rangle}-(1+2C_{np})
  \end{equation}
$$

$\left\langle\rho_p^2\rho_n\right\rangle=(C_{np^2}+1+2C_{np})\langle\rho_p\rangle^2\langle\rho_n\rangle$

$$
\begin{align*}
  \langle\delta\rho_p^2\delta\rho_n^2\rangle=&\left\langle\rho_p^2\rho_n^2\right\rangle-2\langle\rho_n\rangle\langle\rho_p^2\rho_n\rangle+\langle\rho_n\rangle^2\langle\rho_p^2\rangle-2\langle\rho_p\rangle\langle\rho_p\rho_n^2\rangle+4\langle\rho_p\rangle\langle\rho_n\rangle\langle\rho_p\rho_n\rangle\\
  &-2\langle\rho_p\rangle^2\langle\rho_n\rangle^2+\langle\rho_p\rangle^2\langle\rho_n^2\rangle-2\langle\rho_p\rangle^2\langle\rho_n\rangle^2+\langle\rho_p\rangle^2\langle\rho_n\rangle^2\\
  =&\left\langle\rho_p^2\rho_n^2\right\rangle-2\langle\rho_n\rangle\langle\rho_p^2\rho_n\rangle-2\langle\rho_p\rangle\langle\rho_p\rho_n^2\rangle+\langle\rho_n\rangle^2\langle\rho_p^2\rangle+\langle\rho_p\rangle^2\langle\rho_n^2\rangle\\
  &+4\langle\rho_p\rangle\langle\rho_n\rangle\langle\rho_p\rho_n\rangle-3\langle\rho_p\rangle^2\langle\rho_n\rangle^2\\
  =&\left\langle\rho_p^2\rho_n^2\right\rangle-2(C_{np^2}+1+2C_{np})\langle\rho_p\rangle^2\langle\rho_n\rangle^2-2(C_{n^2p}+1+2C_{np})\langle\rho_p\rangle^2\langle\rho_n\rangle^2\\
  &+\langle\rho_n\rangle^2\langle\rho_p^2\rangle+\langle\rho_p\rangle^2\langle\rho_n^2\rangle+4(1+C_{np})\langle\rho_p\rangle^2\langle\rho_n\rangle^2-3\langle\rho_p\rangle^2\langle\rho_n\rangle^2\\
  =&\left\langle\rho_p^2\rho_n^2\right\rangle-(2C_{np^2}+2C_{n^2p}+4C_{np}+3)\langle\rho_p\rangle^2\langle\rho_n\rangle^2+\langle\rho_n\rangle^2\langle\rho_p^2\rangle+\langle\rho_p\rangle^2\langle\rho_n^2\rangle
\end{align*}
$$

so
$$
  \begin{equation}
    C_{n^2p^2}=\frac{\left\langle\rho_p^2\rho_n^2\right\rangle}{\langle\rho_p\rangle^2\langle\rho_n\rangle^2}-(2C_{np^2}+2C_{n^2p}+4C_{np}+3)+\frac{\langle\rho_p^2\rangle}{\langle\rho_p\rangle^2}+\frac{\langle\rho_n^2\rangle}{\langle\rho_n\rangle^2}
  \end{equation}
$$
