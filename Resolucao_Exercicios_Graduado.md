# Resolução Passo a Passo — Exercícios de Nível Graduado (Concreto I)

Guia de estudo com resolução detalhada para os **5 temas** pedidos, utilizando os exercícios da seção **Propostos — Nível Graduado** do [CadernodeExercícios-EstruturasConcreto-2021.pdf](file:///c:/Users/vhlim/01.%20Projetos/concreto%20I%20-%20aproveitamento/CadernodeExercícios-EstruturasConcreto-2021.pdf) e referenciando todas as equações pelos códigos do [Formularios_Mapeados.md](file:///c:/Users/vhlim/01.%20Projetos/concreto%20I%20-%20aproveitamento/Formularios_Mapeados.md) (`[A]` a `[BN]`) e do auxiliar [BeamsDiagrams_Referencia.md](file:///c:/Users/vhlim/01.%20Projetos/concreto%20I%20-%20aproveitamento/00.%20BeamsDiagrams/BeamsDiagrams_Referencia.md).

---

## Sumário dos Exercícios Resolvidos

0. **RAIO-X GERAL DA PROVA:** O que diferencia os exercícios de **Nível Graduado** dos níveis Iniciante e Intermediário?
1. **COMBINAÇÕES:** Exercício `1.4.1 — Viga de ponte` *(Nível Graduado, p. 30)*
2. **ARMADURA RETANGULAR SIMPLES:** Exercício `3.4.1 — Planta de escola` *(Nível Graduado, p. 74)* + Caso completo com balanços `3.3.15` *(p. 73)*
3. **ARMADURA RETANGULAR DUPLA:** Exercício `4.3.9 — Menor altura múltipla de 5` *(p. 90–91, com nota sobre a repetição tipográfica de `4.4.1` na p. 91)*
4. **ARMADURA T SIMPLES:** Exercício `5.4.3 — Largura colaborante e máximo carregamento` *(Nível Graduado, p. 107–108)*
5. **ARMADURA T DUPLA:** Exercício `6.4.1 — Máxima carga móvel possível em viga T` *(Nível Graduado, p. 122–123)* + Roteiro de dimensionamento quando $M_{sd} > M_{rda} + M_{rd,lim}$
6. **ARMADURA TRANSVERSAL (MODELOS I E II):** Exercício `7.4.1 — Menor valor possível de θ` *(Modelo II, p. 165–166)* e Exercício `7.4.2 — Viga de transição` *(Modelo I, p. 166–167)*
7. **EXERCÍCIO COMPLETO INTEGRADO:** Projeto de viga de depósito *(Combinações + Armadura Longitudinal + Armadura Transversal, baseado no Ex. `1.3.3`, p. 28)*

---

## 0. Raio-X Geral da Prova — O Que Torna um Exercício de Nível Graduado?

Não: os exercícios de **Nível Graduado** da apostila/caderno do Prof. Argenta **não são apenas mais longos**. Enquanto o *Nível Iniciante* entrega o esforço pronto ($M_k$ ou $V_{sd}$) para aplicação direta de fórmula e o *Nível Intermediário* dá uma viga isolada com caminho direto ($q_k \to M_{sd} \to A_s$), o **Nível Graduado** testa **cinco mecanismos específicos de raciocínio** (geralmente combinando 2 ou 3 deles na mesma questão):

1. **Engenharia Reversa / Caminho Inverso com Condição-Limite Oculta:**
   - Em vez de dar o carregamento e pedir a armadura ($q_k \to M_{sd} \to A_s$), o exercício **trava um parâmetro interno de deformação ou capacidade** e pede a geometria ou a carga máxima:
     - Ex. `4.3.9`: trava $\beta_x = \beta_{x,lim}$ nas seções B e C para achar a menor altura $h$ múltipla de $5\text{ cm}$.
     - Ex. `5.4.3`: trava a profundidade da linha neutra em $x = 1{,}25\,h_f$ para descobrir o momento resistente e, de trás para frente, achar $q_k$.
     - Ex. `6.4.1`: dá as barras prontas ($3\phi 20$, $4\phi 16 + 2\phi 10$) e pede a maior carga móvel $Q_k$.
     - Ex. `7.4.1`: pede o menor ângulo $\theta$ (múltiplo de $5^\circ$) no limite do esmagamento da biela ($V_{sd} = V_{rdc}(\theta)$).
     - Ex. `7.4.2`: parametriza a carga por pavimento ($P_d = 400\,n$) e pede o número máximo de pavimentos $n_{\max}$ a partir de $V_{rdc,I}$.
2. **Extração de Dados a partir da Planta de Formas (e não da viga isolada):**
   - Nos exercícios `3.4.1` e `5.4.3`, você recebe a **planta baixa de formas**. Precisa saber converter **vão livre em vão teórico entre eixos** ($\ell = \ell_{\text{livre}} + b_{\text{pilar}}/2 + b_{\text{pilar}}/2$), somar o quinhão de **duas lajes adjacentes** sobre vigas internas e calcular a **largura colaborante $b_f$** respeitando a simetria pelo painel mais estreito ($0{,}5\,b_{li,\min}$).
3. **Acoplamento entre Duas Seções ou Inversão de Sinal na Mesma Viga:**
   - A resposta de uma seção governa outra: em `4.3.9`, a altura $h=55\text{ cm}$ definida pela seção B (armadura simples) obriga o meio do vão (onde o momento é maior) a trabalhar com **armadura dupla em 2 camadas**.
   - Em `6.4.1`, a viga T tem **dupla personalidade**: no meio do vão ($M^+$) comprime a mesa larga ($b_f = 60\text{ cm}$), mas nos apoios com balanço ($M^-$) a mesa fica tracionada (inútil!) e quem comprime é a **alma estreita ($b_w = 25\text{ cm}$) com armadura dupla**.
4. **Casos Especiais de Mecânica do Concreto (Não-escoamento $\beta'_s < 1{,}0$ e Detalhamento Real em Camadas):**
   - Nos níveis básicos, quase sempre $\beta_s = \beta'_s = 1{,}0$ e a armadura cabe em 1 camada. No nível graduado:
     - Quando há **2 camadas de barras** (`4.3.9` e `Tema 7`), o centro de gravidade sobe ($y_s = 2{,}0\text{ cm}$), **reduzindo a altura útil real $d$** (`[AE]`, `[AJ]`) e diminuindo $M_{rd,lim}$!
     - Quando uma seção tem armadura dupla mas baixa taxa de tração (`6.4.1` nos apoios), a linha neutra fica muito alta ($\beta_x = 0{,}0920 < 0{,}259$), a armadura comprimida $A'_s$ **não escoa ($\beta'_s = 0{,}5416 < 1{,}0$)** e exige resolver uma equação de 2º grau para $\beta_x$ (`[AB]` + `[S]`).
5. **Pegadinhas Normativas de Estática e de Redução de Esforço Cortante (`[BB]`):**
   - **Efeito Gangorra / Alívio de Apoio (`1.4.1`):** Uma carga variável em balanço alivia o apoio oposto ($R_{C,Q1} = -0{,}1\,q_{1d}$). Logo, a reação máxima ocorre **com apenas um veículo** na ponte (e não com os dois!), e a reação mínima exige $\gamma_g = 1{,}00$ (favorável) + veículo apenas no apoio oposto.
   - **Quando reduzir e quando NÃO reduzir o cortante (`7.4.1` e `7.4.2`):**
     - Em `7.4.1`, **não existe redução a $d/2$** porque não há carga distribuída nos primeiros $2{,}0\text{ m}$ junto ao apoio ($w=0 \implies V_{sd}$ constante!).
     - Em `7.4.2`, a carga concentrada está a $a \le 2d$ do apoio: na verificação do esmagamento da biela ($V_{sd} \le V_{rdc,I}$, item a) **jamais se reduz o cortante**, mas no cálculo dos estribos ($A_{sw}/s$, item b) **deve-se multiplicar $V_{sd}$ pelo fator redutor $a/(2d)$** (`[BB]`).

---

## 1. COMBINAÇÕES — Exercício `1.4.1 Viga de ponte` (p. 30)

### 1.1 Enunciado e Interpretação do Diagrama Estrutural

A seção transversal da ponte apoia-se em duas vigas longitudinais principais: **V01** (apoio **B**) e **V02** (apoio **C**), funcionando como uma viga contínua com dois balanços nas extremidades **A** e **D**:

```text
          Veículo 1 (Q1)                 Veículo 2 (Q2)
        75 kN         75 kN           75 kN         75 kN
          |             |               |             |
          v             v   gk=40 kN/m  v             v
  ↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
  A=======*=============B=======*=======*=======C=============*=======D
  |<-1,3m-><---1,4m---->|<-1,0m-><-2,0m-><-1,0m->|<---1,4m----><-1,3m->|
  |<------ 2,7 m ------>|<------- 4,0 m ------->|<------ 2,7 m ------>|
                        ^                       ^
                       R_B (V01)               R_C (V02)
```

- **Coordenadas a partir da extremidade esquerda $A$ ($x = 0$):**
  - Extremidade livre esquerda $A$: $x = 0\text{ m}$
  - 1ª roda do Veículo 1 ($Q_{1k} = 75\text{ kN}$): $x = 1{,}3\text{ m}$ ($1{,}4\text{ m}$ à esquerda do apoio $B$)
  - Apoio $B$ (`V01`): $x = 2{,}7\text{ m}$
  - 2ª roda do Veículo 1 ($Q_{1k} = 75\text{ kN}$): $x = 3{,}7\text{ m}$ ($1{,}0\text{ m}$ à direita do apoio $B$)
  - Meio do vão central: $x = 4{,}7\text{ m}$
  - 1ª roda do Veículo 2 ($Q_{2k} = 75\text{ kN}$): $x = 5{,}7\text{ m}$ ($1{,}0\text{ m}$ à esquerda do apoio $C$)
  - Apoio $C$ (`V02`): $x = 6{,}7\text{ m}$
  - 2ª roda do Veículo 2 ($Q_{2k} = 75\text{ kN}$): $x = 8{,}1\text{ m}$ ($1{,}4\text{ m}$ à direita do apoio $C$)
  - Extremidade livre direita $D$: $x = 9{,}4\text{ m}$

---

### 1.2 Coeficientes de Ponderação e Fatores de Combinação (Blocos `[A]`, `[C]`, `[E]`, `[F]`)

1. **Equação da Combinação Última Normal — Bloco `[A]`:**
   $$F_{d,nor} := \left(\biguplus \gamma_g F_{gk}\right) \uplus \left(\biguplus \gamma_{\varepsilon g} F_{\varepsilon gk}\right) \uplus \gamma_q F_{q1k} \uplus \left(\biguplus \gamma_q \psi_{0j} F_{qjk}\right) \uplus \left(\biguplus \gamma_{\varepsilon q} \psi_{0\varepsilon} F_{\varepsilon qk}\right)$$
   Como não há ações indiretas ($\varepsilon g, \varepsilon q$):
   $$F_{d,nor} := \gamma_g G_k \uplus \gamma_q Q_{1k} \uplus \gamma_q \psi_0 Q_{2k}$$

2. **Coeficientes $\gamma_g$ para peso próprio — Bloco `[C]`:**
   - Estrutura de concreto armado moldada no local:
     - Sentido **desfavorável**: $\gamma_g = 1{,}35 \implies g_{d,\text{desf}} = 1{,}35 \times 40 = 54{,}0\text{ kN/m}$
     - Sentido **favorável**: $\gamma_g = 1{,}00 \implies g_{d,\text{fav}} = 1{,}00 \times 40 = 40{,}0\text{ kN/m}$

3. **Coeficientes $\gamma_q$ para as cargas móveis dos veículos — Bloco `[E]`:**
   - Demais ações variáveis / uso:
     - Sentido **desfavorável** (veículo presente): $\gamma_q = 1{,}50 \implies Q_d = 1{,}50 \times 75 = 112{,}50\text{ kN}$ por roda.
     - Sentido **favorável** (veículo ausente): $\gamma_q = 0{,}00 \implies Q_d = 0\text{ kN}$.

4. **Fator de redução $\psi_0$ para Pontes Rodoviárias — Bloco `[F]`:**
   - Em **Passarelas e pontes $\to$ Pontes rodoviárias**: $\psi_0 = 0{,}7$.
   - Caso os dois veículos sejam tratados como duas ações variáveis independentes ($Q_1$ principal e $Q_2$ secundária ou vice-versa), a carga por roda do veículo secundário vale:
     $$\gamma_q \psi_0 Q_k = 1{,}50 \times 0{,}7 \times 75 = 78{,}75\text{ kN}$$
   - Caso ambos os veículos sejam tratados como um único carregamento variável de tráfego ($\psi_0 = 1{,}0$), ambos entram com $112{,}50\text{ kN}$ por roda. Apresentamos abaixo os resultados para **ambas** as hipóteses (e veremos que as reações e momentos extremos nos apoios ocorrem justamente quando há **apenas um** veículo na ponte!).

---

### 1.3 Decomposição por Carregamentos Elementares (Superposição)

Pelo método da desconstrução da viga (união disjunta $\biguplus$), calculamos o efeito estático de cada ação isoladamente:

1. **Ação Permanente $g_d$ (uniforme nos $9{,}4\text{ m}$):**
   - Pela simetria da viga:
     $$R_{B,g} = R_{C,g} = \frac{9{,}4\, g_d}{2} = 4{,}7\, g_d$$

2. **Veículo 1 ($q_{1d}$ em $x = 1{,}3\text{ m}$ e $x = 3{,}7\text{ m}$):**
   - Somatório de momentos em torno do apoio $B$ ($x = 2{,}7\text{ m}$, vão $BC = 4{,}0\text{ m}$):
     $$\sum M_B = 0 \implies -q_{1d}(1{,}4) + q_{1d}(1{,}0) - R_{C,Q1}(4{,}0) = 0 \implies R_{C,Q1} = -\frac{0{,}4}{4{,}0}\,q_{1d} = -0{,}1\, q_{1d}$$
   - Equilíbrio vertical ($\sum F_y = 0$):
     $$R_{B,Q1} = 2\,q_{1d} - R_{C,Q1} = 2{,}1\, q_{1d}$$
   - **Interpretação física importante:** Como o centro de gravidade das duas rodas do Veículo 1 está em $x = 2{,}5\text{ m}$ ($0{,}2\text{ m}$ à esquerda do apoio $B$), o Veículo 1 faz efeito de alavanca sobre $B$, **sobrecarregando $B$ ($+2{,}1\,q_{1d}$)** e **aliviando $C$ ($-0{,}1\,q_{1d}$)**!

3. **Veículo 2 ($q_{2d}$ em $x = 5{,}7\text{ m}$ e $x = 8{,}1\text{ m}$):**
   - Por simetria:
     $$R_{B,Q2} = -0{,}1\, q_{2d} \qquad R_{C,Q2} = +2{,}1\, q_{2d}$$

Portanto, para qualquer combinação $(g_d, q_{1d}, q_{2d})$:
$$R_B = 4{,}7\, g_d + 2{,}1\, q_{1d} - 0{,}1\, q_{2d}$$
$$R_C = 4{,}7\, g_d - 0{,}1\, q_{1d} + 2{,}1\, q_{2d}$$

---

### 1.4 Quadro Completo das Combinações (Reações, Cortantes e Momentos)

| Comb. | Descrição ($\gamma_g, Q_1, Q_2$) | $g_d$ (kN/m) | $q_{1d}$ (kN) | $q_{2d}$ (kN) | $R_B$ (kN) | $R_C$ (kN) | $M_B$ (kN$\cdot$m) | $M_{3{,}7}$ (kN$\cdot$m) | $M_{4{,}7}$ (kN$\cdot$m) | $M_C$ (kN$\cdot$m) |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **ELU 1** | $1{,}35G_k \uplus 1{,}5Q_{1k} \uplus 1{,}05Q_{2k}$ | 54,0 | 112,50 | 78,75 | 482,18 | 407,92 | **-354,33** | -157,46 | -127,08 | -307,08 |
| **ELU 2** | $1{,}35G_k \uplus 1{,}05Q_{1k} \uplus 1{,}5Q_{2k}$ | 54,0 | 78,75 | 112,50 | 407,92 | 482,18 | -307,08 | -150,71 | -127,08 | **-354,33** |
| **ELU 3** | $1{,}35G_k \uplus 1{,}5Q_{1k} \uplus 1{,}5Q_{2k}$ *(s/ $\psi_0$)* | 54,0 | 112,50 | 112,50 | 478,80 | 478,80 | **-354,33** | **-160,83** | **-133,83** | **-354,33** |
| **ELU 4** | $1{,}35G_k \uplus 1{,}5Q_{1k} \uplus 0$ *(só Veíc. 1)* | 54,0 | 112,50 | 0,00 | **490,05** | 242,55 | **-354,33** | -149,58 | -111,33 | -196,83 |
| **ELU 5** | $1{,}35G_k \uplus 0 \uplus 1{,}5Q_{2k}$ *(só Veíc. 2)* | 54,0 | 0,00 | 112,50 | 242,55 | **490,05** | -196,83 | -127,08 | -111,33 | **-354,33** |
| **ELU 6** | $1{,}00G_k \uplus 1{,}5Q_{1k} \uplus 0$ *(fav. + Veíc. 1)* | 40,0 | 112,50 | 0,00 | 424,25 | **176,75** | -303,30 | -119,55 | -88,30 | -145,80 |
| **ELU 7** | $1{,}00G_k \uplus 0 \uplus 1{,}5Q_{2k}$ *(fav. + Veíc. 2)* | 40,0 | 0,00 | 112,50 | **176,75** | 424,25 | -145,80 | -97,05 | -88,30 | -303,30 |
| **ELU 8** | $1{,}00G_k \uplus 0 \uplus 0$ *(só perm. fav.)* | 40,0 | 0,00 | 0,00 | 188,00 | 188,00 | **-145,80** | **-85,80** | **-65,80** | **-145,80** |
| **ELU 9** | $1{,}35G_k \uplus 0 \uplus 0$ *(só perm. desf.)* | 54,0 | 0,00 | 0,00 | 253,80 | 253,80 | -196,83 | -115,83 | -88,83 | -196,83 |

---

### 1.5 Reações de Apoio Máxima e Mínima em B (`V01`) e C (`V02`)

- **Reação Máxima de Cálculo ($R_{B,\max}$ e $R_{C,\max}$):**
  - Ocorre na **ELU 4** para $B$ (e **ELU 5** para $C$), com carga permanente majorada ($\gamma_g = 1{,}35$) e **apenas o veículo sobre aquele apoio** ($q_{1d} = 112{,}50\text{ kN}, q_{2d} = 0$):
    $$R_{B,\max} = R_{C,\max} = 4{,}7 \times 54{,}0 + 2{,}1 \times 112{,}50 - 0{,}1 \times 0 = \mathbf{490{,}05\text{ kN}}$$
- **Reação Mínima de Cálculo ($R_{B,\min}$ e $R_{C,\min}$):**
  - Ocorre na **ELU 7** para $B$ (e **ELU 6** para $C$), com carga permanente favorável ($\gamma_g = 1{,}00$), ausência do veículo sobre o apoio analisado e **presença do veículo sobre o apoio oposto** (provocando alívio de $-11{,}25\text{ kN}$):
    $$R_{B,\min} = R_{C,\min} = 4{,}7 \times 40{,}0 + 2{,}1 \times 0 - 0{,}1 \times 112{,}50 = \mathbf{176{,}75\text{ kN}}$$

---

### 1.6 Envoltória de Esforços Cortantes ($V_{sd}$) e de Momentos Fletores ($M_{sd}$)

#### Equações por trecho:
- **Balanço esquerdo ($0 \le x < 2{,}7\text{ m}$):**
  - Para $0 \le x < 1{,}3\text{ m}$: $V(x) = -g_d x$, $M(x) = -\frac{1}{2} g_d x^2$
  - Para $1{,}3 < x < 2{,}7\text{ m}$: $V(x) = -g_d x - q_{1d}$, $M(x) = -\frac{1}{2} g_d x^2 - q_{1d}(x - 1{,}3)$
- **Vão central ($2{,}7 < x < 6{,}7\text{ m}$):**
  - Para $2{,}7 < x < 3{,}7\text{ m}$: $V(x) = -g_d x - q_{1d} + R_B$, $M(x) = -\frac{1}{2}g_d x^2 - q_{1d}(x - 1{,}3) + R_B(x - 2{,}7)$
  - Para $3{,}7 < x < 5{,}7\text{ m}$: $V(x) = -g_d x - 2q_{1d} + R_B$, $M(x) = -\frac{1}{2}g_d x^2 - q_{1d}(x - 1{,}3) - q_{1d}(x - 3{,}7) + R_B(x - 2{,}7)$

#### Valores Extremos da Envoltória de Cortante ($V_{sd}$):
| Seção $x$ (m) | $V_{sd,\min}$ (kN) | $V_{sd,\max}$ (kN) | Observação |
| :---: | :---: | :---: | :--- |
| $0{,}0$ (A) | $0{,}00$ | $0{,}00$ | Extremidade livre |
| $1{,}3^-$ | $-70{,}20$ | $-52{,}00$ | Antes da 1ª roda de $Q_1$ |
| $1{,}3^+$ | $-182{,}70$ | $-52{,}00$ | Após a 1ª roda de $Q_1$ |
| $2{,}7^-$ ($B_{\text{esq}}$) | **$-258{,}30$** | $-108{,}00$ | Face esquerda do apoio $B$ (máx. cortante negativo) |
| $2{,}7^+$ ($B_{\text{dir}}$) | $+68{,}75$ | **$+231{,}75$** | Face direita do apoio $B$ (máx. cortante positivo — ELU 4) |
| $3{,}7^-$ | $+28{,}75$ | $+177{,}75$ | Antes da 2ª roda de $Q_1$ |
| $3{,}7^+$ | $+28{,}75$ | $+65{,}25$ | Após a 2ª roda de $Q_1$ |
| $4{,}7$ (meio) | $-11{,}25$ | $+11{,}25$ | Assimetria máxima (ELU 4 / ELU 5) |
| $5{,}7^-$ | $-65{,}25$ | $-28{,}75$ | Antes da 1ª roda de $Q_2$ |
| $5{,}7^+$ | $-177{,}75$ | $-28{,}75$ | Após a 1ª roda de $Q_2$ |
| $6{,}7^-$ ($C_{\text{esq}}$) | **$-231{,}75$** | $-68{,}75$ | Face esquerda do apoio $C$ |
| $6{,}7^+$ ($C_{\text{dir}}$) | $+108{,}00$ | **$+258{,}30$** | Face direita do apoio $C$ |

#### Valores Extremos da Envoltória de Momento Fletor ($M_{sd}$):
- Em $x = 0\text{ m}$ ($A$) e $x = 9{,}4\text{ m}$ ($D$): $M_{sd} = 0\text{ kN}\cdot\text{m}$
- Em $x = 1{,}3\text{ m}$ e $x = 8{,}1\text{ m}$: $M_{sd} \in [-45{,}63;\, -33{,}80]\text{ kN}\cdot\text{m}$
- **Nos apoios $B$ ($x = 2{,}7\text{ m}$) e $C$ ($x = 6{,}7\text{ m}$):**
  $$M_{sd,\min} = -\frac{1}{2}(54{,}0)(2{,}7)^2 - 112{,}50(1{,}4) = -196{,}83 - 157{,}50 = \mathbf{-354{,}33\text{ kN}\cdot\text{m}}$$
  $$M_{sd,\max} = -\frac{1}{2}(40{,}0)(2{,}7)^2 = \mathbf{-145{,}80\text{ kN}\cdot\text{m}}$$
- Em $x = 3{,}7\text{ m}$ e $x = 5{,}7\text{ m}$:
  - $M_{sd,\min} = -157{,}46\text{ kN}\cdot\text{m}$ (com $\psi_0 = 0{,}7$) ou $-160{,}83\text{ kN}\cdot\text{m}$ (sem $\psi_0$)
  - $M_{sd,\max} = -85{,}80\text{ kN}\cdot\text{m}$ (ELU 8)
- **No meio do vão central ($x = 4{,}7\text{ m}$):**
  - $M_{sd,\min} = -127{,}08\text{ kN}\cdot\text{m}$ (com $\psi_0 = 0{,}7$) ou $-133{,}83\text{ kN}\cdot\text{m}$ (sem $\psi_0$)
  - $M_{sd,\max} = \mathbf{-65{,}80\text{ kN}\cdot\text{m}}$ (ELU 8)
- **Explicação física do diagrama de momentos:** Como os balanços laterais ($2{,}7\text{ m}$) são longos em relação ao vão central ($4{,}0\text{ m}$), toda a viga trabalha tracionada nas fibras superiores (**momento negativo ao longo de todo o comprimento**), apresentando dois picos negativos de $-354{,}33\text{ kN}\cdot\text{m}$ sobre os apoios $B$ e $C$ e aliviando até $-65{,}80\text{ kN}\cdot\text{m}$ no centro do vão.

### 1.7 Conclusão — O que torna o Exercício `1.4.1` de Nível Graduado?
- **Diferença para os exercícios comuns:** Nos níveis Iniciante e Intermediário de combinações, pede-se apenas o esforço máximo em 1 ou 2 pontos fixos onde todas as cargas somam no mesmo sentido. Aqui, pede-se **tanto o máximo quanto o mínimo** das reações e a **envoltória completa** ($V_{sd}(x)$ e $M_{sd}(x)$) em uma viga com **dois balanços e dois veículos independentes**.
- **O "Pulo do Gato" (Efeito Gangorra):** O centro de gravidade das duas rodas do Veículo 1 cai $0{,}20\text{ m}$ à esquerda do apoio $B$ ($x = 2{,}5\text{ m}$ vs. $x_B = 2{,}7\text{ m}$). Isso faz uma alavanca que **sobrecarrega o apoio $B$ ($+2{,}1\,q_{1d}$) e alivia o apoio oposto $C$ ($-0{,}1\,q_{1d}$)**.
- **Armadilha de Prova:** Quem coloca os dois caminhões ao mesmo tempo achando que isso gera a maior reação em $B$ erra ($482{,}18\text{ kN}$ ou $478{,}80\text{ kN}$ em vez de **$490{,}05\text{ kN}$ com apenas o Veículo 1**). Da mesma forma, a reação mínima ($176{,}75\text{ kN}$) não ocorre com a ponte vazia, mas sim com **peso próprio favorável ($\gamma_g = 1{,}00$) + apenas o caminhão do lado oposto** fazendo gangorra!

---

## 2. ARMADURA RETANGULAR SIMPLES — Exercício `3.4.1 Planta de escola` (p. 74)

### 2.1 Interpretação da Planta de Formas e Carregamento

Na planta de formas da p. 74, as vigas internas **V04** (apoiada em `P02` e `P06`) e **V05** (apoiada em `P03` e `P07`) são idênticas e simétricas:
- **Seção transversal:** $b_w = 25\text{ cm}$, $h = 70\text{ cm}$, $d = h - 5 = 65\text{ cm}$, espessura da laje $h_f = 12\text{ cm}$.
- **Vão de cálculo (eixo a eixo dos pilares):**
  $$\ell = 800\text{ cm} + \frac{25\text{ cm}}{2} + \frac{25\text{ cm}}{2} = 825\text{ cm} = 8{,}25\text{ m}$$
- **Carregamento característico em `V04` (e `V05`):**
  - Peso próprio da viga: $g_{1k} = 5\text{ kN/m}$
  - Reação de laje: cada viga interna recebe o quinhão de **duas** lajes adjacentes (`L01` e `L02` para `V04`; `L02` e `L03` para `V05`), sendo $15\text{ kN/m}$ por laje $\implies 2 \times 15 = 30\text{ kN/m}$
  - Peso de parede sobre a viga: $g_{2k} = 15\text{ kN/m}$
  - Carga total distribuída característica:
    $$p_k = 5 + 2 \times 15 + 15 = 50\text{ kN/m}$$
- **Esforço solicitante de cálculo no ELU (`BA1-w` em `BeamsDiagrams`):**
  - Usando o fator padrão $\gamma_f = 1{,}40$ dos capítulos de dimensionamento do Caderno:
    $$p_d = 1{,}40 \times 50 = 70\text{ kN/m}$$
    $$M_{sd} = \frac{p_d \ell^2}{8} = \frac{70 \times 8{,}25^2}{8} = 595{,}547\text{ kN}\cdot\text{m} = \mathbf{59554{,}69\text{ kN}\cdot\text{cm}}$$

---

### 2.2 Parâmetros dos Materiais (Blocos `[P]`, `[Q]`, `[T]`, `[U]`, `[W]`, `[AH]`, `[AI]`, `[AK]`, `[AL]`)

- **Concreto C35 ($f_{ck} = 35\text{ MPa} = 3{,}5\text{ kN/cm}^2 \le 50\text{ MPa}$) e Aço CA-50 ($f_{yk} = 500\text{ MPa} = 50\text{ kN/cm}^2$):**
  - **Bloco `[AI]` / `[H]`:** $\gamma_c = 1{,}40$, $\gamma_s = 1{,}15$
  - **Bloco `[AH]` / `[H]`:**
    $$f_{cd} = \frac{f_{ck}}{\gamma_c} = \frac{3{,}5}{1{,}40} = 2{,}50\text{ kN/cm}^2 \qquad f_{yd} = \frac{f_{yk}}{\gamma_s} = \frac{50}{1{,}15} = 43{,}478\text{ kN/cm}^2$$
  - **Bloco `[P]`:** $\beta_{x,lim} = 0{,}450$ ($f_{ck} \le 50\text{ MPa}$)
  - **Bloco `[Q]`:** $\zeta_c = 0{,}8$ ($f_{ck} \le 50\text{ MPa}$)
  - **Bloco `[T]` e `[W]`:** $\alpha_c = 0{,}85$, $\eta_c = \alpha_c = 0{,}85$ (seção não estreita no topo comprimido)
  - **Bloco `[U]`:**
    $$f_{ctk,sup} = 0{,}39\sqrt[3]{f_{ck}^2} = 0{,}39\sqrt[3]{35^2} = 4{,}173\text{ MPa} = 0{,}4173\text{ kN/cm}^2$$
  - **Bloco `[AK]` e `[AL]`:** $E_s = 21000\text{ kN/cm}^2$, $\varepsilon_{cu} = 3{,}5\text{‰} = 0{,}0035$

---

### 2.3 Resolução 2A — Dimensionamento como Seção Retangular Simples ($b_w = 25\text{ cm}$)

1. **Verificação do Momento Mínimo — Bloco `[R]`:**
   $$W_0 = \frac{b_w h^2}{6} = \frac{25 \times 70^2}{6} = 20416{,}67\text{ cm}^3$$
   $$M_{sd,min} = 0{,}8\, W_0\, f_{ctk,sup} = 0{,}8 \times 20416{,}67 \times 0{,}4173 = 6815{,}8\text{ kN}\cdot\text{cm} < M_{sd} = 59554{,}7\text{ kN}\cdot\text{cm} \quad \text{(OK!)}$$

2. **Verificação de Ductilidade / Armadura Simples — Bloco `[V]`:**
   $$M_{rd,lim} = 0{,}251\, b_w d^2 f_{cd} = 0{,}251 \times 25 \times 65^2 \times 2{,}50 = \mathbf{66279{,}69\text{ kN}\cdot\text{cm}}$$
   Como $M_{sd} = 59554{,}69\text{ kN}\cdot\text{cm} \le M_{rd,lim} = 66279{,}69\text{ kN}\cdot\text{cm}$, a seção resiste com **armadura simples** ($M'_{rd} = 0, A'_s = 0$ e $M_{rdw} = M_{sd}$)!

3. **Cálculo das Variáveis Adimensionais — Bloco `[S]`:**
   $$\beta_x = \frac{1}{\zeta_c} - \frac{1}{\zeta_c}\sqrt{1 - \frac{2 M_{rdw}}{\eta_c b_w d^2 f_{cd}}} = \frac{1}{0{,}8} - \frac{1}{0{,}8}\sqrt{1 - \frac{2 \times 59554{,}69}{0{,}85 \times 25 \times 65^2 \times 2{,}50}} = \mathbf{0{,}3936} \le \beta_{x,lim} = 0{,}450 \quad \text{(OK!)}$$
   $$\beta_y = \zeta_c \beta_x = 0{,}8 \times 0{,}3936 = 0{,}3149$$
   $$\beta_z = 1 - 0{,}5\beta_y = 1 - 0{,}5 \times 0{,}3149 = \mathbf{0{,}8425}$$
   $$\beta_s = \frac{E_s}{f_{yd}}\left(\frac{1 - \beta_x}{\beta_x}\right)\varepsilon_{cu} = \frac{21000}{43{,}478}\left(\frac{1 - 0{,}3936}{0{,}3936}\right) \times 0{,}0035 = 2{,}600 \ge 1{,}0 \implies \mathbf{\beta_s = 1{,}000}$$

4. **Área de Armadura de Tração e Verificação das Taxas — Blocos `[X]`, `[AA]` e `[AC]`:**
   - **Bloco `[X]`** (com $M'_{rd} = 0$):
     $$A_s = \frac{M_{rdw}}{\beta_z d \beta_s f_{yd}} = \frac{59554{,}69}{0{,}8425 \times 65 \times 1{,}000 \times 43{,}478} = \mathbf{25{,}012\text{ cm}^2}$$
   - **Bloco `[AA]` (Taxa mínima):**
     $$A_{s,min} = 0{,}15\%\, A_c = 0{,}0015 \times 25 \times 70 = 2{,}625\text{ cm}^2 \le 25{,}012\text{ cm}^2 \quad \text{(OK!)}$$
   - **Bloco `[AC]` (Taxa máxima):**
     $$A_{s,max} = 4\%\, A_c = 0{,}04 \times 25 \times 70 = 70{,}00\text{ cm}^2 \ge 25{,}012\text{ cm}^2 \quad \text{(OK!)}$$
   - **Escolha de barras — Blocos `[Y]` e `[AG]`:** adotando $\phi_\ell = 25\text{ mm} = 2{,}5\text{ cm}$:
     $$n_{\phi 25} = \left\lceil \frac{4 \times 25{,}012}{\pi \times 2{,}5^2} \right\rceil = \lceil 5{,}095 \rceil = \mathbf{6\,\phi\,25\text{ mm}} \quad \left(A_{s,ef} = \frac{6\pi \times 2{,}5^2}{4} = 29{,}452\text{ cm}^2\right)$$

---

### 2.4 Resolução 2B — Considerando a Colaboração do Painel de Lajes (Seção T Equivalente)

Como o enunciado pede para levar em conta, se possível, a colaboração do painel de lajes, e tanto `V04` quanto `V05` possuem lajes maciças de mesma espessura ($h_f = 12\text{ cm}$) de ambos os lados com $b_{li} = 400\text{ cm}$:
- Viga simplesmente apoiada: $a = \ell = 825\text{ cm}$
- Aba colaborante de cada lado: $b_a = \min(0{,}1 a;\, 0{,}5 b_{li}) = \min(82{,}5\text{ cm};\, 200\text{ cm}) = 82{,}5\text{ cm}$
- Largura colaborante da mesa: $b_f = b_w + 2 b_a = 25 + 2 \times 82{,}5 = \mathbf{190\text{ cm}}$
- **Verificação da posição da linha neutra na mesa — Bloco `[AM]`:**
  $$M_{rdf} = \eta_c h_f b_f \left(d - \frac{h_f}{2}\right) f_{cd} = 0{,}85 \times 12 \times 190 \times \left(65 - \frac{12}{2}\right) \times 2{,}50 = \mathbf{285855{,}0\text{ kN}\cdot\text{cm}}$$
  Como $M_{rdf} = 285855{,}0\text{ kN}\cdot\text{cm} \ge M_{sd} = 59554{,}69\text{ kN}\cdot\text{cm}$, pelo critério do **Bloco `[AM]`** ($M_{rdf} \ge M_{sd} \therefore \text{retangular equivalente de base } b_f$), a linha neutra fica dentro da laje ($y \le 12\text{ cm}$) e dimensionamos como **viga retangular simples de base $b_f = 190\text{ cm}$**:
  - **Bloco `[R]`:** $A_w = 1750\text{ cm}^2$, $A_a = (190 - 25)\times 12 = 1980\text{ cm}^2$, $A_T = 3730\text{ cm}^2$, $c = 50{,}394\text{ cm}$, $c' = 19{,}606\text{ cm}$, $W_0 = 161898{,}1\text{ cm}^3 \implies M_{sd,min} = 54047{,}4\text{ kN}\cdot\text{cm} < M_{sd}$ (OK!)
  - **Bloco `[S]`** (trocando $b_w$ por $b_f = 190\text{ cm}$):
    $$\beta_x = \frac{1}{0{,}8} - \frac{1}{0{,}8}\sqrt{1 - \frac{2 \times 59554{,}69}{0{,}85 \times 190 \times 65^2 \times 2{,}50}} = \mathbf{0{,}0444} \implies y = 0{,}8 \times 0{,}0444 \times 65 = 2{,}31\text{ cm} < 12\text{ cm}$$
    $$\beta_z = 1 - 0{,}4 \times 0{,}0444 = \mathbf{0{,}9822} \qquad \beta_s = 1{,}000$$
  - **Bloco `[X]`:**
    $$A_s = \frac{59554{,}69}{0{,}9822 \times 65 \times 1{,}000 \times 43{,}478} = \mathbf{21{,}454\text{ cm}^2} \quad \left(\ge A_{s,min} = 0{,}0015 \times 3730 = 5{,}595\text{ cm}^2\right)$$

### 2.5 Conclusão — O que torna o Exercício `3.4.1` de Nível Graduado?
- **Diferença para os exercícios comuns:** Nos níveis Iniciante/Intermediário, a viga já vem isolada com o vão $\ell$ e a carga distribuída $p_k$ desenhados. No Nível Graduado, você recebe a **planta de formas da edificação** e precisa **montar o modelo estrutural** antes de dimensionar.
- **Os 3 Pontos Especiais Cobrados:**
  1. **Vão teórico eixo a eixo:** A cota de $800\text{ cm}$ na planta é a distância livre entre faces das vigas/pilares; é preciso somar metade do pilar de cada lado ($\ell = 800 + 12{,}5 + 12{,}5 = 825\text{ cm}$).
  2. **Quinhão de carga de viga interna:** O enunciado informa a reação de *uma* laje ($15\text{ kN/m}$), mas pela planta vê-se que `V04` e `V05` são vigas internas entre salas de aula e recebem **duas lajes adjacentes** ($2 \times 15 = 30\text{ kN/m}$), totalizando $p_k = 5 + 30 + 15 = 50\text{ kN/m}$.
  3. **Por que há uma "Seção T" dentro do Capítulo de Armadura Retangular Simples?** Porque ao considerar a colaboração da laje ($b_f = 190\text{ cm}$, $h_f = 12\text{ cm}$), a linha neutra cai **dentro da espessura da laje** ($y = 2{,}31\text{ cm} \le 12\text{ cm}$, isto é, $M_{sd} \le M_{rdf}$ no Bloco `[AM]`). Assim, ela é dimensionada exatamente pelas fórmulas de **seção retangular simples** (trocando $b_w = 25\text{ cm}$ por $b_f = 190\text{ cm}$), economizando $14{,}2\%$ de aço!

---

## 3. ARMADURA RETANGULAR DUPLA — Exercício `4.3.9 Menor altura múltipla de 5` (p. 90–91)

> [!NOTE]
> **Por que escolhemos o `4.3.9` (p. 90–91)?** No PDF do Caderno de Exercícios, o item `4.4.1 Planta de escola` (p. 91–92) é uma repetição tipográfica idêntica do `3.4.1` (que resulta em armadura simples, $\beta_x < 0{,}45$). Já o exercício **`4.3.9`** (imediatamente anterior, na p. 90–91, com gabarito oficial impresso) percorre todas as etapas de dimensionamento e detalhamento de **Armadura Retangular Dupla** em múltiplas camadas.

### 3.1 Enunciado e Diagrama da Viga

```text
                Qk = 40 kN                Qk = 40 kN
                    |                         |
                    v      gk = 20 kN/m       v
      ↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
      A=============B=========================C=============D
      ^             |<--------- 4 m --------->|             ^
      |<--- 2 m --->|                         |<--- 2 m --->|
      R_A                                                   R_D
```

- **Dados:** Concreto C30 ($f_{ck} = 30\text{ MPa} = 3{,}0\text{ kN/cm}^2$), Aço CA-50 ($f_{yk} = 50\text{ kN/cm}^2$), $b_w = 20\text{ cm}$, $\phi_t = 5{,}0\text{ mm} = 0{,}5\text{ cm}$, $d_{max} = 20\text{ mm} = 2{,}0\text{ cm}$, $c_{nom} = 25\text{ mm} = 2{,}5\text{ cm}$, $\phi_\ell = 20\text{ mm} = 2{,}0\text{ cm}$ (tração) e $\phi'_\ell = 12{,}5\text{ mm} = 1{,}25\text{ cm}$ (compressão).
- **Pede-se:**
  - **(a)** A menor altura $h$ (arredondada para múltiplo de $5\text{ cm}$) para que as seções **B e C** estejam no limite de ductilidade sem armadura de compressão;
  - **(b)** As armaduras longitudinais ($A_s$ e $A'_s$) no **meio do vão AD** mantida a altura $h$ do item (a).

---

### 3.2 Parâmetros dos Materiais e Espaçamentos (Blocos `[P]`, `[Q]`, `[T]`, `[AF]`, `[AH]`, `[AI]`)

- **Blocos `[AH]` e `[AI]`:**
  $$f_{cd} = \frac{3{,}0}{1{,}40} = 2{,}143\text{ kN/cm}^2 \qquad f_{yd} = \frac{50}{1{,}15} = 43{,}478\text{ kN/cm}^2$$
- **Blocos `[P]`, `[Q]`, `[T]`, `[W]`:** $\beta_{x,lim} = 0{,}450$, $\zeta_c = 0{,}8$, $\eta_c = \alpha_c = 0{,}85$.
- **Espaçamentos livres mínimos — Bloco `[AF]`:**
  - Para a armadura de tração ($\phi_\ell = 2{,}0\text{ cm}, d_{max} = 2{,}0\text{ cm}$):
    $$a_h \ge \max\begin{cases} 2{,}0\text{ cm} \\ 2{,}0\text{ cm} \\ 1{,}2 \times 2{,}0 = 2{,}4\text{ cm} \end{cases} \implies \mathbf{a_h = 2{,}4\text{ cm}} \qquad a_v \ge \max\begin{cases} 2{,}0\text{ cm} \\ 2{,}0\text{ cm} \\ 0{,}5 \times 2{,}0 = 1{,}0\text{ cm} \end{cases} \implies \mathbf{a_v = 2{,}0\text{ cm}}$$
  - Para a armadura de compressão ($\phi'_\ell = 1{,}25\text{ cm}$): $a'_h = 2{,}4\text{ cm}$, $a'_v = 2{,}0\text{ cm}$.

---

### 3.3 Resolução do Item (a) — Altura $h$ pela Condição Limite em B e C

1. **Momento Fletor Solicitante nas Seções B ($x = 2\text{ m}$) e C ($x = 6\text{ m}$):**
   - Viga biapoiada simétrica de vão total $L = 2 + 4 + 2 = 8\text{ m}$ (`BA1-w` + `BA9-ff` em `BeamsDiagrams`):
     - Reação pela carga permanente $g_k = 20\text{ kN/m}$: $R_{A,g} = \frac{20 \times 8}{2} = 80\text{ kN} \implies M_{B,gk} = 80 \times 2 - \frac{20 \times 2^2}{2} = 120\text{ kN}\cdot\text{m}$
     - Reação pelas duas cargas $Q_k = 40\text{ kN}$: $R_{A,q} = 40\text{ kN} \implies M_{B,qk} = 40 \times 2 = 80\text{ kN}\cdot\text{m}$
     - No ELU ($\gamma_f = 1{,}40$):
       $$M_{sd,B} = 1{,}40 \times (120 + 80) = 280\text{ kN}\cdot\text{m} = \mathbf{28000\text{ kN}\cdot\text{cm}}$$

2. **Altura útil limite sem armadura de compressão — Bloco `[V]`:**
   $$M_{rd,lim} = 0{,}251\, b_w d^2 f_{cd} \ge M_{sd,B} \implies d_{lim} = \sqrt{\frac{28000}{0{,}251 \times 20 \times 2{,}143}} = \mathbf{51{,}02\text{ cm}}$$

3. **Altura total $h$ — Bloco `[AJ]`:**
   - Com 1 camada inicial ($y_s = 0$):
     $$h = d + c_{nom} + \phi_t + 0{,}5\phi_\ell = 51{,}02 + 2{,}5 + 0{,}5 + 1{,}0 = 55{,}02\text{ cm}$$
   - Arredondando para o múltiplo de $5\text{ cm}$ mais próximo:
     $$\mathbf{h = 55\text{ cm}}$$

---

### 3.4 Resolução do Item (b) — Armadura Dupla no Meio do Vão AD ($x = 4\text{ m}$)

1. **Momento Fletor Solicitante no Meio do Vão ($x = 4\text{ m}$):**
   - Pela carga distribuída $g_k = 20\text{ kN/m}$: $M_{\text{meio},gk} = \frac{20 \times 8^2}{8} = 160\text{ kN}\cdot\text{m}$
   - Pelas duas cargas simétricas $Q_k = 40\text{ kN}$ (`BA9-ff`, trecho central constante): $M_{\text{meio},qk} = 40 \times 2 = 80\text{ kN}\cdot\text{m}$
   - Momento de cálculo no meio do vão *(nota: tanto $1{,}4(160+80)$ quanto $1{,}35(160) + 1{,}5(80)$ resultam exatamente no mesmo valor!)*:
     $$M_{sd} = 1{,}40 \times (160 + 80) = 1{,}35 \times 160 + 1{,}50 \times 80 = 336\text{ kN}\cdot\text{m} = \mathbf{33600\text{ kN}\cdot\text{cm}}$$

2. **Capacidade de Barras por Camada e Alturas Úteis $d$ e $d'$ — Blocos `[Z]`, `[AE]` e `[AJ]`:**
   - Número máximo de barras de $\phi_\ell = 2{,}0\text{ cm}$ por camada (**Bloco `[Z]`**):
     $$n_{\phi_\ell,\text{cam}} \le \left\lfloor \frac{b_w - 2 c_{nom} - 2 \phi_t + a_h}{\phi_\ell + a_h} \right\rfloor = \left\lfloor \frac{20 - 2(2{,}5) - 2(0{,}5) + 2{,}4}{2{,}0 + 2{,}4} \right\rfloor = \lfloor 3{,}727 \rfloor = \mathbf{3\text{ barras/camada}}$$
   - Para $\phi'_\ell = 1{,}25\text{ cm}$ na compressão (**Bloco `[Z]`**):
     $$n'_{\phi'_\ell,\text{cam}} \le \left\lfloor \frac{20 - 5 - 1 + 2{,}4}{1{,}25 + 2{,}4} \right\rfloor = \lfloor 4{,}49 \rfloor = \mathbf{4\text{ barras/camada}}$$
   - Como na tração serão necessárias 6 barras de $20\text{ mm}$ dispostas em **2 camadas de 3 barras**, o centro de gravidade das camadas (**Bloco `[AE]`**) com $y_{\phi 1} = 0$ e $y_{\phi 2} = \phi_\ell + a_v = 2{,}0 + 2{,}0 = 4{,}0\text{ cm}$ é:
     $$y_s = \frac{3 A_{\phi 20}(0) + 3 A_{\phi 20}(4{,}0)}{6 A_{\phi 20}} = \mathbf{2{,}00\text{ cm}}$$
   - Alturas úteis (**Bloco `[AJ]`**):
     $$d = h - c_{nom} - \phi_t - 0{,}5\phi_\ell - y_s = 55 - 2{,}5 - 0{,}5 - 1{,}0 - 2{,}0 = \mathbf{49{,}00\text{ cm}}$$
     $$d' = c_{nom} + \phi_t + 0{,}5\phi'_\ell + y'_s = 2{,}5 + 0{,}5 + 0{,}625 + 0 = \mathbf{3{,}625\text{ cm}}$$

3. **Decomposição do Momento para Armadura Dupla — Blocos `[V]` e `[X]`:**
   - **Bloco `[V]`:**
     $$M_{rd,lim} = 0{,}251\, b_w d^2 f_{cd} = 0{,}251 \times 20 \times 49{,}0^2 \times 2{,}143 = \mathbf{25827{,}90\text{ kN}\cdot\text{cm}}$$
   - Como $M_{sd} = 33600\text{ kN}\cdot\text{cm} > M_{rd,lim} = 25827{,}90\text{ kN}\cdot\text{cm}$, a seção exige **armadura dupla**!
   - Fixamos $M_{rdw} = M_{rd,lim} = 25827{,}90\text{ kN}\cdot\text{cm}$ (com $\beta_x = \beta_{x,lim} = 0{,}450$) e calculamos a parcela da armadura comprimida (**Bloco `[X]`**):
     $$M'_{rd} = M_{sd} - M_{rd,lim} = 33600 - 25827{,}90 = \mathbf{7772{,}10\text{ kN}\cdot\text{cm}}$$

4. **Variáveis Adimensionais em $\beta_x = \beta_{x,lim} = 0{,}450$ — Bloco `[S]`:**
   $$\beta_y = \zeta_c \beta_x = 0{,}8 \times 0{,}450 = 0{,}360 \qquad \beta_z = 1 - 0{,}5\beta_y = \mathbf{0{,}820}$$
   $$\beta_s = \frac{21000}{43{,}478}\left(\frac{1 - 0{,}450}{0{,}450}\right) \times 0{,}0035 = 2{,}066 \ge 1{,}0 \implies \mathbf{\beta_s = 1{,}000}$$
   $$\beta'_s = \frac{21000}{43{,}478}\left(\frac{0{,}450 - \dfrac{3{,}625}{49{,}0}}{0{,}450}\right) \times 0{,}0035 = 1{,}412 \ge 1{,}0 \implies \mathbf{\beta'_s = 1{,}000}$$

5. **Cálculo de $A_s$ e $A'_s$ e Quantidade de Barras — Blocos `[X]` e `[Y]`:**
   - **Bloco `[X]`:**
     $$A_s = \left[\frac{M_{rdw}}{\beta_z d} + \frac{M'_{rd}}{(d - d')}\right]\frac{1}{\beta_s f_{yd}} = \left[\frac{25827{,}90}{0{,}820 \times 49{,}0} + \frac{7772{,}10}{49{,}0 - 3{,}625}\right]\frac{1}{1{,}000 \times 43{,}478} = \mathbf{18{,}724\text{ cm}^2}$$
     $$A'_s = \frac{M'_{rd}}{(d - d')\beta'_s f_{yd}} = \frac{7772{,}10}{(49{,}0 - 3{,}625) \times 1{,}000 \times 43{,}478} = \mathbf{3{,}940\text{ cm}^2}$$
   - **Bloco `[Y]`:**
     $$n_{\phi 20} = \left\lceil \frac{4 \times 18{,}724}{\pi \times 2{,}0^2} \right\rceil = \lceil 5{,}960 \rceil = \mathbf{6\,\phi\,20\text{ mm}} \quad \text{(em 2 camadas de 3 barras)}$$
     $$n'_{\phi 12{,}5} = \left\lceil \frac{4 \times 3{,}940}{\pi \times 1{,}25^2} \right\rceil = \lceil 3{,}211 \rceil = \mathbf{4\,\phi\,12{,}5\text{ mm}} \quad \text{(em 1 camada de 4 barras)}$$

6. **Verificações Finais — Blocos `[AG]`, `[AA]`, `[AC]` e `[AB]`:**
   - **Bloco `[AG]`:** $A_{s,ef} = 6 \times \frac{\pi \times 2{,}0^2}{4} = 18{,}850\text{ cm}^2$; $A'_{s,ef} = 4 \times \frac{\pi \times 1{,}25^2}{4} = 4{,}909\text{ cm}^2$.
   - **Bloco `[AA]`:** $\rho_{min} = \frac{18{,}850}{20 \times 55} = 1{,}71\% \ge 0{,}15\%$ (OK!).
   - **Bloco `[AC]`:** $\rho_{max} = \frac{18{,}850 + 4{,}909}{20 \times 55} = \frac{23{,}759}{1100} = 2{,}16\% \le 4\%$ (OK!).
   - **Bloco `[AB]` (Verificação da linha neutra com áreas efetivas):**
     $$\beta_x = \frac{f_{yd}}{\eta_c \zeta_c b_w d f_{cd}}\left(A_{s,ef}\beta_s - A'_{s,ef}\beta'_s\right) = \frac{43{,}478}{0{,}85 \times 0{,}8 \times 20 \times 49{,}0 \times 2{,}143}\left(18{,}850 \times 1{,}0 - 4{,}909 \times 1{,}0\right) = \mathbf{0{,}4245} \le \beta_{x,lim} = 0{,}450 \quad \text{(OK!)}$$
   - **Conferência com o gabarito oficial do Caderno (p. 91):** `a) h = 55 cm; b) 6 φ 20 mm em 2 camadas e 4 φ 12,5 mm em 1 camada` — **exato!**

### 3.5 Conclusão — O que torna o Exercício `4.3.9` de Nível Graduado?
- **Diferença para os exercícios comuns:** Exercícios básicos de armadura dupla já fornecem $h$, $d$ e $d'$ prontos e pedem apenas a aplicação direta de $M'_{rd} = M_{sd} - M_{rd,lim}$. Aqui, há um **acoplamento entre duas seções diferentes da viga** aliado ao **detalhamento real em múltiplas camadas**.
- **Os 3 Pontos Especiais Cobrados:**
  1. **Dimensionamento geométrico inverso no Item (a):** Nas seções B e C ($M_{sd,B} = 280\text{ kN}\cdot\text{m}$), você impõe a fronteira exata entre armadura simples e dupla ($M_{sd,B} = M_{rd,lim} = 0{,}251\,b_w d_{lim}^2 f_{cd}$, Bloco `[V]`) para encontrar $d_{lim} = 51{,}02\text{ cm}$, somar cobrimento + estribo + meia barra (1 camada, Bloco `[AJ]`) e fixar $h = 55\text{ cm}$.
  2. **Efeito cascata do alojamento em 2 camadas no Item (b):** Ao passar para o meio do vão ($M_{sd} = 336\text{ kN}\cdot\text{m}$), a largura $b_w = 20\text{ cm}$ comporta no máximo **3 barras de $\phi 20\text{ mm}$ por camada** (Bloco `[Z]`). Como são necessárias 6 barras, elas formam **2 camadas**, deslocando o centro de gravidade em $y_s = 2{,}0\text{ cm}$ (Bloco `[AE]`) e **reduzindo a altura útil real de $51\text{ cm}$ para $d = 49{,}0\text{ cm}$** (Bloco `[AJ]`).
  3. **Verificação da linha neutra efetiva após escolha comercial (`[AB]`):** Como o número de barras comprimidas é arredondado para cima ($4\phi 12{,}5\text{ mm} \implies A'_{s,ef} = 4{,}909\text{ cm}^2 > 3{,}940\text{ cm}^2$), a linha neutra efetiva recua para $\beta_{x,ef} = 0{,}4245 \le 0{,}450$, garantindo a ductilidade real da peça.

---

## 4. ARMADURA T SIMPLES — Exercício `5.4.3 Largura colaborante e máximo carregamento` (p. 107–108)

### 4.1 Interpretação da Planta e do Corte Transversal

Na p. 108, temos a viga central **V2 ($20 \times 55\text{ cm}$)** apoiada nos pilares **P3 e P4** com vão $\ell = 8\text{ m} = 800\text{ cm}$:
- **Seção transversal:** $b_w = 20\text{ cm}$, $h = 55\text{ cm}$, $d = h - 5 = 50\text{ cm}$, espessura das lajes $h_f = 8\text{ cm}$.
- **Painéis de laje adjacentes a V2:**
  - Acima: laje `L1` (entre `V1` e `V2`), distância livre entre faces $b_{li,1} = 400\text{ cm}$.
  - Abaixo: laje `L2` (entre `V2` e `V3`), distância livre entre faces $b_{li,2} = 200\text{ cm}$.
- **Materiais:** Concreto C35 ($f_{cd} = 3{,}5/1{,}40 = 2{,}50\text{ kN/cm}^2$), Aço CA-50 ($f_{yd} = 50/1{,}15 = 43{,}478\text{ kN/cm}^2$).
- **Carregamento:** permanente $g_k = 20\text{ kN/m}$ (peso próprio incluído) e variável $q_k$ a determinar.

---

### 4.2 Item (a) — Máximo Valor Possível para $b_f$

1. **Distância entre pontos de momento nulo ($a$):**
   - Viga `V2` simplesmente apoiada em `P3` e `P4`:
     $$a = \ell = 800\text{ cm}$$
2. **Largura de cada aba colaborante ($b_a$):**
   - Para manter a simetria da seção T:
     $$b_a \le \min\begin{cases} 0{,}1\, a = 0{,}1 \times 800 = 80\text{ cm} \\ 0{,}5\, b_{li,1} = 0{,}5 \times 400 = 200\text{ cm} \\ 0{,}5\, b_{li,2} = 0{,}5 \times 200 = 100\text{ cm} \end{cases} \implies \mathbf{b_a = 80\text{ cm}}$$
3. **Largura colaborante total da mesa ($b_f$):**
   $$b_f = b_w + 2 b_a = 20 + 2 \times 80 = \mathbf{180\text{ cm}}$$

---

### 4.3 Item (b) — Máximo Carregamento $q_k$ para Linha Neutra em $1{,}25\,h_f$

No enunciado, pede-se o máximo carregamento $q_k$ admitindo-se que a altura da linha neutra na seção de máxima solicitação seja igual a $1{,}25\,h_f$. Apresentamos abaixo o cálculo para as duas leituras possíveis do termo ("altura da linha neutra $x = 1{,}25\,h_f$" e "altura do diagrama comprimido $y = 1{,}25\,h_f$"):

#### Caso Principal: Profundidade da Linha Neutra $x = 1{,}25\,h_f$ (com $y = \zeta_c x = h_f$)
1. **Posição da linha neutra e variáveis adimensionais — Blocos `[Q]` e `[S]`:**
   $$x = 1{,}25\, h_f = 1{,}25 \times 8 = \mathbf{10{,}0\text{ cm}}$$
   $$\beta_x = \frac{x}{d} = \frac{10{,}0}{50{,}0} = \mathbf{0{,}200} \le \beta_{x,lim} = 0{,}450 \quad \text{(Domínio 2, dúctil — Bloco [P])}$$
   $$\beta_y = \zeta_c \beta_x = 0{,}8 \times 0{,}200 = 0{,}160 \quad \left(y = \beta_y d = 8{,}0\text{ cm} = h_f\right)$$
   $$\beta_z = 1 - 0{,}5\beta_y = 1 - 0{,}5 \times 0{,}160 = \mathbf{0{,}920}$$
   $$\beta_s = \frac{21000}{43{,}478}\left(\frac{1 - 0{,}200}{0{,}200}\right)\times 0{,}0035 = 6{,}762 \ge 1{,}0 \implies \mathbf{\beta_s = 1{,}000}$$

2. **Momento Resistente da Seção T — Blocos `[AM]` e `[S]`:**
   - Parcela das abas da mesa (**Bloco `[AM]`**):
     $$M_{rda} = \eta_c h_f (b_f - b_w)\left(d - \frac{h_f}{2}\right) f_{cd} = 0{,}85 \times 8 \times (180 - 20) \times \left(50 - \frac{8}{2}\right) \times 2{,}50 = \mathbf{125120{,}0\text{ kN}\cdot\text{cm}}$$
   - Parcela da alma (**Bloco `[S]`**):
     $$M_{rdw} = \eta_c \zeta_c \beta_x \beta_z b_w d^2 f_{cd} = 0{,}85 \times 0{,}8 \times 0{,}200 \times 0{,}920 \times 20 \times 50^2 \times 2{,}50 = \mathbf{15640{,}0\text{ kN}\cdot\text{cm}}$$
   - Momento total resistente (**Bloco `[AM]`**, sem armadura comprimida $M'_{rd} = 0$):
     $$M_{sd} = M_{rd} = M_{rda} + M_{rdw} = 125120{,}0 + 15640{,}0 = \mathbf{140760{,}0\text{ kN}\cdot\text{cm}} = 1407{,}60\text{ kN}\cdot\text{m}$$

3. **Determinação de $q_k$ (`BA1-w` em `BeamsDiagrams`):**
   - Para o vão biapoiado $\ell = 8\text{ m}$:
     $$M_{sd} = \frac{p_d \ell^2}{8} \implies p_d = \frac{8 \times 1407{,}60}{8^2} = \mathbf{175{,}95\text{ kN/m}}$$
   - Com $\gamma_g = \gamma_q = 1{,}40$ (padrão dos exemplos de dimensionamento do Caderno):
     $$1{,}40(g_k + q_k) = 175{,}95 \implies 20 + q_k = 125{,}679 \implies \mathbf{q_k = 105{,}679\text{ kN/m}}$$
   - *(Ou usando a tabela do Formulário 1, Blocos **`[C]`** e **`[E]`**, com $\gamma_g = 1{,}35$ e $\gamma_q = 1{,}50$: $1{,}35(20) + 1{,}50\,q_k = 175{,}95 \implies \mathbf{q_k = 99{,}300\text{ kN/m}}$.)*

> **Variante caso o enunciado refira-se a $y = 1{,}25\,h_f = 10\text{ cm}$ ($x = y/\zeta_c = 12{,}5\text{ cm}$):**
> - $\beta_x = 12{,}5/50 = 0{,}250$, $\beta_y = 0{,}200$, $\beta_z = 0{,}900$, $\beta_s = 1{,}000$.
> - $M_{rda} = 125120{,}0\text{ kN}\cdot\text{cm}$ e $M_{rdw} = 0{,}85 \times 0{,}8 \times 0{,}250 \times 0{,}900 \times 20 \times 50^2 \times 2{,}50 = 19125{,}0\text{ kN}\cdot\text{cm}$.
> - $M_{sd} = 125120{,}0 + 19125{,}0 = \mathbf{144245{,}0\text{ kN}\cdot\text{cm}} = 1442{,}45\text{ kN}\cdot\text{m} \implies p_d = 180{,}306\text{ kN/m}$.
> - Daí resulta $\mathbf{q_k = 108{,}790\text{ kN/m}}$ (para $\gamma_f = 1{,}40$) ou $\mathbf{q_k = 102{,}204\text{ kN/m}}$ (para $\gamma_g = 1{,}35, \gamma_q = 1{,}50$).

---

### 4.4 Item (c) — Armadura Longitudinal Necessária ($A_s$) — Blocos `[AM]`, `[AA]` e `[AC]`

1. **Equação de $A_s$ para Seção T — Bloco `[AM]` (com $M'_{rd} = 0$):**
   - Para $x = 10{,}0\text{ cm}$ ($M_{sd} = 140760\text{ kN}\cdot\text{cm}$):
     $$A_s = \left[\frac{M_{rda}}{\left(d - \dfrac{h_f}{2}\right)} + \frac{M_{rdw}}{\beta_z d}\right]\frac{1}{\beta_s f_{yd}} = \left[\frac{125120{,}0}{50 - 4} + \frac{15640{,}0}{0{,}920 \times 50}\right]\frac{1}{1{,}000 \times 43{,}478} = \mathbf{70{,}380\text{ cm}^2}$$
   - Para $y = 10{,}0\text{ cm}$ ($M_{sd} = 144245\text{ kN}\cdot\text{cm}$):
     $$A_s = \left[\frac{125120{,}0}{46} + \frac{19125{,}0}{0{,}900 \times 50}\right]\frac{1}{1{,}000 \times 43{,}478} = \mathbf{72{,}335\text{ cm}^2}$$

2. **Verificação das Taxas Mínima e Máxima — Blocos `[R]`, `[AA]` e `[AC]`:**
   - Área da seção T (**Bloco `[R]`**):
     $$A_T = b_w h + (b_f - b_w)h_f = 20 \times 55 + (180 - 20) \times 8 = 1100 + 1280 = \mathbf{2380\text{ cm}^2}$$
   - **Bloco `[AA]`:** $A_{s,min} = 0{,}0015 \times 2380 = 3{,}57\text{ cm}^2 \le A_s$ (OK!)
   - **Bloco `[AC]`:** $A_{s,max} = 0{,}04 \times 2380 = 95{,}20\text{ cm}^2 \ge A_s$ (OK!)

### 4.5 Conclusão — O que torna o Exercício `5.4.3` de Nível Graduado?
- **Diferença para os exercícios comuns:** Em vez do fluxo direto ($q_k \to M_{sd} \to \text{testar } M_{rdf} \to A_s$), este exercício propõe um **problema inverso com vínculo interno na posição da linha neutra** dentro de uma planta de formas assimétrica.
- **Os 3 Pontos Especiais Cobrados:**
  1. **Largura colaborante $b_f$ limitada pela simetria em planta assimétrica:** A viga `V2` tem uma laje de $400\text{ cm}$ de um lado e outra de $200\text{ cm}$ do outro, além de vão livre de $780\text{ cm}$ entre pilares de $20\text{ cm}$ ($\ell = 800\text{ cm}$). Para manter a seção T simétrica sem introduzir flexão oblíqua, adota-se para ambos os lados o menor limite entre $0{,}1a = 80\text{ cm}$, $0{,}5\,b_{li,1} = 200\text{ cm}$ e $0{,}5\,b_{li,2} = 100\text{ cm}$, resultando em $b_a = 80\text{ cm} \implies b_f = 180\text{ cm}$.
  2. **Engenharia reversa a partir da linha neutra fixada ($1{,}25\,h_f$):** Ao impor $x = 1{,}25\,h_f = 10{,}0\text{ cm}$ (ou $y = 1{,}25\,h_f = 10{,}0\text{ cm}$), você já conhece $\beta_x$ de partida! A partir de $\beta_x$, calcula diretamente a capacidade resistente das abas ($M_{rda}$) e da alma ($M_{rdw}$) pelo Bloco `[AM]`, soma $M_{rd} = M_{rda} + M_{rdw}$ e iguala a $\frac{p_d\ell^2}{8}$ para descobrir a carga variável máxima $q_k$.
  3. **Atenção à nomenclatura ($x$ vs. $y = \zeta_c x$):** Na prova, sempre deixe explícito se está adotando $x = 1{,}25\,h_f$ (profundidade real da linha neutra, onde $y = 0{,}8x = h_f$) ou $y = 1{,}25\,h_f$ (altura do bloco retangular comprimido, onde $x = 1{,}5625\,h_f$), pois o equacionamento de $M_{rda} + M_{rdw}$ no Bloco `[AM]` vale para ambos!

---

## 5. ARMADURA T DUPLA — Exercício `6.4.1 Máxima carga móvel possível em viga T` (p. 122–123)

### 5.1 Interpretação da Geometria, Seções Transversais e Carga Móvel

```text
                        Qk (móvel)
                            |
                            v      gk = 5,357 kN/m (peso próprio)
      =============================================================
            A                                       B
      <-2m->^<---------------- 8 m ---------------->^<-2m->
```

- **Geometria longitudinal:** viga com balanço esquerdo de $2\text{ m}$, vão central $AB$ de $8\text{ m}$ e balanço direito de $2\text{ m}$.
- **Geometria da seção T isolada:** $b_f = 60\text{ cm}$, $h_f = 10\text{ cm}$, $b_w = 25\text{ cm}$, altura da alma abaixo da mesa $= 75\text{ cm} \implies h = 10 + 75 = 85\text{ cm}$, $d = 80\text{ cm}$, $d' = 5\text{ cm}$.
- **Materiais (Blocos `[AH]` e `[AI]`):** Concreto C35 ($f_{cd} = 3{,}5/1{,}40 = 2{,}50\text{ kN/cm}^2$), Aço CA-50 ($f_{yd} = 50/1{,}15 = 43{,}478\text{ kN/cm}^2$).
- **Armaduras existentes na viga (Bloco `[AG]`):**
  1. **No meio do vão AB (momento positivo — mesa superior comprimida, alma inferior tracionada):**
     - Armadura de tração inferior: $3\,\phi\,20\text{ mm} \implies A_{s,ef} = \frac{3\pi \times 2{,}0^2}{4} = \mathbf{9{,}425\text{ cm}^2}$
     - Armadura de compressão superior: $A'_{s,ef} = 0$
  2. **Nos apoios A e B (momento negativo — mesa superior tracionada, alma inferior $b_w = 25\text{ cm}$ comprimida com armadura dupla!):**
     - Armadura de tração superior: $4\,\phi\,16\text{ mm} \implies A_{s,ef} = \frac{4\pi \times 1{,}6^2}{4} = \mathbf{8{,}042\text{ cm}^2}$
     - Armadura de compressão inferior: $2\,\phi\,10\text{ mm} \implies A'_{s,ef} = \frac{2\pi \times 1{,}0^2}{4} = \mathbf{1{,}571\text{ cm}^2}$

---

### 5.2 Passo 1 — Verificação da Largura Colaborante $b_f$

- Para o momento positivo no vão central $AB$ ($\ell = 800\text{ cm}$) de viga com momentos negativos nas duas extremidades:
  $$a = 0{,}6\,\ell = 0{,}6 \times 800 = 480\text{ cm}$$
- Limite de cada aba: $b_a \le 0{,}1\,a = 48\text{ cm}$. Como a aba real da viga isolada mede $b_a = \frac{60 - 25}{2} = 17{,}5\text{ cm} \le 48\text{ cm}$ (e na observação $b_3 = b_4$, toda a aba física colabora), confirma-se $\mathbf{b_f = 60\text{ cm}}$ na região de momento positivo!

---

### 5.3 Passo 2 — Momento Resistente Positivo no Meio do Vão AB (Blocos `[AM]` e `[S]`)

1. **Posição da linha neutra com $A_{s,ef} = 9{,}425\text{ cm}^2$ e base comprimida $b_f = 60\text{ cm}$ — Bloco `[AB]` / `[AM]`:**
   - Admitindo inicialmente $y \le h_f = 10\text{ cm}$ (seção retangular equivalente de largura $b_f = 60\text{ cm}$) e $\beta_s = 1{,}000$:
     $$\beta_x = \frac{f_{yd} A_{s,ef}}{\eta_c \zeta_c b_f d f_{cd}} = \frac{43{,}478 \times 9{,}425}{0{,}85 \times 0{,}8 \times 60 \times 80 \times 2{,}50} = \mathbf{0{,}0502} \le \beta_{x,lim} = 0{,}450$$
   - Altura comprimida $y$ (**Bloco `[S]`**):
     $$y = \zeta_c \beta_x d = 0{,}8 \times 0{,}0502 \times 80 = \mathbf{3{,}21\text{ cm}} \le h_f = 10\text{ cm} \quad \text{(Confirma seção retangular equivalente!)}$$
   - Braço de alavanca relativo (**Bloco `[S]`**):
     $$\beta_z = 1 - 0{,}4\beta_x = 1 - 0{,}4 \times 0{,}0502 = \mathbf{0{,}9799}$$

2. **Momento Resistente Positivo no Vão ($M_{rd,\text{vão}}^+$) — Bloco `[S]`:**
   $$M_{rd,\text{vão}}^+ = \eta_c \zeta_c \beta_x \beta_z b_f d^2 f_{cd} = 0{,}85 \times 0{,}8 \times 0{,}0502 \times 0{,}9799 \times 60 \times 80^2 \times 2{,}50 = \mathbf{32123{,}35\text{ kN}\cdot\text{cm}} = 321{,}234\text{ kN}\cdot\text{m}$$

---

### 5.4 Passo 3 — Momento Resistente Negativo nos Apoios A e B (Armadura Dupla — Blocos `[AB]`, `[S]` e `[X]`)

Nos apoios A e B, o momento fletor é **negativo** (traciona a mesa superior e comprime a base da alma inferior de largura $b_w = 25\text{ cm}$). Logo, a seção trabalha como **retangular de largura $b_w = 25\text{ cm}$ com armadura dupla** ($A_{s,ef} = 8{,}042\text{ cm}^2$ e $A'_{s,ef} = 1{,}571\text{ cm}^2$):

1. **Determinação da linha neutra $\beta_x$ por equilíbrio — Blocos `[AB]` e `[S]`:**
   $$\beta_x = \frac{f_{yd}}{\eta_c \zeta_c b_w d f_{cd}}\left(A_{s,ef}\beta_s - A'_{s,ef}\beta'_s\right) = \frac{43{,}478}{0{,}85 \times 0{,}8 \times 25 \times 80 \times 2{,}50}\left(8{,}042\,\beta_s - 1{,}571\,\beta'_s\right)$$
   $$\beta_x = 0{,}1029\,\beta_s - 0{,}0201\,\beta'_s$$
   - Como $\beta_x < 0{,}259$, a armadura tracionada escoa ($\beta_s = 1{,}000$), mas a armadura comprimida próxima à borda ($d'/d = 5/80 = 0{,}0625$) não atinge o escoamento ($\beta'_s < 1{,}0$). Substituindo a expressão de $\beta'_s$ do **Bloco `[S]`**:
     $$\beta'_s = \frac{E_s}{f_{yd}}\left(\frac{\beta_x - d'/d}{\beta_x}\right)\varepsilon_{cu} = \frac{21000}{43{,}478}\left(\frac{\beta_x - 0{,}0625}{\beta_x}\right)\times 0{,}0035 = 1{,}6905\left(\frac{\beta_x - 0{,}0625}{\beta_x}\right)$$
   - Resolvendo a equação de equilíbrio para $\beta_x$:
     $$\beta_x = 0{,}1029 - 0{,}0201 \times 1{,}6905\left(\frac{\beta_x - 0{,}0625}{\beta_x}\right) \implies \beta_x^2 - 0{,}0689\,\beta_x - 0{,}002124 = 0$$
     $$\mathbf{\beta_x = 0{,}0920} \le \beta_{x,lim} = 0{,}450 \quad \text{(OK!)}$$
   - Parâmetros correspondentes (**Bloco `[S]`**):
     $$\beta'_s = 1{,}6905\left(\frac{0{,}0920 - 0{,}0625}{0{,}0920}\right) = \mathbf{0{,}5416} \qquad \beta_z = 1 - 0{,}4 \times 0{,}0920 = \mathbf{0{,}9632}$$

2. **Momento Resistente Negativo nos Apoios ($M_{rd,\text{apoio}}^-$) — Blocos `[S]` e `[X]`:**
   - Parcela do concreto comprimido (**Bloco `[S]`**):
     $$M_{rdw} = \eta_c \zeta_c \beta_x \beta_z b_w d^2 f_{cd} = 0{,}85 \times 0{,}8 \times 0{,}0920 \times 0{,}9632 \times 25 \times 80^2 \times 2{,}50 = 24105{,}54\text{ kN}\cdot\text{cm}$$
   - Parcela da armadura comprimida (**Bloco `[X]`**):
     $$M'_{rd} = A'_{s,ef} \beta'_s f_{yd} (d - d') = 1{,}571 \times 0{,}5416 \times 43{,}478 \times (80 - 5) = 2763{,}15\text{ kN}\cdot\text{cm}$$
   - Momento resistente negativo total:
     $$M_{rd,\text{apoio}}^- = M_{rdw} + M'_{rd} = 24105{,}54 + 2763{,}15 = \mathbf{26868{,}69\text{ kN}\cdot\text{cm}} = 268{,}687\text{ kN}\cdot\text{m}$$

---

### 5.5 Passo 4 — Posições Críticas da Carga Móvel $Q_k$ e Valor Máximo Admissível

A carga permanente de cálculo vale $g_d = 1{,}40 \times 5{,}357 = \mathbf{7{,}500\text{ kN/m}}$ *(observe que $5{,}357\text{ kN/m}$ foi escolhido no enunciado justamente para que $1{,}40 \times 5{,}357 = 7{,}50\text{ kN/m}$ exato!)*.

1. **Posição Crítica 1 — Carga móvel $Q_k$ na extremidade livre do balanço ($2\text{ m}$ do apoio A ou B):**
   - Provoca o máximo momento fletor negativo sobre o apoio:
     $$|M_{sd,\text{apoio}}^-| = \frac{g_d L_{\text{bal}}^2}{2} + 1{,}40\, Q_k L_{\text{bal}} = \frac{7{,}50 \times 2^2}{2} + 1{,}40\, Q_k \times 2 = 15{,}0 + 2{,}80\, Q_k$$
   - Igualando a $M_{rd,\text{apoio}}^- = 268{,}687\text{ kN}\cdot\text{m}$:
     $$15{,}0 + 2{,}80\, Q_k \le 268{,}687 \implies Q_{k,\text{apoio}} \le \frac{268{,}687 - 15{,}0}{2{,}80} = \mathbf{90{,}602\text{ kN}}$$

2. **Posição Crítica 2 — Carga móvel $Q_k$ no centro do vão AB ($\ell = 8\text{ m}$):**
   - Provoca o máximo momento fletor positivo no meio do vão:
     - Com $\gamma_g = 1{,}40$:
       $$M_{sd,\text{vão}}^+ = g_d\left(\frac{8^2}{8} - \frac{2^2}{2}\right) + 1{,}40\, Q_k \frac{8}{4} = 7{,}50(8 - 2) + 2{,}80\, Q_k = 45{,}0 + 2{,}80\, Q_k$$
       $$45{,}0 + 2{,}80\, Q_k \le 321{,}234 \implies Q_{k,\text{vão}} \le \frac{321{,}234 - 45{,}0}{2{,}80} = \mathbf{98{,}655\text{ kN}}$$
     - Com $\gamma_g = 1{,}00$ favorável nos balanços ($g_d = 5{,}357\text{ kN/m}$):
       $$M_{sd,\text{vão}}^+ = 5{,}357 \times 6 + 2{,}80\, Q_k = 32{,}142 + 2{,}80\, Q_k \le 321{,}234 \implies Q_{k,\text{vão}} \le \mathbf{103{,}247\text{ kN}}$$

3. **Conclusão (Menor entre os limites do apoio e do vão):**
   $$Q_{k,\max} = \min(90{,}602\text{ kN};\, 98{,}655\text{ kN}) = \mathbf{90{,}602\text{ kN}}$$

---

### 5.6 Resumo Complementar — Quando a Própria Seção T Trabalha com Armadura Dupla ($M_{sd} > M_{rda} + M_{rd,lim}$)

Caso em uma questão de prova o momento positivo comprima a mesa ($b_f \times h_f$), ultrapasse $M_{rdf}$ ($y > h_f$) **e ainda** supere $M_{rda} + M_{rd,lim}$, o roteiro exato pelos blocos do formulário é:
1. Calcular $M_{rdf}$ (**Bloco `[AM]`**) e verificar $M_{sd} > M_{rdf}$ ($\therefore$ viga T verdadeira).
2. Calcular $M_{rda}$ (**Bloco `[AM]`**) e $M_{rd,lim}$ da alma $b_w$ (**Bloco `[V]`**).
3. Se $M_{sd} > M_{rda} + M_{rd,lim}$, fixar $M_{rdw} = M_{rd,lim}$ (com $\beta_x = \beta_{x,lim}$ do **Bloco `[P]`**) e obter o momento excedente pela equação do **Bloco `[AM]`**:
   $$M'_{rd} = M_{sd} - M_{rda} - M_{rd,lim}$$
4. Calcular $\beta_z = 1 - 0{,}5\zeta_c \beta_{x,lim}$, $\beta_s$ e $\beta'_s$ em $\beta_{x,lim}$ (**Bloco `[S]`**).
5. Calcular a armadura comprimida $A'_s$ pelo **Bloco `[X]`** e a armadura tracionada $A_s$ pela equação completa do **Bloco `[AM]`**:
   $$A'_s = \frac{M'_{rd}}{(d - d')\beta'_s f_{yd}} \qquad A_s = \left[\frac{M_{rda}}{\left(d - \dfrac{h_f}{2}\right)} + \frac{M'_{rd}}{(d - d')} + \frac{M_{rdw}}{\beta_z d}\right]\frac{1}{\beta_s f_{yd}}$$
6. Após escolher as barras (**Blocos `[Y]`, `[Z]`, `[AG]`**) e corrigir $d, d'$ (**Blocos `[AE]`, `[AJ]`**), verificar a linha neutra efetiva pela última equação do **Bloco `[AM]`**:
   $$\beta_x = \left(\frac{A_{s,ef}}{\eta_c \zeta_c b_w d}\right)\frac{f_{yd}}{f_{cd}}\beta_s - \left(\frac{A'_{s,ef}}{\eta_c \zeta_c b_w d}\right)\frac{f_{yd}}{f_{cd}}\beta'_s - \left[\frac{h_f(b_f - b_w)}{\zeta_c b_w d}\right] \le \beta_{x,lim}$$

### 5.7 Conclusão — O que torna o Exercício `6.4.1` de Nível Graduado?
- **Diferença para os exercícios comuns:** É o exercício mais conceitual de flexão do caderno. Em vez de dimensionar $A_s$ para um momento conhecido, ele fornece **as armaduras já instaladas no vão e nos apoios** e pede a **máxima carga móvel $Q_k$**, combinando **inversão de sinal do momento em seção T** com **armadura comprimida que não escoa ($\beta'_s < 1{,}0$)**.
- **Os 3 Pontos Especiais Cobrados:**
  1. **"Dupla personalidade" da Seção T (Vão vs. Apoio):** No meio do vão ($M^+$), a mesa superior ($b_f = 60\text{ cm}$) é comprimida e a viga trabalha com folga ($y = 3{,}21\text{ cm} \le h_f = 10\text{ cm}$). Já sobre os apoios A e B ($M^-$), a mesa superior fica **tracionada** (sendo desprezada na resistência!), e quem recebe a compressão é a **base estreita da alma ($b_w = 25\text{ cm}$)** com **armadura dupla** ($4\phi 16$ em cima na tração e $2\phi 10$ embaixo na compressão).
  2. **Caso Raro/Especial — Armadura comprimida não escoa ($\beta'_s < 1{,}0$):** Nos apoios, como há pouca armadura tracionada para uma altura útil grande ($d = 80\text{ cm}$), a linha neutra fica muito alta ($\beta_x = 0{,}0920 < 0{,}259$). Como $d'/d = 5/80 = 0{,}0625$ está muito perto de $\beta_x = 0{,}0920$, a deformação no aço comprimido fica abaixo do escoamento ($\beta'_s = 0{,}5416 < 1{,}0$). Para achar $\beta_x$, você precisa substituir a equação de $\beta'_s$ (`[S]`) dentro da equação de equilíbrio de $\beta_x$ (`[AB]`), caindo em uma **equação do 2º grau em $\beta_x$**.
  3. **Disputa entre duas posições da carga móvel $Q_k$:** Você precisa testar $Q_k$ na ponta do balanço ($Q_{k,\text{apoio}} \le 90{,}602\text{ kN}$) e $Q_k$ no meio do vão ($Q_{k,\text{vão}} \le 98{,}655\text{ kN}$), concluindo que **quem governa a ruptura da viga é o apoio negativo ($90{,}602\text{ kN}$)**.

---

## 6. Dimensionamento de Armadura Transversal — Nível Graduado (Modelos I e II)

No capítulo 7 do *Caderno de Exercícios (2021)*, a seção **7.4 Propostos, Nível Graduado** traz exatamente dois exercícios complementares: o **7.4.1** focado no **Modelo II** (treliça generalizada com variação do ângulo $\theta$ da biela comprimida) e o **7.4.2** focado no **Modelo I** ($\theta = 45^\circ$, viga de transição com redução de carga concentrada próxima ao apoio). Apresentamos abaixo a resolução completa de **ambos**.

---

### 6A. Exercício 7.4.1 — Menor Valor Possível de $\theta$ (Modelo II, p. 165–166)

> **Enunciado Oficial (7.4.1 — p. 165–166):**
> Determinar, para a viga abaixo representada:
> **a.** o menor valor possível para o ângulo $\theta$ (múltiplo de $5^\circ$), de tal forma que a viga possa resistir os esforços devidos à força cortante;
> **b.** a armadura necessária ($\text{cm}^2/\text{m}$) nos trechos I, II e III, considerando o valor de $\theta$ estabelecido no item a.
>
> **Dados e Considerações:**
> - Concreto: C20 ($f_{ck} = 20\text{ MPa}$); Aço: CA-50 ($f_{yk} = 500\text{ MPa}$).
> - Seção retangular: $b_w = 15\text{ cm}$, $h = 80\text{ cm}$, altura útil $d = 0{,}90\,h = 72\text{ cm}$.
> - Viga biapoiada nos pilares A e B (largura dos pilares $= 20\text{ cm}$, vão de cálculo entre eixos $L = 2 + 6 + 2 = 10\text{ m}$).
> - Carregamento permanente $g_k = 85\text{ kN/m}$ atuando no trecho central de $6\text{ m}$ ($2\text{ m} \le x \le 8\text{ m}$); peso próprio desconsiderado.
> - Trechos para armadura transversal: **Trecho I** ($3{,}5\text{ m}$ à esquerda), **Trecho II** ($3{,}0\text{ m}$ central) e **Trecho III** ($3{,}5\text{ m}$ à direita).
> - Modelo II ($30^\circ \le \theta \le 45^\circ$), estribos verticais ($\alpha = 90^\circ$) de 2 ramos, ELU combinações normais.

#### Passo 1 — Parâmetros dos materiais e taxa mínima de armadura transversal
1. **Resistências de cálculo do concreto e do aço transversal:** `[BC]`, `[BD]`, `[AW]`, `[AX]`, `[BG]`
   $$f_{cd} = \frac{f_{ck}}{\gamma_c} = \frac{2{,}0}{1{,}4} = \mathbf{1{,}4286\text{ kN/cm}^2}$$
   $$f_{ctk,inf} = 0{,}21\sqrt[3]{f_{ck}^2} = 0{,}21\sqrt[3]{20^2} = 1{,}5473\text{ MPa} \implies f_{ctd} = \frac{1{,}5473}{1{,}4} = 1{,}1052\text{ MPa} = \mathbf{0{,}1105\text{ kN/cm}^2}$$
   $$f_{ywd} = 435\text{ MPa} = \mathbf{43{,}478\text{ kN/cm}^2}$$
2. **Relação mínima de armadura transversal:** `[AY]`
   $$\left(\frac{A_{sw}}{s}\right)_{min} = 0{,}06\,b_w\frac{\sqrt[3]{f_{ck}^2}}{435} = 0{,}06 \times 15 \times \frac{7{,}3681}{435} = \mathbf{0{,}01524\text{ cm}^2/\text{cm}} = \mathbf{1{,}524\text{ cm}^2/\text{m}}$$

#### Passo 2 — Esforço cortante solicitante de cálculo $V_{sd}(x)$ e análise de reduções
1. **Combinação última normal:** `[A]`, `[B]`
   - Adotando $\gamma_g = 1{,}40$ (Tabela Geral `[B]`): $g_d = 1{,}40 \times 85 = \mathbf{119{,}00\text{ kN/m}}$ *(Obs.: com $\gamma_g = 1{,}35$ de Edificação Tipo 1, $g_d = 114{,}75\text{ kN/m}$; apresentamos ambos os resultados)*.
2. **Reações de apoio e diagrama de cortante:**
   - Pela simetria do carregamento centrado de $6\text{ m}$ de extensão:
     $$R_{A,d} = R_{B,d} = \frac{g_d \times 6{,}0}{2} = 3{,}0\,g_d = 3{,}0 \times 119{,}00 = \mathbf{357{,}00\text{ kN}} \quad (\text{ou } 344{,}25\text{ kN c/ }\gamma_g = 1{,}35)$$
   - **Pegadinha clássica de redução no apoio `[BB]`:** entre o eixo do apoio A ($x=0$) e $x=2{,}0\text{ m}$, **não há carga distribuída aplicada** ($w=0$). Portanto, na face do pilar ($x_{face} = 0{,}10\text{ m}$) e na seção a $d/2 = 0{,}36\text{ m}$ da face ($x = 0{,}46\text{ m} < 2{,}0\text{ m}$), o esforço cortante permanece **constante e igual a $R_{A,d}$**!
   - Cortantes máximos por trecho:
     - **Trecho I ($0 \le x \le 3{,}5\text{ m}$) e Trecho III ($6{,}5\text{ m} \le x \le 10{,}0\text{ m}$):**
       $$V_{sd,\text{I}} = |V_{sd,\text{III}}| = R_{A,d} = \mathbf{357{,}00\text{ kN}} \quad (\text{ou } 344{,}25\text{ kN})$$
     - **Trecho II ($3{,}5\text{ m} \le x \le 6{,}5\text{ m}$):** o máximo ocorre nas extremidades do trecho ($x = 3{,}5\text{ m}$ e $x = 6{,}5\text{ m}$):
       $$V_{sd,\text{II}} = 357{,}00 - 119{,}00 \times (3{,}5 - 2{,}0) = \mathbf{178{,}50\text{ kN}} \quad (\text{ou } 172{,}125\text{ kN})$$

#### Passo 3 — Item (a): Determinação do menor ângulo $\theta$ (múltiplo de $5^\circ$) no Modelo II
Para estribos verticais ($\alpha = 90^\circ \implies \cotg\alpha = 0$), a resistência das diagonais comprimidas de concreto é dada pela expressão geral do bloco `[AU]`:
$$V_{rdc}(\theta) = 0{,}536\,b_w d\,\cotg(\theta)\operatorname{sen}^2(\theta)\left(1 - \frac{f_{ck}}{250}\right)f_{cd}$$
Substituindo $b_w = 15\text{ cm}$, $d = 72\text{ cm}$, $f_{ck} = 20\text{ MPa}$ e $f_{cd} = 1{,}4286\text{ kN/cm}^2$:
$$V_{rdc}(\theta) = 0{,}536 \times 15 \times 72 \times \left(1 - \frac{20}{250}\right) \times 1{,}4286 \times \cotg(\theta)\operatorname{sen}^2(\theta) = 760{,}814\,\cotg(\theta)\operatorname{sen}^2(\theta)$$

Testando os múltiplos de $5^\circ$ no intervalo normativo do Modelo II ($30^\circ \le \theta \le 45^\circ$) contra $V_{sd,\max} = 357{,}00\text{ kN}$ `[AR]`:
- Para $\theta = 30^\circ$: $V_{rdc}(30^\circ) = 0{,}232\,b_w d(1 - f_{ck}/250)f_{cd} = \mathbf{329{,}44\text{ kN}} < 357{,}00\text{ kN}$ (**Não atende!** Também não atende para $344{,}25\text{ kN}$).
- Para $\mathbf{\theta = 35^\circ}$: $\cotg(35^\circ)\operatorname{sen}^2(35^\circ) = 1{,}42815 \times 0{,}32899 = 0{,}46985 \implies V_{rdc}(35^\circ) = \mathbf{357{,}47\text{ kN}} \ge 357{,}00\text{ kN}$ (**Atende!**).
- Logo, o menor ângulo múltiplo de $5^\circ$ é $\mathbf{\theta = 35^\circ}$.

#### Passo 4 — Item (b): Armadura transversal necessária ($\text{cm}^2/\text{m}$) nos Trechos I, II e III ($\theta = 35^\circ$)
1. **Parcela de referência $V_{c0}$ e rigidez dos estribos para $\theta = 35^\circ, \alpha = 90^\circ$:** `[AS]`, `[AV]`
   $$V_{c0} = 0{,}6\,f_{ctd}\,b_w d = 0{,}6 \times 0{,}11052 \times 15 \times 72 = \mathbf{71{,}618\text{ kN}}$$
   $$V_{sw}(\theta=35^\circ) = \left(\frac{A_{sw}}{s}\right)0{,}9\,d\,f_{ywd}\cotg(35^\circ) = \left(\frac{A_{sw}}{s}\right) \times 0{,}9 \times 72 \times 43{,}478 \times 1{,}42815 = \mathbf{4023{,}64\left(\frac{A_{sw}}{s}\right)}$$
2. **Dimensionamento nos Trechos I e III ($V_{sd,\text{I}} = V_{sd,\text{III}} = 357{,}00\text{ kN}$):** `[AS]`, `[AT]`, `[AV]`
   $$V_{c,II} = V_{c0}\left(\frac{V_{rdc} - V_{sd}}{V_{rdc} - V_{c0}}\right) = 71{,}618\left(\frac{357{,}466 - 357{,}000}{357{,}466 - 71{,}618}\right) = \mathbf{0{,}117\text{ kN}} \le 71{,}618\text{ kN}$$
   $$V_{sw,\text{I}} = V_{sd,\text{I}} - V_{c,II} = 357{,}000 - 0{,}117 = \mathbf{356{,}883\text{ kN}}$$
   $$\left(\frac{A_{sw}}{s}\right)_{\text{I, III}} = \frac{356{,}883}{4023{,}64} = 0{,}08870\text{ cm}^2/\text{cm} = \mathbf{8{,}870\text{ cm}^2/\text{m}} \ge 1{,}524\text{ cm}^2/\text{m}$$
   *(Nota: para $\gamma_g = 1{,}35 \implies V_{sd} = 344{,}25\text{ kN}, V_{c,II} = 3{,}311\text{ kN}, V_{sw} = 340{,}939\text{ kN} \implies \mathbf{8{,}473\text{ cm}^2/\text{m}}$).*
3. **Dimensionamento no Trecho II ($V_{sd,\text{II}} = 178{,}50\text{ kN}$):** `[AS]`, `[AT]`, `[AV]`
   $$V_{c,II} = 71{,}618\left(\frac{357{,}466 - 178{,}500}{357{,}466 - 71{,}618}\right) = \mathbf{44{,}839\text{ kN}} \le 71{,}618\text{ kN}$$
   $$V_{sw,\text{II}} = 178{,}500 - 44{,}839 = \mathbf{133{,}661\text{ kN}}$$
   $$\left(\frac{A_{sw}}{s}\right)_{\text{II}} = \frac{133{,}661}{4023{,}64} = 0{,}03322\text{ cm}^2/\text{cm} = \mathbf{3{,}322\text{ cm}^2/\text{m}} \ge 1{,}524\text{ cm}^2/\text{m}$$
   *(Nota: para $\gamma_g = 1{,}35 \implies V_{sd} = 172{,}125\text{ kN}, V_{c,II} = 46{,}436\text{ kN}, V_{sw} = 125{,}689\text{ kN} \implies \mathbf{3{,}124\text{ cm}^2/\text{m}}$).*

#### Conclusão — O que torna o Exercício `7.4.1` (Modelo II) de Nível Graduado?
- **Diferença para os exercícios comuns:** Nos exercícios básicos do Modelo II, o ângulo $\theta$ já vem fixado ($\theta = 30^\circ$) e basta substituir na fórmula pronta. Aqui, a alma é propositalmente muito estreita ($b_w = 15\text{ cm}$) e o concreto é C20, fazendo com que **$\theta = 30^\circ$ rompa por esmagamento da biela comprimida** ($V_{rdc}(30^\circ) = 329{,}44\text{ kN} < 357{,}00\text{ kN}$).
- **Os 3 Pontos Especiais Cobrados:**
  1. **Uso da fórmula trigonométrica geral de $V_{rdc}(\theta)$ (`[AU]`):** Como $\theta \ne 30^\circ$ e $\theta \ne 45^\circ$, você não pode usar os coeficientes prontos ($0{,}232$ ou $0{,}268$); precisa usar a expressão geral $V_{rdc}(\theta) = 0{,}536\,b_w d\cotg(\theta)\operatorname{sen}^2(\theta)(1 - f_{ck}/250)f_{cd}$ (`[AU]`) e testar os múltiplos de $5^\circ$ até encontrar $\mathbf{\theta = 35^\circ}$ ($V_{rdc}(35^\circ) = 357{,}47\text{ kN}$).
  2. **Pegadinha da redução $d/2$ junto ao apoio (`[BB]`):** Como a carga distribuída só começa em $x = 2{,}0\text{ m}$, entre o apoio ($x=0$) e $x=2{,}0\text{ m}$ **não há carga distribuída ($w=0$)**. Logo, a seção a $d/2 = 0{,}36\text{ m}$ da face do pilar tem **exatamente o mesmo cortante da reação de apoio ($357{,}00\text{ kN}$)** — quem desconta $g_d\cdot(d/2)$ no piloto automático erra toda a questão!
  3. **Quase anulação de $V_{c,II}$ no trecho crítico:** Como em $\theta = 35^\circ$ tem-se $V_{sd} = 357{,}00\text{ kN}$ quase empatado com $V_{rdc} = 357{,}47\text{ kN}$, a contribuição dos mecanismos complementares do concreto cai praticamente a zero ($V_{c,II} = 0{,}117\text{ kN}$), obrigando os estribos a absorverem quase $100\%$ do cortante nos Trechos I e III, enquanto no Trecho II ($V_{sd} = 178{,}50\text{ kN}$) $V_{c,II}$ sobe para $44{,}84\text{ kN}$.

---

### 6B. Exercício 7.4.2 — Viga de Transição (Modelo I, p. 166–167)

> **Enunciado Oficial (7.4.2 — p. 166–167):**
> A viga ABCD da estrutura abaixo representada receberá a carga de $n$ pavimentos. Cada pavimento transmite uma carga $P_{d,i} = 400\text{ kN}$ (valor de cálculo) a cada uma das colunas verticais. O carregamento total que chega aos pontos B e C da viga é a soma das cargas de todos os pavimentos. Pede-se:
> **a.** o número máximo de pavimentos ($n$) que a viga ABCD é capaz de suportar;
> **b.** a armadura transversal ($\text{cm}^2/\text{m}$) no trecho AB da referida viga.
>
> **Dados e Considerações:**
> - Concreto: C30 ($f_{ck} = 30\text{ MPa}$); Aço: CA-50 ($f_{yk} = 500\text{ MPa}$).
> - Seção T: mesa $b_f = 120\text{ cm}$, $h_f = 10\text{ cm}$; alma $b_w = 25\text{ cm}$, altura da nervura sob a mesa $= 110\text{ cm} \implies h = 120\text{ cm}$ e $d = h - 10\text{ cm} = 110\text{ cm}$ *(verificamos também a variante $h = 110\text{ cm} \implies d = 100\text{ cm}$)*.
> - Pilares de apoio em A e D com $40\text{ cm}$ de largura ($20\text{ cm}$ entre o eixo e a face interna).
> - Cotas longitudinais: face interna de A até B $= 80\text{ cm}$ ($\implies x_B = 20 + 80 = 100\text{ cm} = 1{,}0\text{ m}$ do eixo A); entre B e C $= 500\text{ cm} = 5{,}0\text{ m}$ ($\implies x_C = 6{,}0\text{ m}$ do eixo A); entre C e a face interna de D $= 180\text{ cm}$ ($\implies L = 6{,}0 + 1{,}80 + 0{,}20 = 8{,}0\text{ m}$ entre eixos A e D).
> - Modelo I ($\theta = 45^\circ$), estribos verticais ($\alpha = 90^\circ$), peso próprio desprezado.

#### Passo 1 — Estática da viga de transição em função do número de pavimentos $n$
Cada coluna descarrega em B ($x_B = 1{,}0\text{ m}$) e em C ($x_C = 6{,}0\text{ m}$) a carga concentrada total de cálculo $P_{d,\text{total}} = n \cdot P_{d,i} = 400\,n\text{ (kN)}$.
Pelo equilíbrio de momentos em relação ao apoio D ($L = 8{,}0\text{ m}$):
$$R_{A,d} \times 8{,}0 = P_{d,\text{total}}(8{,}0 - 1{,}0) + P_{d,\text{total}}(8{,}0 - 6{,}0) = 9{,}0\,P_{d,\text{total}}$$
$$R_{A,d} = \frac{9}{8}\,P_{d,\text{total}} = 1{,}125 \times 400\,n = \mathbf{450\,n\text{ (kN)}} \qquad R_{D,d} = \frac{7}{8}\,P_{d,\text{total}} = \mathbf{350\,n\text{ (kN)}}$$
- Esforço cortante solicitante por trecho:
  - **Trecho AB ($0 \le x < 1{,}0\text{ m}$):** $V_{sd,\text{AB}} = +450\,n\text{ (kN)}$ (**trecho crítico da viga!**)
  - **Trecho BC ($1{,}0\text{ m} < x < 6{,}0\text{ m}$):** $V_{sd,\text{BC}} = 450\,n - 400\,n = +50\,n\text{ (kN)}$
  - **Trecho CD ($6{,}0\text{ m} < x \le 8{,}0\text{ m}$):** $V_{sd,\text{CD}} = -350\,n\text{ (kN)}$

#### Passo 2 — Item (a): Número máximo de pavimentos $n$ (verificação da biela comprimida $V_{rdc,I}$)
1. **Resistências de cálculo (Concreto C30):** `[BC]`, `[BD]`, `[AW]`, `[AX]`
   $$f_{cd} = \frac{3{,}0}{1{,}4} = \mathbf{2{,}1429\text{ kN/cm}^2} \qquad f_{ctd} = \frac{0{,}21\sqrt[3]{30^2}}{1{,}4} = 1{,}4484\text{ MPa} = \mathbf{0{,}14484\text{ kN/cm}^2}$$
2. **Resistência da diagonal comprimida no Modelo I ($b_w = 25\text{ cm}, d = 110\text{ cm}$):** `[AU]`
   $$V_{rdc,I} = 0{,}268\,b_w d\left(1 - \frac{f_{ck}}{250}\right)f_{cd} = 0{,}268 \times 25 \times 110 \times \left(1 - \frac{30}{250}\right) \times 2{,}1429 = \mathbf{1389{,}77\text{ kN}}$$
3. **Condição limite de integridade do concreto na face do apoio A (sem redução!):** `[AR]`, `[BB]`
   $$V_{sd,\text{AB}} \le V_{rdc,I} \implies 450\,n \le 1389{,}77 \implies n \le 3{,}088 \implies \mathbf{n_{\max} = 3\text{ pavimentos}}$$
   Para $n = 3$ pavimentos, $P_{d,\text{total}} = 1200\text{ kN}$ e o cortante no trecho AB é $V_{sd,\text{AB}} = 3 \times 450 = \mathbf{1350{,}00\text{ kN}} \le 1389{,}77\text{ kN}$ (**OK!**).
   *(Nota: caso se interprete a cota $110\text{ cm}$ como altura total $h = 110\text{ cm} \implies d = 100\text{ cm}$, tem-se $V_{rdc,I} = 1263{,}43\text{ kN} \implies n \le 2{,}808 \implies \mathbf{n_{\max} = 2\text{ pavimentos}}$, com $V_{sd,\text{AB}} = 900{,}00\text{ kN}$).*

#### Passo 3 — Item (b): Armadura transversal no Trecho AB com redução de carga concentrada próxima ao apoio
1. **Redução do esforço cortante para cálculo de $A_{sw}/s$:** `[BB]`
   A carga concentrada em B está aplicada a uma distância $a \le 2d = 220\text{ cm}$ do apoio A, permitindo reduzir o cortante pela razão $\dfrac{a}{2d}$:
   - **Critério 1 (cota $a = 80\text{ cm}$ até a face interna do pilar A):**
     $$V_{sd,\text{red}} = V_{sd,\text{AB}}\frac{a}{2d} = 1350{,}00 \times \frac{80}{2 \times 110} = 1350{,}00 \times 0{,}36364 = \mathbf{490{,}909\text{ kN}}$$
   - **Critério 2 (cota $a = 100\text{ cm}$ até o eixo do apoio A, conforme Ex. Resolvido 7.1.7):**
     $$V_{sd,\text{red}} = 1350{,}00 \times \frac{100}{2 \times 110} = 1350{,}00 \times 0{,}45455 = \mathbf{613{,}636\text{ kN}}$$
2. **Parcela do concreto $V_{c,I}$ e armadura mínima $(A_{sw}/s)_{min}$:** `[AS]`, `[AY]`
   $$V_{c,I} = 0{,}6\,f_{ctd}\,b_w d = 0{,}6 \times 0{,}14484 \times 25 \times 110 = \mathbf{238{,}98\text{ kN}}$$
   $$\left(\frac{A_{sw}}{s}\right)_{min} = 0{,}06 \times 25 \times \frac{\sqrt[3]{30^2}}{435} = 0{,}03329\text{ cm}^2/\text{cm} = \mathbf{3{,}329\text{ cm}^2/\text{m}}$$
3. **Relação de armadura transversal $(A_{sw}/s)$ no Trecho AB:** `[AT]`, `[AV]`
   $$V_{sw,I} = V_{sd,\text{red}} - V_{c,I} = 0{,}9\left(\frac{A_{sw}}{s}\right)d\,f_{ywd} = 0{,}9 \times 110 \times 43{,}478\left(\frac{A_{sw}}{s}\right) = 4304{,}35\left(\frac{A_{sw}}{s}\right)$$
   - **Com $a = 80\text{ cm}$ (face):** $V_{sw,I} = 490{,}909 - 238{,}98 = 251{,}93\text{ kN} \implies \left(\dfrac{A_{sw}}{s}\right) = \mathbf{5{,}853\text{ cm}^2/\text{m}} \ge 3{,}329\text{ cm}^2/\text{m}$.
   - **Com $a = 100\text{ cm}$ (eixo):** $V_{sw,I} = 613{,}636 - 238{,}98 = 374{,}66\text{ kN} \implies \left(\dfrac{A_{sw}}{s}\right) = \mathbf{8{,}705\text{ cm}^2/\text{m}} \ge 3{,}329\text{ cm}^2/\text{m}$.
   *(Para $h = 110\text{ cm} \implies d = 100\text{ cm}, n = 2$: $V_{c,I} = 217{,}24\text{ kN}$, resultando em $\mathbf{3{,}648\text{ cm}^2/\text{m}}$ para $a=80\text{ cm}$ ou $\mathbf{5{,}948\text{ cm}^2/\text{m}}$ para $a=100\text{ cm}$).*

#### Conclusão — O que torna o Exercício `7.4.2` (Modelo I) de Nível Graduado?
- **Diferença para os exercícios comuns:** Modela uma **viga de transição real** (que recebe pilares que nascem sobre ela nos pontos B e C), parametrizando o esforço pelo número de pavimentos $n$ e cobrando a **regra especial de redução de carga concentrada próxima ao apoio (`[BB]`)**.
- **Os 3 Pontos Especiais Cobrados:**
  1. **Problema inverso de capacidade máxima ($n_{\max}$) governado pela biela (`[AR]`, `[AU]`):** Como a carga em B está mais próxima do apoio A ($1{,}0\text{ m}$) do que C está de D ($2{,}0\text{ m}$), a reação em A é maior ($R_{A,d} = 450\,n$ contra $R_{D,d} = 350\,n$). O limite de pavimentos que a viga suporta sem esmagar o concreto da alma é dado por $450\,n \le V_{rdc,I} = 1389{,}77\text{ kN} \implies n_{\max} = 3\text{ pavimentos}$ (arredondado sempre para baixo, pois $n$ é inteiro!).
  2. **Distinção crucial entre verificar $V_{rdc}$ (sem redução!) e calcular $A_{sw}/s$ (com redução $a/2d$!):** Esta é a regra mais importante do Bloco `[BB]`: na verificação do esmagamento da biela comprimida ($V_{sd} \le V_{rdc}$, item a), usa-se o **cortante cheio de $1350\text{ kN}$**. Já para dimensionar os estribos ($A_{sw}/s$, item b), como a carga concentrada em B está a uma distância $a \le 2d = 220\text{ cm}$ do apoio A, parte da força escoa diretamente por puntal para o apoio, permitindo reduzir o cortante para $V_{sd,\text{red}} = V_{sd}\cdot\frac{a}{2d}$.
  3. **Seção T submetida a cisalhamento:** Embora a figura mostre uma seção T com mesa larga ($b_f = 120\text{ cm}$), nas fórmulas de cisalhamento ($V_{rdc}$, $V_c$ e $(A_{sw}/s)_{min}$) **entra exclusivamente a largura da alma $b_w = 25\text{ cm}$**!

---

## 7. Exercício Completo Integrado — Combinações + Flexão Longitudinal + Cisalhamento (Baseado no Ex. 1.3.3, p. 28)

Para integrar todas as etapas da disciplina de **Concreto I** (Formulários 1, 2 e 3), tomamos a viga de depósito do **Exercício 1.3.3** (*Caderno de Exercícios*, p. 28 — cujo enunciado original inicia com *"Deseja-se dimensionar a viga de concreto armado de um depósito abaixo indicada..."*) e realizamos o **projeto completo de ponta a ponta**:
1. **Etapa A — Combinações Últimas Normais (ELU) e Envoltórias de $M_{sd}$ e $V_{sd}$** (Formulário 1: `[A]`, `[B]`, `[F]`, `[AQ]`/`[BN]`).
2. **Etapa B — Dimensionamento e Detalhamento da Armadura Longitudinal de Flexão** no apoio B (armadura simples negativa) e no meio do vão C (armadura dupla positiva) (Formulário 2: `[P]` a `[AL]`).
3. **Etapa C — Dimensionamento e Detalhamento da Armadura Transversal de Cisalhamento** nos trechos I, II e III pelos **Modelos I e II** (Formulário 3: `[AR]` a `[BI]`).

> **Enunciado Completo Integrado (Baseado no Ex. 1.3.3 — p. 28):**
> Deseja-se projetar integralmente a viga de concreto armado de um depósito representada na figura (balanço esquerdo AB de $2{,}0\text{ m}$ e vão entre apoios BD de $8{,}0\text{ m}$, com ponto C no meio do vão BD). A viga está submetida à carga permanente uniformemente distribuída $g_k = 20\text{ kN/m}$ em toda a sua extensão e a duas cargas acidentais concentradas independentes: $Q_{k1} = 40\text{ kN}$ na extremidade livre A do balanço e $Q_{k2} = 30\text{ kN}$ no meio do vão C.
>
> **Dados de Projeto:**
> - Concreto **C30** ($f_{ck} = 30\text{ MPa}$); Aço **CA-50** ($f_{yk} = 500\text{ MPa}$, $f_{ywd} = 435\text{ MPa}$).
> - Seção transversal retangular: $b_w = 20\text{ cm}$, $h = 50\text{ cm}$ ($d_{\text{est}} = 45\text{ cm}$, $d'_{\text{est}} = 4\text{ cm}$).
> - Pilares de apoio em B e D com largura $\ell_{\text{pil}} = 20\text{ cm}$; cobrimento nominal $c_{nom} = 2{,}5\text{ cm}$; brita 1 ($d_{\max} = 19\text{ mm}$).
> - Edificação Tipo 1 (depósito: $\gamma_g = 1{,}35$ desfavorável / $1{,}00$ favorável; $\gamma_q = 1{,}50$; $\psi_0 = 0{,}80$).

### Etapa A — Ações, Combinações ELU e Envoltórias de Solicitações ($M_{sd}$ e $V_{sd}$)

1. **Esforços característicos por ação isolada (usando `VB1-w` espelhada `[AQ]`/`[BN]` e superposição):**
   - **Carga permanente $g_k = 20\text{ kN/m}$ (em todos os $10\text{ m}$):**
     - Reações: $R_{B,g} = 125{,}0\text{ kN}$ e $R_{D,g} = 75{,}0\text{ kN}$.
     - Cortantes: $V_g(B_{\text{esq}}) = -40{,}0\text{ kN}$; $V_g(B_{\text{dir}}) = +85{,}0\text{ kN}$; $V_g(C) = +5{,}0\text{ kN}$; $V_g(D_{\text{esq}}) = -75{,}0\text{ kN}$.
     - Momentos: $M_g(B) = -\dfrac{20 \times 2^2}{2} = \mathbf{-40{,}0\text{ kN}\cdot\text{m}}$; $M_g(C) = -40 + 85(4) - \dfrac{20(4^2)}{2} = \mathbf{+140{,}0\text{ kN}\cdot\text{m}}$.
   - **Carga acidental $Q_{k1} = 40\text{ kN}$ (na ponta A do balanço):**
     - Reações: $R_{B,Q1} = +50{,}0\text{ kN}$ e $R_{D,Q1} = -10{,}0\text{ kN}$.
     - Cortantes: $V_{Q1}(\text{AB}) = -40{,}0\text{ kN}$; $V_{Q1}(\text{BD}) = +10{,}0\text{ kN}$ (constante no vão BD).
     - Momentos: $M_{Q1}(B) = -40 \times 2 = \mathbf{-80{,}0\text{ kN}\cdot\text{m}}$; $M_{Q1}(C) = -80 + 10(4) = \mathbf{-40{,}0\text{ kN}\cdot\text{m}}$ (alivia o momento positivo em C!).
   - **Carga acidental $Q_{k2} = 30\text{ kN}$ (no meio do vão C):**
     - Reações: $R_{B,Q2} = +15{,}0\text{ kN}$ e $R_{D,Q2} = +15{,}0\text{ kN}$.
     - Cortantes: $V_{Q2}(\text{AB}) = 0$; $V_{Q2}(\text{BC}) = +15{,}0\text{ kN}$; $V_{Q2}(\text{CD}) = -15{,}0\text{ kN}$.
     - Momentos: $M_{Q2}(B) = \mathbf{0}$; $M_{Q2}(C) = \dfrac{30 \times 8}{4} = \mathbf{+60{,}0\text{ kN}\cdot\text{m}}$.

2. **Combinações Últimas Normais Críticas (ELU):** `[A]`, `[B]`, `[C]`, `[E]`, `[F]`
   $$F_{d,nor} := \gamma_g G_k \uplus \gamma_q F_{q1k} \uplus \gamma_q \psi_0 F_{q2k}$$
   - **Momento negativo máximo no Apoio B ($M_{sd,B}^-$):** $g_k$ desfavorável ($\gamma_g = 1{,}35$) e $Q_{k1}$ principal ($\gamma_q = 1{,}50$):
     $$M_{sd,B}^- = 1{,}35 \times (-40{,}0) + 1{,}50 \times (-80{,}0) = -54{,}0 - 120{,}0 = \mathbf{-174{,}00\text{ kN}\cdot\text{m}}$$
   - **Momento positivo máximo no Meio do Vão C ($M_{sd,C}^+$):** $g_k$ desfavorável ($\gamma_g = 1{,}35$), $Q_{k2}$ principal ($\gamma_q = 1{,}50$) e $Q_{k1} = 0$ (pois $Q_{k1}$ é favorável ao momento positivo em C):
     $$M_{sd,C}^+ = 1{,}35 \times (+140{,}0) + 1{,}50 \times (+60{,}0) = +189{,}0 + 90{,}0 = \mathbf{+279{,}00\text{ kN}\cdot\text{m}}$$
   - **Verificação de inversão de momento em C ($M_{sd,C,\min}$):** $g_k$ favorável ($\gamma_g = 1{,}00$), $Q_{k1}$ atuando ($\gamma_q = 1{,}50$) e $Q_{k2} = 0$:
     $$M_{sd,C,\min} = 1{,}00 \times (+140{,}0) + 1{,}50 \times (-40{,}0) = \mathbf{+80{,}00\text{ kN}\cdot\text{m}} > 0 \quad (\text{não há inversão!})$$
   - **Envoltória de Esforços Cortantes Solicitantes ($V_{sd}$ nos 3 trechos):**
     - **Trecho I (Balanço AB):** $V_{sd,\text{I}}(B_{\text{esq}}) = 1{,}35(-40) + 1{,}50(-40) = \mathbf{-114{,}00\text{ kN}}$.
     - **Trecho II (Vão BC):** no apoio $B_{\text{dir}}$, $V_g, V_{Q1}, V_{Q2} > 0$:
       - Com $\psi_0 = 0{,}80$ ($Q_{k2}$ principal): $V_{sd,\text{II}}(B_{\text{dir}}) = 1{,}35(85) + 1{,}50(15 + 0{,}80 \times 10) = \mathbf{+149{,}25\text{ kN}}$.
       - Com atuação simultânea plena ($\psi_0 = 1{,}0$): $V_{sd,\text{II}}(B_{\text{dir}}) = 1{,}35(85) + 1{,}50(15 + 10) = \mathbf{+152{,}25\text{ kN}}$.
     - **Trecho III (Vão CD):** no apoio $D_{\text{esq}}$, $V_g = -75\text{ kN}$, $V_{Q2} = -15\text{ kN}$ e $V_{Q1} = +10\text{ kN}$ (favorável $\implies Q_{k1}=0$):
       $$V_{sd,\text{III}}(D_{\text{esq}}) = 1{,}35(-75) + 1{,}50(-15) = -101{,}25 - 22{,}50 = \mathbf{-123{,}75\text{ kN}}$$

---

### Etapa B — Dimensionamento da Armadura Longitudinal de Flexão (Seções B e C)

1. **Parâmetros da seção e momento limite de armadura simples ($d_{\text{est}} = 45\text{ cm}, d'_{\text{est}} = 4\text{ cm}$):** `[P]`, `[Q]`, `[R]`, `[T]`, `[U]`, `[V]`, `[AA]`, `[AH]`
   - $f_{cd} = 2{,}1429\text{ kN/cm}^2$, $f_{yd} = 43{,}478\text{ kN/cm}^2$, $\eta_c = 0{,}85$, $\zeta_c = 0{,}80$, $\beta_{x,lim} = 0{,}45$.
   - Momento limite para armadura simples:
     $$M_{rd,lim} = 0{,}25092\,b_w d^2 f_{cd} = 0{,}25092 \times 20 \times 45^2 \times 2{,}1429 = \mathbf{21776{,}27\text{ kN}\cdot\text{cm}} = \mathbf{217{,}76\text{ kN}\cdot\text{m}}$$
   - Armadura mínima de tração: $W_0 = \dfrac{20 \times 50^2}{6} = 8333{,}33\text{ cm}^3$, $f_{ctk,sup} = 0{,}39\sqrt[3]{30^2} = 3{,}766\text{ MPa} \implies M_{sd,\min} = 0{,}8\,W_0 f_{ctk,sup} = 2510{,}60\text{ kN}\cdot\text{cm} \implies A_{s,\min} = \max(0{,}15\%\,b_w h\,;\,1{,}431\text{ cm}^2) = \mathbf{1{,}500\text{ cm}^2}$.

2. **Seção do Apoio B — Flexão Negativa ($|M_{sd,B}^-| = 174{,}00\text{ kN}\cdot\text{m} \le M_{rd,lim} \implies$ Armadura Simples):** `[S]`, `[X]`, `[Y]`, `[Z]`, `[AB]`, `[AE]`–`[AJ]`
   $$\beta_x = \frac{1 - \sqrt{1 - \dfrac{2 \times 17400}{0{,}85 \times 20 \times 45^2 \times 2{,}1429}}}{0{,}80} = \mathbf{0{,}3415} \le 0{,}45 \implies \beta_z = 1 - 0{,}4(0{,}3415) = \mathbf{0{,}8634}$$
   $$A_{s,B,\text{calc}} = \frac{17400}{0{,}8634 \times 45 \times 43{,}478} = \mathbf{10{,}300\text{ cm}^2} \ge 1{,}500\text{ cm}^2$$
   - **Detalhamento e verificação real:** Adotando $\mathbf{6\phi 16\text{ mm}}$ ($A_{s,ef,B} = 12{,}064\text{ cm}^2$) dispostas em **2 camadas de 3 barras**:
     - Espaçamentos: $a_h = \dfrac{20 - 2(2{,}5 + 0{,}63) - 3(1{,}6)}{2} = \mathbf{4{,}47\text{ cm}} \ge 2{,}28\text{ cm}$ (`[AF]`); $a_v = \mathbf{2{,}00\text{ cm}}$.
     - Posição do CG e altura útil real: $y_s = 0{,}5(1{,}6 + 2{,}0) = 1{,}80\text{ cm} \implies d_{\text{real},B} = 50 - 2{,}5 - 0{,}63 - 0{,}80 - 1{,}80 = \mathbf{44{,}27\text{ cm}}$ (`[AE]`, `[AJ]`).
     - Linha neutra e momento resistente efetivos (`[AB]`):
       $$\beta_{x,ef,B} = \frac{12{,}064 \times 43{,}478}{0{,}85 \times 0{,}80 \times 20 \times 44{,}27 \times 2{,}1429} = \mathbf{0{,}4065} \le 0{,}45 \quad (\text{Domínio 3})$$
       $$M_{rd,ef,B} = 12{,}064 \times 44{,}27 \times \left[1 - 0{,}4(0{,}4065)\right] \times 43{,}478 = \mathbf{194{,}44\text{ kN}\cdot\text{m}} \ge 174{,}00\text{ kN}\cdot\text{m} \quad (\text{OK!})$$

3. **Seção do Meio do Vão C — Flexão Positiva ($M_{sd,C}^+ = 279{,}00\text{ kN}\cdot\text{m} > M_{rd,lim} \implies$ Armadura Dupla):** `[P]`, `[S]`, `[V]`, `[X]`, `[AB]`, `[AE]`–`[AJ]`
   - Fixando $\beta_x = \beta_{x,lim} = 0{,}45$ ($\beta_z = 0{,}82$, $\beta_s = 1{,}0$):
     $$M_{rdw} = M_{rd,lim} = \mathbf{21776{,}27\text{ kN}\cdot\text{cm}} \qquad M'_{rd} = 27900 - 21776{,}27 = \mathbf{6123{,}73\text{ kN}\cdot\text{cm}}$$
   - Como $d'/d = 4/45 = 0{,}0889$, a deformação na armadura comprimida é $\varepsilon'_s = 3{,}5\left(\dfrac{0{,}45 - 0{,}0889}{0{,}45}\right) = 2{,}809\text{‰} \ge 2{,}07\text{‰} \implies \beta'_s = 1{,}0$:
     $$A'_{s,C,\text{calc}} = \frac{6123{,}73}{(45 - 4{,}0) \times 1{,}0 \times 43{,}478} = \mathbf{3{,}435\text{ cm}^2}$$
     $$A_{s,C,\text{calc}} = \left[\frac{21776{,}27}{0{,}82 \times 45} + \frac{6123{,}73}{45 - 4{,}0}\right]\frac{1}{43{,}478} = 13{,}574 + 3{,}435 = \mathbf{17{,}009\text{ cm}^2}$$
   - **Detalhamento e verificação real no Vão C:**
     - **Armadura de tração (inferior):** $\mathbf{6\phi 20\text{ mm}}$ em 2 camadas de 3 barras ($A_{s,ef,C} = \mathbf{18{,}850\text{ cm}^2}$), com $a_h = 3{,}87\text{ cm} \ge 2{,}28\text{ cm}$, $a_v = 2{,}00\text{ cm}$, $y_s = 2{,}00\text{ cm}$ e $d_{\text{real},C} = 50 - 2{,}5 - 0{,}63 - 1{,}00 - 2{,}00 = \mathbf{43{,}87\text{ cm}}$.
     - **Armadura de compressão (superior):** $\mathbf{3\phi 16\text{ mm}}$ em 1 camada ($A'_{s,ef,C} = \mathbf{6{,}032\text{ cm}^2}$ — aproveitando 3 barras corridas da armadura superior!), com $d'_{\text{real},C} = 2{,}5 + 0{,}63 + 0{,}80 = \mathbf{3{,}93\text{ cm}}$.
     - **Verificação de $\beta_{x,ef}$ e $M_{rd,ef}$ (`[AB]`):**
       $$\beta_{x,ef,C} = \frac{(18{,}850 - 6{,}032) \times 43{,}478}{0{,}85 \times 0{,}80 \times 20 \times 43{,}87 \times 2{,}1429} = \mathbf{0{,}4359} \le 0{,}45 \quad (\text{Ductilidade OK!})$$
       $$\varepsilon'_s = 3{,}5\left(\frac{0{,}4359 \times 43{,}87 - 3{,}93}{0{,}4359 \times 43{,}87}\right) = \mathbf{2{,}781\text{‰}} \ge 2{,}07\text{‰} \implies \beta'_s = 1{,}0$$
       $$M_{rd,ef,C} = (18{,}850 - 6{,}032)(43{,}87)\left[1 - 0{,}4(0{,}4359)\right](43{,}478) + 6{,}032(43{,}478)(43{,}87 - 3{,}93) = \mathbf{306{,}60\text{ kN}\cdot\text{m}} \ge 279{,}00\text{ kN}\cdot\text{m} \quad (\text{OK!})$$
     - **Taxa máxima `[AC]`:** $\rho_{\max} = \dfrac{18{,}850 + 6{,}032}{20 \times 50} = \mathbf{2{,}49\%} \le 4{,}00\%$ (**OK!**).

---

### Etapa C — Dimensionamento da Armadura Transversal nos Trechos I, II e III (Modelos I e II)

1. **Resistências ao cisalhamento e cortante mínimo ($b_w = 20\text{ cm}, d = 45\text{ cm}, \text{C30}$):** `[AS]`, `[AU]`, `[AY]`, `[BH]`
   - Taxa mínima: $\left(\dfrac{A_{sw}}{s}\right)_{min} = 0{,}06 \times 20 \times \dfrac{\sqrt[3]{30^2}}{435} = \mathbf{0{,}02663\text{ cm}^2/\text{cm}} = \mathbf{2{,}663\text{ cm}^2/\text{m}}$.
   - Parcela $V_{c0} = 0{,}6\,f_{ctd}\,b_w d = 0{,}6 \times 0{,}14484 \times 20 \times 45 = \mathbf{78{,}205\text{ kN}}$.
   - Resistência das bielas comprimidas:
     $$V_{rdc,I} = 0{,}268 \times 20 \times 45 \times \left(1 - \frac{30}{250}\right) \times 2{,}1429 = \mathbf{454{,}83\text{ kN}} \qquad V_{rdc,II} = 0{,}232 \times 20 \times 45 \times 0{,}88 \times 2{,}1429 = \mathbf{393{,}74\text{ kN}}$$
   - Cortante solicitante máximo para uso de armadura mínima `[BH]`:
     $$V_{sd,\min,I} = 0{,}9(0{,}02663)(45)(43{,}478) + 78{,}205 = \mathbf{125{,}10\text{ kN}}$$
     $$V_{sd,\min,II} = 1{,}559(0{,}02663)(45)(43{,}478) + 78{,}205\left[1 - \frac{81{,}231}{393{,}737}\right] = \mathbf{143{,}31\text{ kN}}$$

2. **Reduções de $V_{sd}$ junto aos apoios B e D ($d/2 = 22{,}5\text{ cm}$ da face do pilar de $20\text{ cm}$):** `[BB]`
   A carga distribuída de cálculo $g_d = 1{,}35 \times 20 = 27{,}0\text{ kN/m}$ permite reduzir o cortante entre o eixo do pilar e a seção a $0{,}10\text{ m} + 0{,}225\text{ m} = 0{,}325\text{ m}$ do eixo ($\Delta V_{d/2} = 27{,}0 \times 0{,}325 = 8{,}775\text{ kN}$; na face do pilar $\Delta V_{\text{face}} = 27{,}0 \times 0{,}10 = 2{,}70\text{ kN}$):
   - **Verificação de $V_{rdc}$ na face crítica (`[AR]`):** $|V_{sd,\text{face},\max}| = 149{,}55\text{ kN} \le V_{rdc,II} = 393{,}74\text{ kN} < V_{rdc,I} = 454{,}83\text{ kN}$ (**Bielas folgadas em ambos os modelos!**).

3. **Quadro de Dimensionamento e Detalhamento por Trecho (Estribos de 2 ramos, $\phi_t = 6{,}3\text{ mm} \implies A_{sw,ef} = 0{,}623\text{ cm}^2$):** `[AZ]`, `[BA]`, `[BE]`, `[BF]`, `[BI]`
   - Limites de bitola (`[AZ]`): $5\text{ mm} \le \phi_t = 6{,}3\text{ mm} \le b_w/10 = 20\text{ mm}$ (**OK**).
   - Limites de espaçamento (`[BA]`): como $V_{sd}/V_{rdc} \le 0{,}38 \le 0{,}67$, $10\text{ cm} \le s \le \min(0{,}6 \times 45 = 27\text{ cm}\,;\,30\text{ cm}) \implies \mathbf{10\text{ cm} \le s \le 27\text{ cm}}$.

| Trecho da Viga | $\|V_{sd,\text{face}}\|$ (kN) | $\|V_{sd,d/2}\|$ (kN) | Modelo I: $(A_{sw}/s)_I$ ($\text{cm}^2/\text{m}$) | Modelo I: Detalhamento ($\phi_t = 6{,}3\text{ mm}$) | Modelo II ($\theta=30^\circ$): $(A_{sw}/s)_{II}$ ($\text{cm}^2/\text{m}$) | Modelo II: Detalhamento ($\phi_t = 6{,}3\text{ mm}$) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Trecho I (Balanço AB)** | $111{,}30$ | $105{,}23 \le V_{sd,\min,I}$ | **$2{,}663$** *(mínima)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** | **$2{,}663$** *(mínima)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** |
| **Trecho II (Vão BC — $\psi_0=0{,}8$)** | $146{,}55$ | $140{,}48 > V_{sd,\min,I}$ | **$3{,}536$** *(calculada)* | **$\phi 6{,}3\text{ c/ } 17\text{ cm}$** | **$2{,}663$** *(mínima)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** |
| **Trecho II (Vão BC — simult.)** | $149{,}55$ | $143{,}48 > V_{sd,\min,II}$ | **$3{,}707$** *(calculada)* | **$\phi 6{,}3\text{ c/ } 16\text{ cm}$** | **$2{,}670$** *(calculada)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** |
| **Trecho III (Vão CD)** | $121{,}05$ | $114{,}98 \le V_{sd,\min,I}$ | **$2{,}663$** *(mínima)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** | **$2{,}663$** *(mínima)* | **$\phi 6{,}3\text{ c/ } 23\text{ cm}$** |

### Conclusão — O que torna o Exercício Completo Integrado (Tema 7) um Caso Clássico de Prova?
- **Visão de Prova Integrada (Formulários 1 + 2 + 3):** Em exames de aproveitamento, é muito comum uma questão encadear **Combinações $\to$ Flexão Longitudinal $\to$ Cisalhamento** na mesma viga. O desafio aqui não é apenas a extensão, mas sim **não carregar um erro de uma etapa para a outra** e reconhecer como o comportamento muda de seção para seção:
  1. **Na Etapa A (Combinações):** A carga acidental $Q_{k1}$ na ponta do balanço é **desfavorável** para o apoio B ($M_{Q1}(B) = -80\text{ kN}\cdot\text{m}$) e para o cortante em BC ($V_{Q1}(\text{BC}) = +10\text{ kN}$), mas é **favorável (alivia!)** o momento positivo no meio do vão C ($M_{Q1}(C) = -40\text{ kN}\cdot\text{m}$) e o cortante negativo em CD ($V_{Q1}(\text{CD}) = +10\text{ kN}$). Por isso, para maximizar $M_{sd,C}^+$ e $|V_{sd,\text{III}}|$, **deve-se zerar $Q_{k1}$ ($\gamma_{q1} = 0$)**!
  2. **Na Etapa B (Flexão):** A mesma seção $20 \times 50\text{ cm}$ ($M_{rd,lim} = 217{,}76\text{ kN}\cdot\text{m}$) trabalha como **Armadura Simples** no apoio B ($|M_{sd,B}^-| = 174{,}0\text{ kN}\cdot\text{m} \le M_{rd,lim}$) e como **Armadura Dupla** no meio do vão C ($M_{sd,C}^+ = 279{,}0\text{ kN}\cdot\text{m} > M_{rd,lim}$). Além disso, o alojamento em **2 camadas** altera $d_{\text{real}}$ e exige a verificação final de $\beta_{x,ef} \le 0{,}45$ (`[AB]`).
  3. **Na Etapa C (Cisalhamento):** O uso direto de $V_{sd,\min,I} = 125{,}10\text{ kN}$ e $V_{sd,\min,II} = 143{,}31\text{ kN}$ (Bloco `[BH]`) economiza muito tempo de prova: após descontar $\Delta V_{d/2} = 8{,}775\text{ kN}$ a $d/2$ da face do pilar (`[BB]`), vê-se imediatamente que os Trechos I e III ($105{,}23$ e $114{,}98\text{ kN}$) caem direto na **armadura mínima**, restando apenas o Trecho II para cálculo efetivo!
