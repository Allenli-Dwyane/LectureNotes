## Double-Sideband Amplitude Modulation

* Amplitude of the carrier is varied in proportion to the baseband(message) signal.

* ***Modulation:***
  $$
  message \quad signal:m(t)\\
  carrier \quad signal:cos(\omega_ct)\\
  modulated \quad signal:m(t)cos(\omega_ct)=\frac{1}{2}m(t)e^{-j\omega_c t}+\frac{1}{2}m(t)e^{j\omega_c t}\\
  Spectrum:M(\omega)\rightarrow\frac{1}{2}[M(\omega+\omega_c)+M(\omega-\omega_c)]
  $$

* ***Demodulation: Synchronous/Coherent demodulation***
  $$
  m(t)cos(\omega_ct)\times cos(\omega_ct)=\frac{1}{2}m(t)cos(2\omega_ct)+\frac{1}{2}m(t)\\
  spectrum:\frac{1}{4}[M(\omega+2\omega_c)+M(\omega-2\omega_c)]+\frac{1}{2}M{\omega}
  $$
  

## Amplitude Modulation

* ***Motivation:*** coherent demodulation of DSB-SC requires the receiver to generate a carrier. To simplify receiver, we use AM.

* ***Modulation:***
  $$
  Message \quad signal:m(t)\\
  Carrier \quad signal:cos(\omega_ct)\\
  Modulated signal:(A+m(t))cos(\omega_ct)\\
  Spectrum:M(\omega)\rightarrow\frac{1}{2}[M(\omega+\omega_c)+M(\omega-\omega_c)]+\frac{A}{2}[\delta(\omega+\omega_c)+\delta(\omega-\omega_c)]
  $$
  > Drawback: Extra transmit power

* ***Demodulation: Envelope detector***
  
  To ensure correct envelope detector, we must have
  $$
  A+m(t)>0 \quad for \quad all \quad t\\
  Define:\mu-Modulation\quad index,\mu=\frac{m_p}{A}\\
  $$

  Envelope detection requires that
  $$
  0\le\mu\le1
  $$

* ***Side Band and Carrier Power***
  
  * Advantage of envelope detection is achieved under the expense of extra energy
  $$
  \phi_{AM}(t)=Acos(\omega_ct)+m(t)cos(\omega_ct),where \quad Acos\omega_ct\rightarrow carrier,m(t)cos\omega_ct\Rightarrow sideband\\
  P_c=\frac{1}{T}\int_{\frac{T_c}{2}}^{\frac{T_c}{2}}A^2cos^2\omega_ctdt=\frac{A^2}{2},P_s=\frac{1}{2}\overline{m^2(t)}=\frac{1}{2}P_m\\
  $$
  * Power efficiency is as follows
  $$
  \eta=\frac{P_s}{P_c+P_s}=\frac{\overline{m^2(t)}}{A^2+\overline{m^2(t)}}\le\frac{1}{3}\\
  Given \quad that \quad when \quad m(t)=cos\omega_mt,\quad \eta \quad reaches \quad maximum
  $$

## Quadrature Amplitude Modulation
* ***Motivation:***
  
  Using DSB-SC,
  $$
  if \quad m(t) \quad real\rightarrow M(\omega)=M^*(-\omega)\\
  Modulated \quad signal \quad \varPhi(t) \quad real \rightarrow \varPhi(\omega)=\varPhi^*(-\omega)
  $$
  We can tell that **only half** of the frequency spectrum of **message signal** and **one fourth** of the frequency spectrum of the **modulated signal** carries information.

* ***Modulation:***
  $$
  basband \quad signals:m_1(t),m_2(t)\\
  Modulated \quad signal:\Phi(t)=m_1(t)cos\omega_ct+m_2(t)sin\omega_ct\\
  Spectrum: \Phi(\omega)=\frac{1}{2}(M_1(\omega-\omega_c)+M_1(\omega+\omega_c))+\frac{j}{2}(M_1(\omega-\omega_c)+M_1(\omega+\omega_c))
  $$
<div align=center>
<img src=./1.png style="zoom:60%;">
</div>

* ***Demodulation***
  $$
  Channel\quad 1:\Phi(t)2cos\omega_ct=2m_1(t)cos^2\omega_ct+2m_2(t)cos\omega_ct sin\omega_ct=m_1(t)+m_1(t)cos2\omega_ct+m_2(t)sin2\omega_ct\\
  Channel \quad 2:\Phi(t)2sin\omega_ct=2m_1(t)sin\omega_ct cos\omega_ct+2m_2(t)sin^2\omega_ct=m_1(t)sin2\omega_ct-m_2(t)cos2\omega_ct+m_2(t)sin2\omega_ct+m_2(t)
  $$

* ***Complex View of Modulation:***
  $$
  Message \quad signal:m(t)=m_1(t)+jm_2(t)\rightarrow M(\omega)\ne M*(-\omega)
  $$

  * This implies that both positive and negative spectra carry information.
  $$
  Carrier \quad signal:cos\omega_ct=Re\{e^{-j\omega_ct}\}\\
  Modulated \quad signal:Re\{m(t)e^{-j\omega_ct}\}=m_1(t)cos\omega_ct+m_2(t)sin\omega_ct\\
  Spectrum:\Phi(\omega)=F\{Re\{m(t)e^{-j\omega_ct}\}\}\\
  $$ 

  * ***Demodulation***:
  $$
  \Phi(t)\rightarrow\Phi(t)e^{j\omega_ct}\Rightarrow\Phi(\omega)\rightarrow\Phi(\omega+\omega_c)\rightarrow lowpass-filter\rightarrow\frac{1}{2}M(\omega)
  $$
  <center class="half">
  <img src=./2.png style="zoom:40%;">
  <img src=./3.png style="zoom:50%;">
  </center>

## Single Sideband Modulation

* ***Modulation:***
  $$
  Step \quad 1:m(t)cos\omega_ct\rightarrow\Phi(\omega)=\frac{1}{2}[M(\omega+\omega_c)+M(\omega-\omega_c)]\\
  Step \quad 2: Bandpass\quad filter \quad to \quad remove\quad either\quad the \quad LSB\quad or\quad USB.
  $$
  
* ***Hilbert Transform***
  $$
  Hilbert \quad tranform:H(\omega)=-jsgn(\omega)=\begin{cases}
  j&\omega\le0\\
  -j&\omega>0\\    
  \end{cases}\\
  H(\omega)\stackrel{F}{\leftrightarrow}h(t)=F^{-1}(-jsgn(\omega))=\frac{1}{\pi t}
  $$

* ***SSB Modulation via Hilbert Transform***
  * ***Modulation***:
  $$
  \Phi(t)=m(t)\cos{\omega_ct}+m_h(t)\sin{\omega_ct},m_h(t)=m(t)*h(t),h(t):Hilbert \quad transform\\
  \Rightarrow\Phi(\omega)=\frac{1}{2}[M(\omega+\omega_c)-jM_h(\omega+\omega_c)]+\frac{1}{2}[M(\omega-\omega_c)+jM_h(\omega-\omega_c)]
  $$
  <div align=center>
  <img src=./4.png style="zoom:50%;">
  </div>

  * ***Modulation Using Phase Shift***:
  <div align=center>
  <img src=./5.png style="zoom:40%;">
  </div>

  * ***Modulation Using Selective Filtering***:

  <div align=center>
  <img src=./6.png style="zoom:35%;">
  </div>

  *  ***Demodulation***:
  
  1. ***Coherent Demodulation***:

  $$
  \Phi(t)\cos{\omega_ct}=m(t)\cos^2{\omega_ct}+m_h(t)\sin{\omega_ct}\cos{\omega_ct}=\frac{1}{2}m(t)+\frac{1}{2}[m(t)\cos{2\omega_ct}+m_h(t)\sin{2\omega_ct}]
  $$

  2. ***Envelope Demodulation:***
  
  $$
  Acquirements:A\gg m^2(t)+m_h^2(t)\\
  \Phi(t)+A\cos{\omega_ct}=(A+m(t))\cos{\omega_ct}+m_h(t)\sin{\omega_ct}=K(t)[\cos{\theta_t}\cos{\omega_ct}+\sin{\theta_ta}\sin{\omega_ct}]\\
  K^2(t)=(A+m(t))^2+m_h^2(t)=A^2[1+\frac{2m(t)}{A}+\frac{m^2(t)+m_h^2(t)}{A^2}]\\
  \Rightarrow Envelope\approx\sqrt{1+\frac{2m(t)}{A}}-1\approx\frac{m(t)}{A}
  $$

## Vestigial Sideband Modulation

* ***Motivation:***
  
  It's hard to implement a bandpass filter with sharp edges.

* ***Modulation:***
  $$
  \Phi_{VSB}(\omega)=[M(\omega-\omega_c)+M(\omega+\omega_c)]H_i(\omega),H_i(\omega):transmitter \quad shaping\quad filter.
  $$

* ***Demodulation:***
  $$
  pass \quad 2\Phi_{VSB}(t)\cos{\omega_ct}\quad through\quad H_o(\omega),H_o(\omega):receiver \quad shaping \quad filter.\\
  Spectrum:[\Phi_{VSB}(\omega+\omega_c)+\Phi_{VSB}(\omega-\omega_c)]H_o{\omega}=M(\omega)[H_i(\omega)+H_i(\omega-\omega_c)]H_o(\omega)+high\quad frequency\quad terms\\
  Thus\quad we\quad require:[H_i(\omega+\omega_c)+H_i(\omega-\omega_c)]H_o(\omega)=1
  $$
  
  To simplify the filter used by the receiver, we want that
  $$
  H_i(\omega-\omega_c)+H_i(\omega+\omega_c)=1\quad for |\omega_c|<2\pi B\\
  \Rightarrow H_o(\omega)=1
  $$
  so that for the receiver, he only needs to do lowpass