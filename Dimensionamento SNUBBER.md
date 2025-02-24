# Dimensionamento Snubber

Un modo per eliminare i picchi e oscillazioni e controllare la pendenza delle transizioni di tensione è quello di inserire una rete RC di smorzamneto o "snubber".

La capacità di snubber $C_s$ deve essere più grande della capacità equivalente del circuito risonante ma la più piccola possibile in modo da minimizzare le perdite sulla resistenza.

La capaità parassita $C_p$ è legata alla porta di uscita dello switch

Il valore della resistenza di snubber $R_s$ deve essere prossimo al valore dell' impedenza parassita, alla risonanza.

La tecnica proposta propone di inserire dei componenti fittizi nel circuito  per poi deimensionarli dopo la sua realizzazione per via empirica.

## 1. Misura della frequenza caratteristica e $C_p$

Misurare la forma d'onda della tensione di switching e calcolare il periodo $t_1$.

Il periodo è funzione dei parassiti: $t_1=2*\pi*\sqrt{L_p C_p}$   

Cortocircuitare $R_s$ e variare $C_s$ sino a quando il periodo dell'oscillazione $t_2 = 2*t_1$.

Eq.1      $t_2=2*\pi*\sqrt{L_p(C_p+C_s)}$

Eq.1a     $C_p+C_s = 4C_p$

Eq.1b     $C_p=\frac{C_s}{3}$ 

Questo valore è quello ottimale dato che introduce uno smorzamento prossimo a $Q=1$.

## 2. Calcolo di $L_p$

Dall'Eq.1 si può calcolare $L_p=$

## 3. Determinazione di $R_s$

Per avere uno smorzamento prossimo a $Q=1$ bisogna impostare $R_s=Z_0=\sqrt{\frac{L_p}{C_p} } $ 
