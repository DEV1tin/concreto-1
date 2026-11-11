# Mapeamento dos Formulários — Concreto I

Arquivo de referência paralelo aos três PDFs de formulário da prova (`A` a `BN`) para identificação rápida por código durante a resolução de exercícios.

---

## Índice Rápido

| Código | Formulário | Posição na Folha | Título |
| :---: | :---: | :--- | :--- |
| **A** | Form. 1 | Topo esquerdo | Combinações Últimas (ELU) |
| **B** | Form. 1 | Topo direito | Combinações de Serviço (ELS) |
| **C** | Form. 1 | Meio esquerdo (sup.) | Coeficientes de ponderação de ações permanentes diretas ($\gamma_g$) |
| **D** | Form. 1 | Meio direito (1ª tabela) | Coeficientes de ponderação de ações permanentes indiretas ($\gamma_{\varepsilon g}$) |
| **E** | Form. 1 | Meio direito (2ª tabela) | Coeficientes de ponderação de ações variáveis diretas ($\gamma_q$) |
| **F** | Form. 1 | Meio esquerdo (inf.) | Fatores de combinação e redução ($\psi_0, \psi_1, \psi_2$) |
| **G** | Form. 1 | Meio direito (3ª tabela) | Coeficientes de ponderação de ações variáveis indiretas ($\gamma_{\varepsilon q}$) |
| **H** | Form. 1 | Meio direito (4ª tabela) | Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$) e $f_{cd}, f_{yd}$ |
| **I** | Form. 1 | Vigas, coluna esq. (sup.) | Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`) |
| **J** | Form. 1 | Vigas, topo centro-dir. | Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`) |
| **K** | Form. 1 | Vigas, centro | Viga apoiada-engastada com carga distribuída parcial $w$ em $a$ |
| **L** | Form. 1 | Vigas, direita | Viga apoiada-engastada com momento concentrado $M$ (`AE10-m`) |
| **M** | Form. 1 | Vigas, 3ª faixa | Viga contínua de 2 vãos com carga distribuída $w$ no 1º vão ($a$) |
| **N** | Form. 1 | Vigas, 4ª faixa | Viga contínua de 2 vãos com carga distribuída $w$ no 2º vão ($L-a$) |
| **O** | Form. 1 | Vigas, faixa inferior | Viga contínua de 2 vãos com carga distribuída $w$ nos dois vãos |
| **P** | Form. 2 | Topo esquerdo | Limite de ductilidade / profundidade relativa limite da linha neutra ($\beta_{x,lim}$) |
| **Q** | Form. 2 | Topo centro | Parâmetro $\zeta_c$ do diagrama retangular simplificado |
| **R** | Form. 2 | Topo direito | Módulo resistente ($W_0$) e momento solicitante mínimo ($M_{sd,min}$) |
| **S** | Form. 2 | Coluna esq., 2º bloco | Variáveis adimensionais de flexão para seção retangular ($\beta_x, \beta_z, \beta_y, \beta_s, \beta'_s, \beta_c$) |
| **T** | Form. 2 | Centro, 2º bloco | Fator de tensão de compressão no concreto ($\alpha_c$) |
| **U** | Form. 2 | Centro, 3º bloco | Resistência característica à tração superior do concreto ($f_{ctk,sup}$) |
| **V** | Form. 2 | Centro-dir., abaixo de U/R | Momento resistente de cálculo limite para armadura simples ($M_{rd,lim}$) |
| **W** | Form. 2 | Coluna esq., 3º bloco | Parâmetro redutor $\eta_c$ conforme geometria da zona comprimida |
| **X** | Form. 2 | Centro-dir., abaixo de V | Cálculo de armadura longitudinal para seção retangular ($A_s, A'_s, M'_{rd}$) |
| **Y** | Form. 2 | Faixa 4, esquerda | Número necessário de barras longitudinais ($n_{\phi_\ell}, n'_{\phi'_\ell}$) |
| **Z** | Form. 2 | Faixa 4, centro | Número máximo de barras por camada na largura $b_w$ |
| **AA** | Form. 2 | Faixa 4, direita | Taxa geométrica mínima de armadura de tração ($\rho_{min}$) |
| **AB** | Form. 2 | Faixa 5, esquerda | Verificação de $\beta_x$ a partir das áreas efetivas (seção retangular) |
| **AC** | Form. 2 | Faixa 5, centro | Taxa geométrica máxima de armadura longitudinal ($\rho_{max}$) |
| **AD** | Form. 2 | Faixa 5, direita | Ajuste de armaduras quando $\rho_{min} < 0{,}15\%$ |
| **AE** | Form. 2 | Faixa 6, esquerda | Centro de gravidade das camadas de armadura ($y_s, y'_s$) |
| **AF** | Form. 2 | Faixa 6, centro-esq. | Espaçamentos livres mínimos entre barras ($a_h, a_v$) |
| **AG** | Form. 2 | Faixa 6, centro-dir. | Áreas efetivas de aço ($A_{s,ef}, A'_{s,ef}$) |
| **AH** | Form. 2 | Faixa 6, direita | Resistências de cálculo ($f_{cd}, f_{yd}$) |
| **AI** | Form. 2 | Bloco inf. esq. (tabela) | Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$) |
| **AJ** | Form. 2 | Bloco inf. esq. (abaixo de AI) | Alturas úteis ($d, d'$) |
| **AK** | Form. 2 | Bloco inf. esq. (ao lado de AJ) | Módulo de elasticidade do aço ($E_s$) |
| **AL** | Form. 2 | Bloco inf. esq. (abaixo de AJ/AK) | Deformação última de encurtamento do concreto ($\varepsilon_{cu}$) |
| **AM** | Form. 2 | Bloco inf. direito | Dimensionamento e verificação de Seção T ($M_{rdf}, M_{rda}, M_{sd}, A_s, \beta_x$) |
| **AN** | Form. 2 | Vigas, 1ª coluna | Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`) |
| **AO** | Form. 2 | Vigas, 2ª coluna | Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`) |
| **AP** | Form. 2 | Vigas, 3ª coluna | Viga apoiada-engastada com momento concentrado $M$ (`AE10-m`) |
| **AQ** | Form. 2 | Vigas, 4ª coluna | Viga biapoiada com balanço e carga distribuída total $w$ (`VB1-w`) |
| **AR** | Form. 3 | Topo esquerdo | Condições de segurança ao cisalhamento ($V_{sd} \le V_{rdc}, V_{sd} \le V_{rdw}$) |
| **AS** | Form. 3 | Topo centro | Parcela resistente pelos mecanismos complementares ($V_{c,I}, V_{c,II}$) |
| **AT** | Form. 3 | Topo direito | Força cortante resistente por tração na diagonal ($V_{rdw} = V_c + V_{sw}$) |
| **AU** | Form. 3 | Faixa 2, esquerda | Força cortante resistente das diagonais comprimidas ($V_{rdc}, V_{rdc,I}, V_{rdc,II}$) |
| **AV** | Form. 3 | Faixa 2, direita | Força cortante resistente pela armadura transversal ($V_{sw}, V_{sw,I}, V_{sw,II}$) |
| **AW** | Form. 3 | Faixa 3, esquerda | Resistência característica à tração inferior do concreto ($f_{ctk,inf}$) |
| **AX** | Form. 3 | Faixa 3, centro-esq. | Resistência de cálculo à tração direta do concreto ($f_{ctd}$) |
| **AY** | Form. 3 | Faixa 3, centro-dir. | Taxa / relação mínima de armadura transversal ($\left(A_{sw}/s\right)_{min}$) |
| **AZ** | Form. 3 | Faixa 3, direita | Limites de diâmetro dos estribos ($5\text{ mm} \le \phi_t \le b_w/10$) |
| **BA** | Form. 3 | Faixa 4 (largura total) | Espaçamentos mínimo e máximo entre estribos ($s$) |
| **BB** | Form. 3 | Meio esquerdo (esquemas) | Reduções de $V_{sd}$ junto aos apoios ($d/2$ e $a \le 2d$) |
| **BC** | Form. 3 | Meio direito (tabela sup.) | Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$) |
| **BD** | Form. 3 | Meio direito (abaixo de BC, esq.) | Resistências de cálculo ($f_{cd}, f_{yd}$) |
| **BE** | Form. 3 | Meio direito (abaixo de BC, dir.) | Área efetiva de um estribo ($A_{sw,ef} = n_r \cdot 0{,}25\pi\phi_t^2$) |
| **BF** | Form. 3 | Meio direito (bloco inf., esq.) | Verificação da relação efetiva ($A_{sw,ef}/s_{ef} \ge A_{sw}/s$) |
| **BG** | Form. 3 | Meio direito (bloco inf., dir.) | Tensão limite de cálculo na armadura transversal ($f_{ywd} = 435\text{ MPa}$) |
| **BH** | Form. 3 | Abaixo dos esquemas, esq. | Cortante solicitante mínimo para armadura mínima ($V_{sd,min,I}, V_{sd,min,II}$) |
| **BI** | Form. 3 | Abaixo de BF/BG, dir. | Espaçamento efetivo máximo dos estribos ($s_{ef,I}, s_{ef,II}$) |
| **BJ** | Form. 3 | Faixa intermediária (largura total) | Viga apoiada-engastada com dois momentos concentrados $M$ (`AE11-mo`) |
| **BK** | Form. 3 | Vigas, 1ª coluna | Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`) |
| **BL** | Form. 3 | Vigas, 2ª coluna | Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`) |
| **BM** | Form. 3 | Vigas, 3ª coluna | Viga biengastada com carga distribuída total $w$ (`BE1-w`) |
| **BN** | Form. 3 | Vigas, 4ª coluna | Viga biapoiada com balanço e carga distribuída total $w$ (`VB1-w`) |

---

## Formulário 1 — Combinações e Vigas (`Formulario-a-Combinacoes-2022-1.pdf`)

### [A] Combinações Últimas (ELU)
- **Localização:** Formulário 1 — Topo esquerdo.
- **Descrição:** Expressões gerais das combinações de ações no Estado Limite Último (normais, especiais/de construção e excepcionais). O operador $\biguplus$ indica união disjunta dos efeitos das ações de cálculo (ponderando cada carregamento separadamente quando têm posições/distribuições diferentes).

$$F_{d,nor} := \left(\biguplus \gamma_g F_{gk}\right) \uplus \left(\biguplus \gamma_{\varepsilon g} F_{\varepsilon gk}\right) \uplus \gamma_q F_{q1k} \uplus \left(\biguplus \gamma_q \psi_{0j} F_{qjk}\right) \uplus \left(\biguplus \gamma_{\varepsilon q} \psi_{0\varepsilon} F_{\varepsilon qk}\right)$$

$$F_{d,esp} := \left(\biguplus \gamma_g F_{gk}\right) \uplus \left(\biguplus \gamma_{\varepsilon g} F_{\varepsilon gk}\right) \uplus \gamma_q F_{q1k} \uplus \left(\biguplus \gamma_q \psi_{0j} F_{qjk}\right) \uplus \left(\biguplus \gamma_{\varepsilon q} \psi_{0\varepsilon} F_{\varepsilon qk}\right)$$

$$F_{d,exc} := \left(\biguplus \gamma_g F_{gk}\right) \uplus F_{q1exc} \uplus \left(\biguplus \gamma_q \psi_{0j} F_{qjk}\right)$$

---

### [B] Combinações de Serviço (ELS)
- **Localização:** Formulário 1 — Topo direito.
- **Descrição:** Expressões das combinações de ações no Estado Limite de Serviço: quase permanentes ($F_{d,qp}$), frequentes ($F_{d,f}$) e raras ($F_{d,r}$). Não se aplicam coeficientes de ponderação $\gamma$, apenas fatores de redução $\psi_1$ e $\psi_2$.

$$F_{d,qp} := \left(\biguplus F_{gk}\right) \uplus \left(\biguplus \psi_{2j} F_{qjk}\right)$$

$$F_{d,f} := \left(\biguplus F_{gk}\right) \uplus \psi_1 F_{q1k} \uplus \left(\biguplus \psi_{2j} F_{qjk}\right)$$

$$F_{d,r} := \left(\biguplus F_{gk}\right) \uplus F_{q1k} \uplus \left(\biguplus \psi_{1j} F_{qjk}\right)$$

---

### [C] Coeficientes de ponderação de ações permanentes diretas ($\gamma_g$)
- **Localização:** Formulário 1 — Meio esquerdo (tabela superior).
- **Descrição:** Valores de $\gamma_g$ para combinações normais, especiais e excepcionais. O valor sem parênteses aplica-se no sentido **desfavorável** e o valor entre parênteses no sentido **favorável**. Notas das alíneas: *(a)* elementos pré-moldados com fim estrutural; *(b)* estruturas convencionais de concreto armado moldadas no local; *(c)* elementos industrializados sem fim estrutural já acabados (ex.: gesso acartonado, painéis acabados); *(d)* industrializados sem fim estrutural com acabamentos *in loco* (ex.: alvenaria pré-fabricada sem revestimento); *(e)* alvenarias com revestimento, contrapisos e equipamentos fixos.

| Natureza da ação | Normal | Especial | Excep. |
| :--- | :---: | :---: | :---: |
| Peso próprio de estruturas metálicas | 1,25 (1,00) | 1,15 (1,00) | 1,10 (1,00) |
| Peso próprio de estruturas pré-moldadas$^{a)}$ | 1,30 (1,00) | 1,20 (1,00) | 1,15 (1,00) |
| Peso próprio de estruturas moldadas no local$^{b)}$, de elementos construtivos industrializados$^{c)}$ e empuxos permanentes | 1,35 (1,00) | 1,25 (1,00) | 1,15 (1,00) |
| Peso próprio de elementos construtivos industrializados com adições *in loco*$^{d)}$ | 1,40 (1,00) | 1,30 (1,00) | 1,20 (1,00) |
| Peso próprio de elementos construtivos em geral e equipamentos$^{e)}$ | 1,50 (1,00) | 1,40 (1,00) | 1,30 (1,00) |

---

### [D] Coeficientes de ponderação de ações permanentes indiretas ($\gamma_{\varepsilon g}$)
- **Localização:** Formulário 1 — Meio direito (1ª tabela).
- **Descrição:** Valores de $\gamma_{\varepsilon g}$ para ações permanentes indiretas. Sem parênteses: sentido **desfavorável**; entre parênteses: sentido **favorável**.

| Natureza da ação | Normal | Especial | Excep. |
| :--- | :---: | :---: | :---: |
| Retração e fluência | 1,20 (0,00) | 1,20 (0,00) | 0,00 (0,00) |
| Deslocamento de apoio | 1,20 (0,00) | 1,20 (0,00) | 0,00 (0,00) |
| Protensão | 1,2 (0,90) | 1,20 (0,90) | 1,20 (0,90) |
| Imperfeições geométricas | 1,20 (0,00) | 1,20 (0,00) | 0,00 (0,00) |

---

### [E] Coeficientes de ponderação de ações variáveis diretas ($\gamma_q$)
- **Localização:** Formulário 1 — Meio direito (2ª tabela).
- **Descrição:** Valores de $\gamma_q$ no sentido **desfavorável** (no sentido favorável, ações variáveis assumem $0{,}00$). Notas: *(a)* empuxos de água/líquidos em reservatórios, tanques, decantadores; *(b)* ações com máximo limitado por dispositivo físico.

| Natureza da ação | Normal | Especial | Excep. |
| :--- | :---: | :---: | :---: |
| Ações decorrentes do uso e ocupação | 1,50 | 1,30 | 1,0 |
| Ação do vento | 1,40 | 1,20 | 0,00 |
| Ação da água$^{a)}$ | 1,20 | 1,20 | 1,20 |
| Ações truncadas$^{b)}$ | 1,20 | 1,10 | 0,00 |
| Demais ações variáveis | 1,50 | 1,30 | 1,00 |

---

### [F] Fatores de combinação e redução de ações variáveis ($\psi_0, \psi_1, \psi_2$)
- **Localização:** Formulário 1 — Meio esquerdo (tabela inferior).
- **Descrição:** Fatores para simultaneidade de ações variáveis: $\psi_0$ (ELU, ações secundárias), $\psi_1$ (ELS frequente e secundárias na rara) e $\psi_2$ (ELS quase permanente e secundárias na frequente).

| Natureza da ação | Ocorrência | $\psi_0$ | $\psi_1$ | $\psi_2$ |
| :--- | :--- | :---: | :---: | :---: |
| Cargas acidentais de edifícios | Edificações residenciais, de acesso restrito | 0,5 | 0,4 | 0,3 |
| Cargas acidentais de edifícios | Edificações comerciais, de escritórios de acesso público | 0,7 | 0,6 | 0,4 |
| Cargas acidentais de edifícios | Bibliotecas, arquivos, depósitos, oficinas e garagens | 0,8 | 0,7 | 0,6 |
| Vento | Pressão dinâmica do vento nas estruturas em geral | 0,6 | 0,3 | 0,0 |
| Temperatura | Variações uniformes de temperatura em relação à média anual local | 0,6 | 0,5 | 0,3 |
| Passarelas e pontes | Passarelas de pedestre | 0,6 | 0,4 | 0,3 |
| Passarelas e pontes | Pontes rodoviárias | 0,7 | 0,5 | 0,3 |
| Passarelas e pontes | Pontes ferroviárias não especializadas | 1,0 | 0,7 | 0,5 |
| Passarelas e pontes | Pontes ferroviárias especializadas | 1,0 | 1,0 | 0,6 |
| Passarelas e pontes | Vigas de rolamento de pontes rolantes | 1,0 | 0,8 | 0,5 |

---

### [G] Coeficientes de ponderação de ações variáveis indiretas ($\gamma_{\varepsilon q}$)
- **Localização:** Formulário 1 — Meio direito (3ª tabela).
- **Descrição:** Valores de $\gamma_{\varepsilon q}$ para efeito da temperatura (variações uniformes e não uniformes) no sentido desfavorável.

| Natureza da ação | Normal | Especial | Excep. |
| :--- | :---: | :---: | :---: |
| Efeito da temperatura | 1,20 | 1,00 | 0,0 |

---

### [H] Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$) e resistências de cálculo ($f_{cd}, f_{yd}$)
- **Localização:** Formulário 1 — Meio direito (4ª tabela).
- **Descrição:** Coeficientes minoradores da resistência do concreto ($\gamma_c$) e do aço ($\gamma_s$) em ELU e ELS, acompanhados das definições de resistência de cálculo $f_{cd}$ e $f_{yd}$.

| Estado Limite | Combinações | $\gamma_c$ | $\gamma_s$ |
| :--- | :--- | :---: | :---: |
| **E.L.U.** | Normais | 1,40 | 1,15 |
| **E.L.U.** | Especiais ou de construção | 1,20 | 1,15 |
| **E.L.U.** | Excepcionais | 1,20 | 1,00 |
| **E.L.S.** | — | 1,00 | 1,00 |

$$f_{cd} = \frac{f_{ck}}{\gamma_c} \qquad f_{yd} = \frac{f_{yk}}{\gamma_s}$$

---

### [I] Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`)
- **Localização:** Formulário 1 — Parte inferior, bloco esquerdo superior (corresponde ao bloco **[AN]** `AE1-w` do Formulário 2).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), submetida a carregamento distribuído uniforme $w$ em todo o vão ($0 \le x \le L$). Possui trecho único $A$.

$$M_A = \frac{wx(3L - 4x)}{8} \qquad V_A = \frac{w(3L - 8x)}{8}$$

$$R_1 = \frac{3Lw}{8} \qquad R_2 = \frac{5Lw}{8} \qquad M_2 = -\frac{L^2 w}{8}$$

---

### [J] Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`)
- **Localização:** Formulário 1 — Parte inferior, bloco superior direito (corresponde ao bloco **[AO]** `AE8-fa` do Formulário 2).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com força concentrada vertical $F$ aplicada à distância $a$ do apoio esquerdo. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{Fx\left(2L^3 - 3L^2 a + a^3\right)}{2L^3} \qquad M_B = \frac{Fa\left(2L^3 - 3L^2 x + a^2 x\right)}{2L^3}$$

$$V_A = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad V_B = \frac{Fa\left(-3L^2 + a^2\right)}{2L^3}$$

$$R_1 = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad R_2 = \frac{Fa\left(3L^2 - a^2\right)}{2L^3} \qquad M_2 = \frac{Fa\left(-L^2 + a^2\right)}{2L^2}$$

---

### [K] Viga apoiada-engastada com carga distribuída parcial $w$ em $a$
- **Localização:** Formulário 1 — Parte inferior, bloco central.
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com carregamento distribuído uniforme $w$ apenas de $x=0$ até $x=a$. Trecho $A$: $0 \le x \le a$ (carregado); Trecho $B$: $a \le x \le L$ (descarregado).

$$M_A = \frac{wx\left(8L^3 a - 4L^3 x - 6L^2 a^2 + a^4\right)}{8L^3} \qquad M_B = \frac{a^2 w\left(4L^3 - 6L^2 x + a^2 x\right)}{8L^3}$$

$$V_A = aw - wx - \frac{3a^2 w}{4L} + \frac{a^4 w}{8L^3} \qquad V_B = \frac{a^2 w\left(-6L^2 + a^2\right)}{8L^3}$$

$$R_1 = \frac{aw\left(8L^3 - 6L^2 a + a^3\right)}{8L^3} \qquad R_2 = \frac{a^2 w\left(6L^2 - a^2\right)}{8L^3} \qquad M_2 = -\frac{a^2 w}{4} + \frac{a^4 w}{8L^2}$$

---

### [L] Viga apoiada-engastada com momento concentrado $M$ (`AE10-m`)
- **Localização:** Formulário 1 — Parte inferior, coluna direita (corresponde ao bloco **[AP]** `AE10-m` do Formulário 2).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com momento fletor concentrado $M$ (sentido anti-horário no esquema) aplicado à distância $a$ do apoio esquerdo. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$. *(Atenção: neste PDF de 2022, $V_B$ está impresso igual a $R_2$; no Formulário 2 de 2024, bloco **[AP]**, foi corrigido para $V_B = \frac{3M(-L^2 + a^2)}{2L^3}$.)*

$$M_A = \frac{3Mx\left(-L^2 + a^2\right)}{2L^3} \qquad M_B = M - \frac{3Mx}{2L} + \frac{3Ma^2 x}{2L^3}$$

$$V_A = R_1 = \frac{3M\left(-L^2 + a^2\right)}{2L^3} \qquad V_B = R_2 = \frac{3M\left(L^2 - a^2\right)}{2L^3} \qquad M_2 = \frac{M\left(-L^2 + 3a^2\right)}{2L^2}$$

---

### [M] Viga contínua de 2 vãos com carga distribuída $w$ no 1º vão ($a$)
- **Localização:** Formulário 1 — Parte inferior, 3ª faixa (esquerda até o bloco **[L]**).
- **Descrição:** Viga contínua de comprimento total $L$ sobre três apoios ($R_1$ em $x=0$, $R_2$ em $x=a$, $R_3$ em $x=L$), com carregamento distribuído uniforme $w$ somente no primeiro vão ($0 \le x \le a$). Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{wx\left(4La - 4Lx - a^2\right)}{8L} \qquad M_B = \frac{a^3 w(-L + x)}{8L(L - a)}$$

$$V_A = \frac{aw}{2} - wx - \frac{a^2 w}{8L} \qquad V_B = \frac{a^3 w}{8L(L - a)}$$

$$R_1 = \frac{aw(4L - a)}{8L} \qquad R_2 = \frac{aw(-4L + 3a)}{8(-L + a)} \qquad R_3 = \frac{a^3 w}{8L(-L + a)}$$

---

### [N] Viga contínua de 2 vãos com carga distribuída $w$ no 2º vão ($L - a$)
- **Localização:** Formulário 1 — Parte inferior, penúltima faixa (largura total).
- **Descrição:** Viga contínua de comprimento total $L$ sobre três apoios ($R_1$ em $x=0$, $R_2$ em $x=a$, $R_3$ em $x=L$), com carregamento distribuído uniforme $w$ somente no segundo vão ($a \le x \le L$). Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{wx\left(-L^3 + 3L^2 a - 3La^2 + a^3\right)}{8La} \qquad M_B = \frac{w\left(L\left(-L^2 - 2La + 5Lx - a^2 + 2ax - 4x^2\right) + a^2 x\right)}{8L}$$

$$V_A = \frac{w\left(-L^3 + 3L^2 a - 3La^2 + a^3\right)}{8La} \qquad V_B = \frac{w\left(5L^2 + 2La - 8Lx + a^2\right)}{8L}$$

$$R_1 = \frac{w\left(-L^3 + 3L^2 a - 3La^2 + a^3\right)}{8La} \qquad R_2 = \frac{w\left(L^2 + 2La - 3a^2\right)}{8a} \qquad R_3 = \frac{w\left(3L^2 - 2La - a^2\right)}{8L}$$

---

### [O] Viga contínua de 2 vãos com carga distribuída $w$ nos dois vãos
- **Localização:** Formulário 1 — Parte inferior, última faixa (largura total).
- **Descrição:** Viga contínua de comprimento total $L$ sobre três apoios ($R_1$ em $x=0$, $R_2$ em $x=a$, $R_3$ em $x=L$), com carregamento distribuído uniforme $w$ ao longo de todo o comprimento $L$. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{wx\left(-L^2 + 3La + a^2 - 4ax\right)}{8a} \qquad M_B = \frac{w\left(-L^3 - L^2 a + 5L^2 x + La^2 - 3Lax - 4Lx^2 - a^2 x + 4ax^2\right)}{8(L - a)}$$

$$V_A = \frac{w\left(-L^2 + 3La + a^2 - 8ax\right)}{8a} \qquad V_B = \frac{w\left(5L^2 - 3La - 8Lx - a^2 + 8ax\right)}{8(L - a)}$$

$$R_1 = \frac{w\left(-L^2 + 3La + a^2\right)}{8a} \qquad R_2 = \frac{Lw\left(-L^2 - La + a^2\right)}{8a(-L + a)} \qquad R_3 = \frac{w\left(-3L^2 + 5La - a^2\right)}{8(-L + a)}$$

---

## Formulário 2 — Armadura Simples, Dupla e Seção T (`Formulario-ArmaduraSimplesDuplaT-2024-1.pdf`)

### [P] Limite de ductilidade / profundidade relativa limite da linha neutra ($\beta_{x,lim}$)
- **Localização:** Formulário 2 — Topo esquerdo.
- **Descrição:** Limite normativo da relação $x/d$ para garantir condições adequadas de ductilidade na flexão simples de vigas (separa o regime de armadura simples do regime de armadura dupla quando $\beta_x > \beta_{x,lim}$).

$$\beta_{x,lim} = \begin{cases} 0{,}450 & f_{ck} \le 50\text{ MPa} \\ 0{,}350 & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [Q] Parâmetro $\zeta_c$ do diagrama retangular simplificado
- **Localização:** Formulário 2 — Topo centro.
- **Descrição:** Razão $\zeta_c = y/x$ entre a altura do bloco retangular equivalente de tensões de compressão no concreto ($y$) e a profundidade da linha neutra ($x$).

$$\zeta_c = \begin{cases} 0{,}8 & f_{ck} \le 50\text{ MPa} \\ 0{,}8 - \dfrac{f_{ck} - 50}{400} & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [R] Módulo resistente ($W_0$) e momento solicitante mínimo ($M_{sd,min}$)
- **Localização:** Formulário 2 — Topo direito.
- **Descrição:** Cálculo do módulo de resistência à flexão em relação à fibra mais tracionada ($W_0$) para seções **T** (com aba $b_f \times h_f$ e alma $b_w \times h$) e seções **retangulares**, usado para obter o momento fletor mínimo de dimensionamento $M_{sd,min}$.

$$W_0 = \frac{A_w}{3c}\left(h^2 + 3c^2\right) + \frac{A_a}{3c}\left(h_f^2 + 3c'^2\right) \quad \text{(T)}$$

$$A_w = b_w h \qquad A_a = (b_f - b_w) h_f \qquad A_T = A_w + A_a$$

$$c = \frac{A_w h}{2 A_T} + \frac{A_a}{2 A_T}(2h - h_f) \qquad c' = h - c$$

$$W_0 = \frac{b_w h^2}{6} \quad \text{(retangulares)} \qquad M_{sd,min} = 0{,}8\, W_0\, f_{ctk,sup}$$

---

### [S] Variáveis adimensionais de flexão para seção retangular
- **Localização:** Formulário 2 — Coluna esquerda, 2º bloco.
- **Descrição:** Conjunto de variáveis adimensionais para dimensionamento na flexão simples sem uso de tabelas: posição relativa da linha neutra ($\beta_x = x/d$), braço de alavanca relativo ($\beta_z = z/d$), altura relativa comprimida ($\beta_y$), fatores de tensão nas armaduras tracionada ($\beta_s = \sigma_{sd}/f_{yd} \le 1{,}0$) e comprimida ($\beta'_s = \sigma'_{sd}/f_{yd} \le 1{,}0$) e momento adimensional reduzido ($\beta_c$). Usar $\varepsilon_{cu}$ em valor absoluto adimensional (ex.: $3{,}5\times 10^{-3}$) compatível com $E_s/f_{yd}$.

$$\beta_x = \frac{1}{\zeta_c} - \frac{1}{\zeta_c}\sqrt{1 - \frac{2 M_{rdw}}{\eta_c b_w d^2 f_{cd}}}$$

$$\beta_z = \frac{z}{d} = 1 - 0{,}5\,\beta_y \qquad \beta_y = \zeta_c \beta_x$$

$$\beta_s = \frac{E_s}{f_{yd}}\left(\frac{1 - \beta_x}{\beta_x}\right)\varepsilon_{cu} \le 1{,}0$$

$$\beta'_s = \frac{E_s}{f_{yd}}\left(\frac{\beta_x - \dfrac{d'}{d}}{\beta_x}\right)\varepsilon_{cu} \le 1{,}0$$

$$\beta_c = \eta_c \zeta_c \beta_x \beta_z = \frac{M_{rdw}}{b_w d^2 f_{cd}}$$

---

### [T] Fator de tensão de compressão no concreto ($\alpha_c$)
- **Localização:** Formulário 2 — Centro, 2º bloco (abaixo de **[Q]**).
- **Descrição:** Fator multiplicador da resistência de cálculo $f_{cd}$ no diagrama retangular simplificado de tensões de compressão do concreto.

$$\alpha_c = \begin{cases} 0{,}85 & f_{ck} \le 50\text{ MPa} \\ 0{,}85\left[1{,}0 - \dfrac{f_{ck} - 50}{200}\right] & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [U] Resistência característica à tração superior do concreto ($f_{ctk,sup}$)
- **Localização:** Formulário 2 — Centro, 3º bloco (abaixo de **[T]**).
- **Descrição:** Resistência característica superior do concreto à tração direta (em MPa para $f_{ck}$ em MPa), utilizada no cálculo de $M_{sd,min}$ em **[R]**.

$$f_{ctk,sup} = \begin{cases} 0{,}39 \sqrt[3]{f_{ck}^2} & f_{ck} \le 50\text{ MPa} \\ 2{,}756 \ln(1 + 0{,}11 f_{ck}) & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [V] Momento resistente de cálculo limite para armadura simples ($M_{rd,lim}$)
- **Localização:** Formulário 2 — Centro-direita, abaixo de **[U]** e **[R]**.
- **Descrição:** Máximo momento fletor que a seção retangular (ou a alma $b_w$ da viga T) resiste apenas com armadura tracionada respeitando $\beta_{x,lim}$ (e considerando $\eta_c = \alpha_c$). Se $M_{sd} > M_{rd,lim}$ (ou $M_{sd} - M_{rda} > M_{rd,lim}$ na viga T), é necessária armadura dupla.

$$M_{rd,lim} = \begin{cases} 0{,}251\, b_w d^2 f_{cd} & f_{ck} \le 50\text{ MPa} \\ \zeta_c b_w d^2 (0{,}298 - 0{,}052 \zeta_c)\left[1{,}0 - \dfrac{f_{ck} - 50}{200}\right] f_{cd} & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [W] Parâmetro redutor $\eta_c$ conforme geometria da zona comprimida
- **Localização:** Formulário 2 — Coluna esquerda, 3º bloco (abaixo de **[S]**).
- **Descrição:** Coeficiente $\eta_c$ aplicado à tensão máxima do diagrama retangular do concreto. Mantém-se $\eta_c = \alpha_c$ quando a largura da zona comprimida não diminui em direção à borda mais comprimida (diagrama superior, trapézio mais largo no lado comprimido); reduz-se para $\eta_c = 0{,}9\alpha_c$ quando a largura diminui em direção à borda mais comprimida (diagrama inferior, trapézio mais estreito no lado comprimido).

$$\eta_c = \alpha_c \quad \text{(largura constante ou maior na borda mais comprimida)}$$

$$\eta_c = 0{,}9\,\alpha_c \quad \text{(largura decrescente em direção à borda mais comprimida)}$$

---

### [X] Cálculo de armadura longitudinal para seção retangular ($A_s, A'_s, M'_{rd}$)
- **Localização:** Formulário 2 — Centro-direita, abaixo de **[V]**.
- **Descrição:** Áreas necessárias de armadura de tração ($A_s$) e de compressão ($A'_s$) para seção retangular. Na **armadura simples**, adota-se $M_{rdw} = M_{sd}$ e $M'_{rd} = 0$ ($A'_s = 0$). Na **armadura dupla**, adota-se $M_{rdw} = M_{rd,lim}$ (com $\beta_x = \beta_{x,lim}$), $M'_{rd} = M_{sd} - M_{rd,lim}$ e calcula-se $\beta_s, \beta'_s$ em $\beta_{x,lim}$.

$$A_s = \left[\frac{M_{rdw}}{\beta_z d} + \frac{M'_{rd}}{(d - d')}\right] \frac{1}{\beta_s f_{yd}} \qquad A'_s = \frac{M'_{rd}}{(d - d')\,\beta'_s f_{yd}} \qquad M'_{rd} = M_{sd} - M_{rd,lim}$$

---

### [Y] Número necessário de barras longitudinais ($n_{\phi_\ell}, n'_{\phi'_\ell}$)
- **Localização:** Formulário 2 — Faixa 4, esquerda.
- **Descrição:** Quantidade inteira mínima de barras (arredondamento para cima, função teto $\lceil \cdot \rceil$) necessária para atender às áreas calculadas de tração ($A_s$) e compressão ($A'_s$), escolhidos os diâmetros $\phi_\ell$ e $\phi'_\ell$.

$$n_{\phi_\ell} = \left\lceil \frac{4 A_s}{\pi \phi_\ell^2} \right\rceil \qquad n'_{\phi'_\ell} = \left\lceil \frac{4 A'_s}{\pi \phi_\ell'^2} \right\rceil$$

---

### [Z] Número máximo de barras por camada na largura $b_w$
- **Localização:** Formulário 2 — Faixa 4, centro.
- **Descrição:** Quantidade inteira máxima de barras (arredondamento para baixo, função piso $\lfloor \cdot \rfloor$) que cabem em uma única camada horizontal dentro da largura da alma $b_w$, descontando cobrimento nominal ($c_{nom}$), diâmetro do estribo ($\phi_t$ / $\phi'_t$) e respeitando o espaçamento horizontal mínimo $a_h$.

$$n_{\phi_\ell} \le \left\lfloor \frac{b_w - 2 c_{nom} - 2 \phi_t + a_h}{\phi_\ell + a_h} \right\rfloor \qquad n'_{\phi'_\ell} \le \left\lfloor \frac{b_w - 2 c_{nom} - 2 \phi'_t + a_h}{\phi'_\ell + a_h} \right\rfloor$$

---

### [AA] Taxa geométrica mínima de armadura de tração ($\rho_{min}$)
- **Localização:** Formulário 2 — Faixa 4, direita.
- **Descrição:** Verificação da taxa mínima absoluta de armadura longitudinal de tração em relação à área da seção de concreto ($A_c$).

$$\rho_{min} = \frac{A_s}{A_c} \ge 0{,}15\%$$

---

### [AB] Verificação de $\beta_x$ a partir das áreas efetivas (seção retangular)
- **Localização:** Formulário 2 — Faixa 5, esquerda.
- **Descrição:** Recálculo de $\beta_x$ após o detalhamento das barras (usando as áreas efetivas $A_{s,ef}$ e $A'_{s,ef}$) para verificar se a linha neutra permanece abaixo de $\beta_{x,lim}$ e confirmar $d, d'$ e os valores de $\beta_s, \beta'_s$.

$$\beta_x = \frac{f_{yd}}{\eta_c \zeta_c b_w d f_{cd}} \left( A_{s,ef}\beta_s - A'_{s,ef}\beta'_s \right)$$

---

### [AC] Taxa geométrica máxima de armadura longitudinal ($\rho_{max}$)
- **Localização:** Formulário 2 — Faixa 5, centro.
- **Descrição:** Verificação de que a soma das áreas efetivas de tração e compressão não ultrapassa o limite máximo normativo de 4% da área da seção transversal de concreto ($A_c$).

$$\rho_{max} = \frac{A_{s,ef} + A'_{s,ef}}{A_c} \le 4\%$$

---

### [AD] Ajuste de armaduras quando $\rho_{min} < 0{,}15\%$
- **Localização:** Formulário 2 — Faixa 5, direita.
- **Descrição:** Regra sequencial de compensação quando a área de tração calculada resulta inferior à taxa mínima ($0{,}15\% A_c$): transfere-se a diferença para $A'_s$, fixa-se $A_s = 0{,}0015 A_c$ e adotam-se $\beta_s = 1{,}0$ e $\beta'_s$ mantido (executando as atribuições na ordem escrita).

$$\text{Se } \rho_{min} < 0{,}15\% : \quad A'_s = A'_s + \left(0{,}0015 A_c - A_s\right) \quad A_s = 0{,}0015 A_c \quad \beta_s = 1{,}0 \quad \beta'_s = \beta'_s \quad \text{(na ordem)}$$

---

### [AE] Centro de gravidade das camadas de armadura ($y_s, y'_s$)
- **Localização:** Formulário 2 — Faixa 6, esquerda.
- **Descrição:** Distância do centro de gravidade da armadura ao centro da 1ª camada (mais próxima da borda) quando há múltiplas camadas ($n$ camadas) na tração ($y_s$) ou na compressão ($y'_s$), ponderada pelas áreas $A_{\phi i}$ de cada camada e pelos espaçamentos acumulados $\sum_{j=1}^{i} y_{\phi j}$.

$$y_s = \frac{\displaystyle\sum_{i=1}^{n} \left[ A_{\phi i} \left( \displaystyle\sum_{j=1}^{i} y_{\phi j} \right) \right]}{A_{s,ef}} \qquad y'_s = \frac{\displaystyle\sum_{i=1}^{n} \left[ A'_{\phi i} \left( \displaystyle\sum_{j=1}^{i} y'_{\phi j} \right) \right]}{A'_{s,ef}}$$

---

### [AF] Espaçamentos livres mínimos entre barras ($a_h, a_v$)
- **Localização:** Formulário 2 — Faixa 6, centro-esquerda.
- **Descrição:** Critérios mínimos para o espaçamento livre horizontal ($a_h$) e vertical ($a_v$) entre faces das barras longitudinais em função do diâmetro da barra ($\phi_\ell$) e da dimensão máxima característica do agregado graúdo ($d_{max}$).

$$a_h \ge \begin{cases} 2\text{ cm} \\ \phi_\ell \\ 1{,}2\, d_{max} \end{cases} \qquad a_v \ge \begin{cases} 2\text{ cm} \\ \phi_\ell \\ 0{,}5\, d_{max} \end{cases}$$

---

### [AG] Áreas efetivas de aço ($A_{s,ef}, A'_{s,ef}$)
- **Localização:** Formulário 2 — Faixa 6, centro-direita.
- **Descrição:** Cálculo das áreas reais adotadas após a escolha do número inteiro de barras ($n_{\phi_\ell}, n'_{\phi'_\ell}$) e dos respectivos diâmetros ($\phi_\ell, \phi'_\ell$).

$$A_{s,ef} = \frac{n_{\phi_\ell} \pi \phi_\ell^2}{4} \qquad A'_{s,ef} = \frac{n'_{\phi'_\ell} \pi \phi_\ell'^2}{4}$$

---

### [AH] Resistências de cálculo ($f_{cd}, f_{yd}$)
- **Localização:** Formulário 2 — Faixa 6, direita.
- **Descrição:** Obtenção das resistências de cálculo do concreto ($f_{cd}$) e do aço ($f_{yd}$) a partir das resistências características e dos coeficientes minoradores $\gamma_c, \gamma_s$ (ver bloco **[AI]**).

$$f_{cd} = \frac{f_{ck}}{\gamma_c} \qquad f_{yd} = \frac{f_{yk}}{\gamma_s}$$

---

### [AI] Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$)
- **Localização:** Formulário 2 — Bloco inferior esquerdo (tabela superior).
- **Descrição:** Valores de $\gamma_c$ e $\gamma_s$ para combinações do ELU (normais, especiais/de construção e excepcionais) e do ELS.

| Estado Limite | Combinações | $\gamma_c$ | $\gamma_s$ |
| :--- | :--- | :---: | :---: |
| **E.L.U.** | Normais | 1,40 | 1,15 |
| **E.L.U.** | Especiais ou de construção | 1,20 | 1,15 |
| **E.L.U.** | Excepcionais | 1,20 | 1,00 |
| **E.L.S.** | — | 1,00 | 1,00 |

---

### [AJ] Alturas úteis ($d, d'$)
- **Localização:** Formulário 2 — Bloco inferior esquerdo, abaixo de **[AI]**.
- **Descrição:** Altura útil tracionada ($d$) e distância da borda comprimida ao centro da armadura comprimida ($d'$), considerando altura total $h$, cobrimento nominal $c_{nom}$, diâmetro do estribo $\phi_t$, diâmetro longitudinal $\phi_\ell$ (ou $\phi'_\ell$) e deslocamento do CG das camadas ($y_s, y'_s$).

$$d = h - c_{nom} - \phi_t - 0{,}5\,\phi_\ell - y_s$$

$$d' = c_{nom} + \phi_t + 0{,}5\,\phi'_\ell + y'_s$$

---

### [AK] Módulo de elasticidade do aço ($E_s$)
- **Localização:** Formulário 2 — Bloco inferior esquerdo, ao lado direito de **[AJ]**.
- **Descrição:** Módulo de elasticidade longitudinal padrão dos aços de armadura passiva utilizado no cálculo de $\beta_s$ e $\beta'_s$.

$$E_s = 21000\text{ }\frac{\text{kN}}{\text{cm}^2}$$

---

### [AL] Deformação última de encurtamento do concreto ($\varepsilon_{cu}$)
- **Localização:** Formulário 2 — Bloco inferior esquerdo, abaixo de **[AJ]** e **[AK]**.
- **Descrição:** Deformação específica de ruptura do concreto comprimido na flexão, para concretos do Grupo I ($f_{ck} \le 50\text{ MPa}$) e do Grupo II ($f_{ck} > 50\text{ MPa}$).

$$\varepsilon_{cu} = 3{,}5\text{‰} \qquad (f_{ck} \le 50\text{ MPa})$$

$$\varepsilon_{cu} = 2{,}6\text{‰} + 35{,}0\text{‰}\left(\frac{90 - f_{ck}}{100}\right)^4 \qquad (f_{ck} > 50\text{ MPa})$$

---

### [AM] Dimensionamento e verificação de Seção T
- **Localização:** Formulário 2 — Bloco inferior direito (ao lado de **[AI]**–**[AL]**).
- **Descrição:** Fluxo completo para seção T com mesa colaborante de largura $b_f$ e espessura $h_f$:
  1. Calcula-se $M_{rdf}$ (momento resistente se toda a mesa estivesse comprimida, $y = h_f$).
  2. Se $M_{rdf} \ge M_{sd}$ ($y \le h_f$), dimensiona-se como **seção retangular equivalente de largura $b_f$** (blocos **[S]**, **[V]**, **[X]** trocando $b_w$ por $b_f$).
  3. Se $M_{rdf} < M_{sd}$ ($y > h_f$), trabalha-se como **viga T verdadeira**: parcela das abas $M_{rda}$ mais parcela da alma $M_{rdw}$ (e eventual armadura comprimida $M'_{rd} = M_{sd} - M_{rda} - M_{rd,lim}$ caso $M_{sd} - M_{rda} > M_{rd,lim}$). A última equação permite verificar $\beta_x$ após o detalhamento (com $A_{s,ef}$ e $A'_{s,ef}$).

$$M_{rdf} = \eta_c h_f b_f \left(d - \frac{h_f}{2}\right) f_{cd} \qquad \begin{cases} M_{rdf} < M_{sd} \therefore \text{viga T} \\ M_{rdf} \ge M_{sd} \therefore \text{retangular equivalente de base } b_f \end{cases}$$

$$M_{rda} = \eta_c h_f (b_f - b_w)\left(d - \frac{h_f}{2}\right) f_{cd}$$

$$M_{sd} = M_{rd} = M_{rdw} + M'_{rd} + M_{rda}$$

$$A_s = \left[\frac{M_{rda}}{\left(d - \dfrac{h_f}{2}\right)} + \frac{M'_{rd}}{(d - d')} + \frac{M_{rdw}}{\beta_z d}\right] \frac{1}{\beta_s f_{yd}}$$

$$\beta_x = \left(\frac{A_s}{\eta_c \zeta_c b_w d}\right)\frac{f_{yd}}{f_{cd}}\beta_s - \left(\frac{A'_s}{\eta_c \zeta_c b_w d}\right)\frac{f_{yd}}{f_{cd}}\beta'_s - \left[\frac{h_f(b_f - b_w)}{\zeta_c b_w d}\right]$$

---

### [AN] Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`)
- **Localização:** Formulário 2 — Faixa inferior de vigas, 1ª coluna (equivalente ao bloco **[I]** do Formulário 1).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com carga distribuída $w$ em todo o vão.

$$M_A = \frac{wx(3L - 4x)}{8} \qquad V_A = \frac{w(3L - 8x)}{8} \qquad R_1 = \frac{3Lw}{8} \qquad R_2 = \frac{5Lw}{8} \qquad M_2 = -\frac{L^2 w}{8}$$

---

### [AO] Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`)
- **Localização:** Formulário 2 — Faixa inferior de vigas, 2ª coluna (equivalente ao bloco **[J]** do Formulário 1).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com carga concentrada $F$ à distância $a$ de $R_1$. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{Fx\left(2L^3 - 3L^2 a + a^3\right)}{2L^3} \qquad M_B = \frac{Fa\left(2L^3 - 3L^2 x + a^2 x\right)}{2L^3}$$

$$V_A = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad V_B = \frac{Fa\left(-3L^2 + a^2\right)}{2L^3}$$

$$R_1 = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad R_2 = \frac{Fa\left(3L^2 - a^2\right)}{2L^3} \qquad M_2 = \frac{Fa\left(-L^2 + a^2\right)}{2L^2}$$

---

### [AP] Viga apoiada-engastada com momento concentrado $M$ (`AE10-m`)
- **Localização:** Formulário 2 — Faixa inferior de vigas, 3ª coluna (equivalente ao bloco **[L]** do Formulário 1).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com momento concentrado $M$ aplicado à distância $a$ de $R_1$. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$. *(Nota: neste formulário de 2024, o sinal de $V_B$ aparece corrigido e igual a $V_A$, pois o momento concentrado não gera salto no diagrama de cortante.)*

$$M_A = \frac{3Mx\left(-L^2 + a^2\right)}{2L^3} \qquad M_B = M - \frac{3Mx}{2L} + \frac{3Ma^2 x}{2L^3}$$

$$V_A = \frac{3M\left(-L^2 + a^2\right)}{2L^3} \qquad V_B = \frac{3M\left(-L^2 + a^2\right)}{2L^3}$$

$$R_1 = \frac{3M\left(-L^2 + a^2\right)}{2L^3} \qquad R_2 = \frac{3M\left(L^2 - a^2\right)}{2L^3} \qquad M_2 = \frac{M\left(-L^2 + 3a^2\right)}{2L^2}$$

---

### [AQ] Viga biapoiada com balanço e carga distribuída total $w$ (`VB1-w`)
- **Localização:** Formulário 2 — Faixa inferior de vigas, 4ª coluna.
- **Descrição:** Viga de comprimento total $L$, com apoio $R_1$ em $x=0$, apoio $R_2$ em $x=a$ e balanço de comprimento $L-a$ à direita ($a \le x \le L$), sob carregamento distribuído uniforme $w$ em todo o comprimento. Trecho $A$: vão entre apoios ($0 \le x \le a$); Trecho $B$: balanço ($a \le x \le L$).

$$M_A = \frac{wx\left(-L^2 + 2La - ax\right)}{2a} \qquad M_B = \frac{w\left(-L^2 + 2Lx - x^2\right)}{2}$$

$$V_A = -\frac{L^2 w}{2a} + Lw - wx \qquad V_B = w(L - x)$$

$$R_1 = \frac{Lw(-L + 2a)}{2a} \qquad R_2 = \frac{L^2 w}{2a}$$

---

## Formulário 3 — Armadura Transversal (`Formulario-ArmaduraTransversal-2022-1.pdf`)

### [AR] Condições de segurança ao cisalhamento ($V_{sd} \le V_{rdc}, V_{sd} \le V_{rdw}$)
- **Localização:** Formulário 3 — Topo esquerdo.
- **Descrição:** Verificações fundamentais do ELU para força cortante: as diagonais comprimidas de concreto ($V_{rdc}$) e os montantes tracionados com contribuição complementar ($V_{rdw}$) devem resistir ao cortante solicitante de cálculo $V_{sd}$.

$$V_{sd} \le V_{rdc} \qquad V_{sd} \le V_{rdw}$$

---

### [AS] Parcela resistente pelos mecanismos complementares ($V_{c,I}, V_{c,II}$)
- **Localização:** Formulário 3 — Topo centro.
- **Descrição:** Contribuição $V_c$ do concreto e engrenamento dos agregados somada à armadura transversal na treliça generalizada. No **Modelo I** ($\theta = 45^\circ$), $V_{c,I}$ é constante; no **Modelo II** ($30^\circ \le \theta \le 45^\circ$), $V_{c,II}$ reduz linearmente conforme $V_{sd}$ se aproxima de $V_{rdc}$ (limitado a $0{,}6 f_{ctd} b_w d$).

$$V_{c,I} = 0{,}6 f_{ctd} b_w d \qquad V_{c,II} = 0{,}6 f_{ctd} b_w d \left(\frac{V_{rdc} - V_{sd}}{V_{rdc} - 0{,}6 f_{ctd} b_w d}\right) \le 0{,}6 f_{ctd} b_w d$$

---

### [AT] Força cortante resistente por tração na diagonal ($V_{rdw}$)
- **Localização:** Formulário 3 — Topo direito.
- **Descrição:** Parcela total resistente à ruína por tração diagonal (escoamento dos estribos + mecanismos complementares), utilizada na verificação $V_{sd} \le V_{rdw}$ ou para isolar $V_{sw} = V_{sd} - V_c$ no dimensionamento.

$$V_{rdw} = V_c + V_{sw}$$

---

### [AU] Força cortante resistente das diagonais comprimidas ($V_{rdc}, V_{rdc,I}, V_{rdc,II}$)
- **Localização:** Formulário 3 — Faixa 2, esquerda.
- **Descrição:** Resistência máxima à compressão das bielas de concreto ($V_{rdc}$) na expressão geral (ângulo da biela $\theta$ e inclinação do estribo $\alpha$) e nos casos práticos com estribos verticais ($\alpha = 90^\circ$): **Modelo I** ($\theta = 45^\circ$) e **Modelo II** ($\theta = 30^\circ$). Inserir $f_{ck}$ em MPa no termo $(1 - f_{ck}/250)$.

$$V_{rdc} = 0{,}536\, b_w d \left[\cotg(\alpha) + \cotg(\theta)\right]\operatorname{sen}^2(\theta)\left(1 - \frac{f_{ck}}{250}\right) f_{cd}$$

$$V_{rdc,I} = 0{,}268\, b_w d \left(1 - \frac{f_{ck}}{250}\right) f_{cd}$$

$$V_{rdc,II} = 0{,}232\, b_w d \left(1 - \frac{f_{ck}}{250}\right) f_{cd}$$

---

### [AV] Força cortante resistente pela armadura transversal ($V_{sw}, V_{sw,I}, V_{sw,II}$)
- **Localização:** Formulário 3 — Faixa 2, direita.
- **Descrição:** Parcela resistida pelos estribos ($V_{sw}$) na expressão geral e nos casos com $\alpha = 90^\circ$ para **Modelo I** ($\theta = 45^\circ$) e **Modelo II** ($\theta = 30^\circ$). No dimensionamento, faz-se $V_{sw} = V_{sd} - V_c$ para isolar a relação necessária $(A_{sw}/s)$.

$$V_{sw} = \left(\frac{A_{sw}}{s}\right) 0{,}9\, d\, f_{ywd}\left[\cotg(\theta) + \cotg(\alpha)\right]\operatorname{sen}(\alpha)$$

$$V_{sw,I} = 0{,}9 \left(\frac{A_{sw}}{s}\right) d\, f_{ywd}$$

$$V_{sw,II} = 1{,}559 \left(\frac{A_{sw}}{s}\right) d\, f_{ywd}$$

---

### [AW] Resistência característica à tração inferior do concreto ($f_{ctk,inf}$)
- **Localização:** Formulário 3 — Faixa 3, esquerda.
- **Descrição:** Valor característico inferior da resistência do concreto à tração direta (em MPa para $f_{ck}$ em MPa), usado na determinação de $f_{ctd}$ e da parcela $V_c$.

$$f_{ctk,inf} = \begin{cases} 0{,}21 \sqrt[3]{f_{ck}^2} & f_{ck} \le 50\text{ MPa} \\ 1{,}484 \ln(1 + 0{,}11 f_{ck}) & f_{ck} > 50\text{ MPa} \end{cases}$$

---

### [AX] Resistência de cálculo à tração direta do concreto ($f_{ctd}$)
- **Localização:** Formulário 3 — Faixa 3, centro-esquerda.
- **Descrição:** Resistência de cálculo do concreto à tração obtida dividindo $f_{ctk,inf}$ pelo coeficiente $\gamma_c$ (bloco **[BC]**).

$$f_{ctd} = \frac{f_{ctk,inf}}{\gamma_c}$$

---

### [AY] Taxa / relação mínima de armadura transversal ($\left(A_{sw}/s\right)_{min}$)
- **Localização:** Formulário 3 — Faixa 3, centro-direita.
- **Descrição:** Relação mínima entre área da seção dos estribos e seu espaçamento longitudinal para estribos verticais ($\alpha = 90^\circ$). Inserir $f_{ck}$ em MPa; a unidade de $(A_{sw}/s)_{min}$ acompanha a unidade de comprimento adotada para $b_w$ (ex.: para $b_w$ em cm, resulta em $\text{cm}^2/\text{cm}$).

$$\left(\frac{A_{sw}}{s}\right)_{min} \ge 0{,}06\, b_w \frac{\sqrt[3]{f_{ck}^2}}{435}$$

---

### [AZ] Limites de diâmetro dos estribos ($\phi_t$)
- **Localização:** Formulário 3 — Faixa 3, direita.
- **Descrição:** Limites normativos mínimo e máximo para a bitola dos estribos em função da largura da alma $b_w$.

$$5\text{ mm} \le \phi_t \le \frac{b_w}{10}$$

---

### [BA] Espaçamentos mínimo e máximo entre estribos ($s$)
- **Localização:** Formulário 3 — Faixa 4 (largura total).
- **Descrição:** Limites de espaçamento longitudinal entre estribos conforme a razão $V_{sd}/V_{rdc}$. *(Obs. das notas de aula: se $d \le 35\text{ cm}$ e $0{,}3d < 10\text{ cm}$, o mínimo de $10\text{ cm}$ é dispensado, respeitando $s \le 0{,}3d$.)*

$$\frac{V_{sd}}{V_{rdc}} \le 0{,}67 \implies 10\text{ cm} \le s \le \min\begin{cases} 0{,}6 d \\ 30\text{ cm} \end{cases}$$

$$\frac{V_{sd}}{V_{rdc}} > 0{,}67 \implies 10\text{ cm} \le s \le \min\begin{cases} 0{,}3 d \\ 30\text{ cm} \end{cases}$$

---

### [BB] Reduções de $V_{sd}$ junto aos apoios ($d/2$ e $a \le 2d$)
- **Localização:** Formulário 3 — Meio esquerdo (dois esquemas gráficos de apoio e diagrama $V_{sd}$).
- **Descrição:** Regras gráficas para redução do esforço cortante solicitante $V_{sd}$ próximo aos apoios no dimensionamento dos estribos ($A_{sw}$ — lembrando que para a verificação da biela comprimida $V_{rdc}$ usa-se o cortante na face do apoio):
  - **Esquema esquerdo (carga distribuída):** o diagrama de $V_{sd}$ para cálculo da armadura transversal pode ser considerado constante entre a face do apoio e a seção distante $d/2$ da face do apoio, igual ao valor em $d/2$.
  - **Esquema direito (carga concentrada a distância $a \le 2d$ da face do apoio):** no trecho entre a carga e a face do apoio, reduz-se a parcela do cortante proveniente dessa carga multiplicando-a por $\dfrac{a}{2d}$, isto é, $V_{sd}\dfrac{a}{2d}$.

---

### [BC] Coeficientes de ponderação das resistências ($\gamma_c, \gamma_s$)
- **Localização:** Formulário 3 — Meio direito (tabela superior).
- **Descrição:** Valores de $\gamma_c$ e $\gamma_s$ para combinações do ELU e do ELS.

| Estado Limite | Combinações | $\gamma_c$ | $\gamma_s$ |
| :--- | :--- | :---: | :---: |
| **E.L.U.** | Normais | 1,40 | 1,15 |
| **E.L.U.** | Especiais ou de construção | 1,20 | 1,15 |
| **E.L.U.** | Excepcionais | 1,20 | 1,00 |
| **E.L.S.** | — | 1,00 | 1,00 |

---

### [BD] Resistências de cálculo ($f_{cd}, f_{yd}$)
- **Localização:** Formulário 3 — Meio direito, abaixo de **[BC]** à esquerda.
- **Descrição:** Resistências de cálculo do concreto ($f_{cd}$) e do aço longitudinal ($f_{yd}$) obtidas com os coeficientes do bloco **[BC]**.

$$f_{cd} = \frac{f_{ck}}{\gamma_c} \qquad f_{yd} = \frac{f_{yk}}{\gamma_s}$$

---

### [BE] Área efetiva de um estribo ($A_{sw,ef}$)
- **Localização:** Formulário 3 — Meio direito, abaixo de **[BC]** à direita.
- **Descrição:** Área total da seção transversal de um estribo considerando o número de ramos ($n_r$, normalmente $2$ ou $4$) e o diâmetro adotado ($\phi_t$).

$$A_{sw,ef} = n_r\, 0{,}25\,\pi\,\phi_t^2$$

---

### [BF] Verificação da relação efetiva de armadura transversal
- **Localização:** Formulário 3 — Meio direito, bloco inferior esquerdo.
- **Descrição:** Condição final de verificação após a escolha de $\phi_t$, $n_r$ e $s_{ef}$: a relação efetiva adotada deve ser maior ou igual à relação necessária (ou mínima).

$$\left(\frac{A_{sw,ef}}{s_{ef}}\right) \ge \left(\frac{A_{sw}}{s}\right)$$

---

### [BG] Tensão limite de cálculo na armadura transversal ($f_{ywd}$)
- **Localização:** Formulário 3 — Meio direito, bloco inferior direito.
- **Descrição:** Tensão máxima de cálculo admitida para os estribos pela NBR 6118 (correspondente ao $f_{yd}$ do aço CA-50: $500 / 1{,}15 \approx 435\text{ MPa}$; vale para CA-50 e CA-60 na combinação normal).

$$f_{ywd} = 435\text{ MPa}$$

---

### [BH] Cortante solicitante mínimo para armadura mínima ($V_{sd,min,I}, V_{sd,min,II}$)
- **Localização:** Formulário 3 — Abaixo dos esquemas, bloco esquerdo.
- **Descrição:** Valor de esforço cortante solicitante correspondente exatamente à armadura transversal mínima $(A_{sw}/s)_{min}$ (para Modelo I ou Modelo II). Nos trechos da viga onde $V_{sd} \le V_{sd,min}$, basta adotar a armadura transversal mínima.

$$V_{sd,min,I} = 0{,}9 \left(\frac{A_{sw}}{s}\right)_{min} d\, f_{ywd} + 0{,}6 f_{ctd} b_w d$$

$$V_{sd,min,II} = 1{,}559 \left(\frac{A_{sw}}{s}\right)_{min} d\, f_{ywd} + 0{,}6 f_{ctd} b_w d \left[1 - 1{,}559 \left(\frac{A_{sw}}{s}\right)_{min} \frac{d\, f_{ywd}}{V_{rdc}}\right]$$

---

### [BI] Espaçamento efetivo máximo dos estribos ($s_{ef,I}, s_{ef,II}$)
- **Localização:** Formulário 3 — Abaixo de **[BF]**/**[BG]**, bloco direito.
- **Descrição:** Espaçamento inteiro máximo (função piso $\lfloor \cdot \rfloor$, arredondando para baixo) permitido entre estribos de área efetiva $A_{sw,ef}$ para equilibrar $V_{sw}$ no Modelo I ou Modelo II (deve também atender aos limites do bloco **[BA]**).

$$s_{ef,I} \le \left\lfloor \frac{0{,}9\, A_{sw,ef}\, d\, f_{ywd}}{V_{sw,I}} \right\rfloor \qquad s_{ef,II} \le \left\lfloor \frac{1{,}559\, A_{sw,ef}\, d\, f_{ywd}}{V_{sw,II}} \right\rfloor$$

---

### [BJ] Viga apoiada-engastada com dois momentos concentrados $M$ (`AE11-mo`)
- **Localização:** Formulário 3 — Faixa intermediária (largura total, acima das 4 vigas).
- **Descrição:** Viga de vão total $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), submetida a dois momentos concentrados iguais $M$ (sentido anti-horário no esquema): um à distância $a$ do apoio esquerdo $R_1$ e outro à distância $b$ do engaste direito $R_2$. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L - b$; Trecho $C$: $L - b \le x \le L$. *(Equivalente a `AE11-mo` em `BeamsDiagrams`.)*

$$M_A = \frac{3Mx\left(-L^2 - 2Lb + a^2 + b^2\right)}{2L^3} \qquad M_B = \frac{M\left(2L^3 - 3L^2 x - 6Lbx + 3x(a^2 + b^2)\right)}{2L^3}$$

$$M_C = \frac{M\left(4L^3 - 3L^2 x - 6Lbx + 3x(a^2 + b^2)\right)}{2L^3}$$

$$V_A = \frac{3M\left(-L^2 - 2Lb + a^2 + b^2\right)}{2L^3} \qquad V_B = \frac{3M\left(-L^2 - 2Lb + a^2 + b^2\right)}{2L^3} \qquad V_C = \frac{3M\left(-L^2 - 2Lb + a^2 + b^2\right)}{2L^3}$$

$$R_1 = \frac{3M\left(-L^2 - 2Lb + a^2 + b^2\right)}{2L^3} \qquad R_2 = \frac{3M\left(L^2 + 2Lb - a^2 - b^2\right)}{2L^3} \qquad M_2 = \frac{M\left(L^2 - 6Lb + 3a^2 + 3b^2\right)}{2L^2}$$

---

### [BK] Viga apoiada-engastada com carga distribuída total $w$ (`AE1-w`)
- **Localização:** Formulário 3 — Faixa inferior de vigas, 1ª coluna (equivalente aos blocos **[I]** e **[AN]**).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com carga distribuída $w$ em todo o vão.

$$M_A = \frac{wx(3L - 4x)}{8} \qquad V_A = \frac{w(3L - 8x)}{8} \qquad R_1 = \frac{3Lw}{8} \qquad R_2 = \frac{5Lw}{8} \qquad M_2 = -\frac{L^2 w}{8}$$

---

### [BL] Viga apoiada-engastada com carga concentrada $F$ (`AE8-fa`)
- **Localização:** Formulário 3 — Faixa inferior de vigas, 2ª coluna (equivalente aos blocos **[J]** e **[AO]**).
- **Descrição:** Viga de vão $L$, apoio simples à esquerda ($R_1$) e engaste à direita ($R_2, M_2$), com carga concentrada $F$ à distância $a$ de $R_1$. Trecho $A$: $0 \le x \le a$; Trecho $B$: $a \le x \le L$.

$$M_A = \frac{Fx\left(2L^3 - 3L^2 a + a^3\right)}{2L^3} \qquad M_B = \frac{Fa\left(2L^3 - 3L^2 x + a^2 x\right)}{2L^3}$$

$$V_A = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad V_B = \frac{Fa\left(-3L^2 + a^2\right)}{2L^3}$$

$$R_1 = F - \frac{3Fa}{2L} + \frac{Fa^3}{2L^3} \qquad R_2 = \frac{Fa\left(3L^2 - a^2\right)}{2L^3} \qquad M_2 = \frac{Fa\left(-L^2 + a^2\right)}{2L^2}$$

---

### [BM] Viga biengastada com carga distribuída total $w$ (`BE1-w`)
- **Localização:** Formulário 3 — Faixa inferior de vigas, 3ª coluna.
- **Descrição:** Viga de vão $L$ com engastes nas duas extremidades ($R_1, M_1$ à esquerda e $R_2, M_2$ à direita), submetida a carregamento distribuído uniforme $w$ em todo o vão ($0 \le x \le L$). Trecho único $A$. *(Atenção aos sinais indicados nas setas de momento do esquema: $M_1 = +\frac{L^2 w}{12}$ no sentido anti-horário à esquerda e $M_2 = -\frac{L^2 w}{12}$ no sentido horário à direita; na equação de $M_A$, ambos os apoios têm momento fletor negativo $-L^2 w / 12$.)*

$$M_A = \frac{w\left(-L^2 + 6Lx - 6x^2\right)}{12} \qquad V_A = \frac{w(L - 2x)}{2}$$

$$R_1 = \frac{Lw}{2} \qquad M_1 = \frac{L^2 w}{12} \qquad R_2 = \frac{Lw}{2} \qquad M_2 = -\frac{L^2 w}{12}$$

---

### [BN] Viga biapoiada com balanço e carga distribuída total $w$ (`VB1-w`)
- **Localização:** Formulário 3 — Faixa inferior de vigas, 4ª coluna (equivalente ao bloco **[AQ]**).
- **Descrição:** Viga de comprimento total $L$, com apoio $R_1$ em $x=0$, apoio $R_2$ em $x=a$ e balanço de comprimento $L-a$ à direita ($a \le x \le L$), sob carregamento distribuído uniforme $w$ em todo o comprimento. Trecho $A$: vão entre apoios ($0 \le x \le a$); Trecho $B$: balanço ($a \le x \le L$).

$$M_A = \frac{wx\left(-L^2 + 2La - ax\right)}{2a} \qquad M_B = \frac{w\left(-L^2 + 2Lx - x^2\right)}{2}$$

$$V_A = -\frac{L^2 w}{2a} + Lw - wx \qquad V_B = w(L - x)$$

$$R_1 = \frac{Lw(-L + 2a)}{2a} \qquad R_2 = \frac{L^2 w}{2a}$$
