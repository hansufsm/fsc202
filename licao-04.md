**FSC202 - Eletromagnetismo**

Prof. Hans R Zimermann

2026

**Lição 05: Fluxo do Campo Elétrico e o Enunciado Fundamental da Lei de Gauss**

Número da Lição: 05 Título: Fluxo do Campo Elétrico e o Enunciado Fundamental da Lei de Gauss Unidade temática: Lei de Gauss Tópicos principais: Conceito de fluxo elétrico, cálculo do fluxo através de superfícies abertas e fechadas, Lei de Gauss (enunciado e forma integral), aplicação da Lei de Gauss para distribuições de carga com alta simetria. Pré-requisitos: Campo elétrico, vetores, cálculo integral (Lição 04). Conexão com a lição anterior: Introduz uma ferramenta poderosa para calcular campos elétricos, especialmente para distribuições de carga simétricas, como alternativa à integração direta da Lei de Coulomb. Objetivos de aprendizagem:

1. Definir e calcular o fluxo elétrico através de uma superfície.

2. Enunciar a Lei de Gauss em sua forma integral.

3. Explicar a relação entre o fluxo elétrico e a carga líquida envolvida por uma superfície fechada.

4. Identificar situações onde a Lei de Gauss pode ser aplicada de forma simplificada devido à simetria.

5. Aplicar a Lei de Gauss para determinar o campo elétrico de distribuições de carga simples e simétricas.



**Introdução**

Até agora, calculamos o campo elétrico usando a Lei de Coulomb e o princípio da superposição, o que pode ser computacionalmente intensivo para distribuições contínuas de carga. Nesta lição, introduzimos uma ferramenta mais elegante e poderosa para calcular campos el elétricos em situações de alta simetria: a **Lei de Gauss**. Antes de enunciá-la, precisamos entender o conceito de **fluxo elétrico**.

**Fluxo do Campo Elétrico**

O conceito de fluxo é uma medida de “quanto” de um campo vetorial atravessa uma determinada superfície. Para o campo elétrico, o fluxo elétrico $\Phi_E$ através de uma superfície é uma medida do número de linhas de campo elétrico que a atravessam.

***Fluxo através de uma Pequena Área Plana***

Considere um campo elétrico uniforme $\vec{E}$ atravessando uma pequena área plana $dA$. Definimos um vetor área $d\vec{A}$ cuja magnitude é $dA$ e cuja direção é perpendicular à superfície (normal à superfície). O fluxo elétrico elementar $d\Phi_E$ através dessa área é:

$$d\Phi_E = \vec{E} \cdot d\vec{A} = E dA \cos\theta$$

Onde $\theta$ é o ângulo entre o vetor campo elétrico $\vec{E}$ e o vetor área $d\vec{A}$.

* Se $\vec{E}$ é paralelo a $d\vec{A}$ ($\theta = 0^\circ$), $\cos\theta = 1$, e o fluxo é máximo ($E dA$).

* Se $\vec{E}$ é perpendicular a $d\vec{A}$ ($\theta = 90^\circ$), $\cos\theta = 0$, e o fluxo é zero.

* Se $\vec{E}$ aponta para dentro da superfície ($\theta > 90^\circ$), $\cos\theta < 0$, e o fluxo é negativo.

A unidade de fluxo elétrico no SI é **N**$\cdot$**m**$^2$**/C**.

***Fluxo através de uma Superfície Geral***

Para uma superfície de tamanho finito e/ou um campo elétrico não uniforme, o fluxo elétrico total é a integral de superfície do produto escalar $\vec{E} \cdot d\vec{A}$:

$$\Phi_E = \int \vec{E} \cdot d\vec{A}$$

Se a superfície for **fechada** (como uma esfera ou um cubo), a integral é denotada por um círculo no sinal de integral:

$$\Phi_E = \oint \vec{E} \cdot d\vec{A}$$

Por convenção, para uma superfície fechada, o vetor $d\vec{A}$ sempre aponta para fora da superfície.

**Exemplo 3.1: Fluxo através de um cubo.** Um campo elétrico uniforme $\vec{E} = (3.0 \hat{i}) \text{ N/C}$ atravessa um cubo de lado $L = 0.1 \text{ m}$ com uma face no plano $yz$ (ou seja, a face esquerda está em $x=0$). Calcule o fluxo elétrico total através do cubo.

**Solução:** O campo elétrico é uniforme e aponta na direção $+x$. As faces do cubo são:

1. **Face esquerda (**$x=0$**):**$d\vec{A} = -dA \hat{i}$. $\Phi_{E,esquerda} = \int \vec{E} \cdot d\vec{A} = \int (3.0 \hat{i}) \cdot (-dA \hat{i}) = -3.0 \int dA = -3.0 L^2 = -3.0 (0.1)^2 = -0.03 \text{ N}\cdot\text{m}^2/\text{C}$.

2. **Face direita (**$x=L$**):**$d\vec{A} = +dA \hat{i}$. $\Phi_{E,direita} = \int \vec{E} \cdot d\vec{A} = \int (3.0 \hat{i}) \cdot (+dA \hat{i}) = +3.0 \int dA = +3.0 L^2 = +3.0 (0.1)^2 = +0.03 \text{ N}\cdot\text{m}^2/\text{C}$.

3. **Faces superior, inferior, frontal e traseira:** Para essas faces, o vetor área $d\vec{A}$ é perpendicular ao campo $\vec{E}$ (por exemplo, para a face superior, $d\vec{A} = dA \hat{j}$, e $\vec{E} \cdot d\vec{A} = 0$). Portanto, o fluxo através dessas quatro faces é zero.

O fluxo total através do cubo é a soma dos fluxos através de todas as faces: $\Phi_{E,total} = \Phi_{E,esquerda} + \Phi_{E,direita} + 0 + 0 + 0 + 0 = -0.03 + 0.03 = 0$. O fluxo elétrico total através do cubo é zero. Isso ocorre porque o campo é uniforme e não há carga líquida dentro do cubo.

**Lei de Gauss**

A Lei de Gauss é uma das quatro equações de Maxwell e é fundamental para a eletrostática. Ela relaciona o fluxo elétrico total através de uma superfície fechada com a carga elétrica líquida contida dentro dessa superfície.

**Enunciado Fundamental:** O fluxo elétrico líquido através de qualquer superfície gaussiana (superfície fechada imaginária) é proporcional à carga elétrica líquida envolvida por essa superfície.

**Forma Integral:**

$$\oint \vec{E} \cdot d\vec{A} = \frac{Q_{int}}{\epsilon_0}$$

Onde:

* $\oint \vec{E} \cdot d\vec{A}$ é o fluxo elétrico total através da superfície fechada.

* $Q_{int}$ é a carga elétrica líquida total contida **dentro** da superfície gaussiana.

* $\epsilon_0 = 8.854 \times 10^{-12} \text{ C}^2/(\text{N} \cdot \text{m}^2)$ é a permissividade do vácuo.

**Interpretação:**

* Se $Q_{int} > 0$, o fluxo é positivo (linhas de campo saem da superfície).

* Se $Q_{int} < 0$, o fluxo é negativo (linhas de campo entram na superfície).

* Se $Q_{int} = 0$, o fluxo é zero (o mesmo número de linhas que entram, saem).

* A Lei de Gauss é sempre verdadeira, mas é particularmente útil para calcular o campo elétrico quando a distribuição de carga possui alta simetria.

**Aplicação da Lei de Gauss: Escolha da Superfície Gaussiana**

Para aplicar a Lei de Gauss de forma eficaz, devemos escolher uma **superfície gaussiana** (uma superfície fechada imaginária) que aproveite a simetria da distribuição de carga. As condições ideais para a superfície gaussiana são:

1. O campo elétrico $\vec{E}$ é **constante em magnitude** em toda a superfície (ou em partes dela).

2. O campo elétrico $\vec{E}$ é **paralelo ou perpendicular** ao vetor área $d\vec{A}$ em toda a superfície (ou em partes dela).

As simetrias mais comuns são:

* **Simetria esférica:** Para cargas puntiformes, esferas carregadas uniformemente, cascas esféricas. A superfície gaussiana é uma esfera concêntrica.

* **Simetria cilíndrica:** Para fios infinitos, cilindros carregados uniformemente. A superfície gaussiana é um cilindro coaxial.

* **Simetria planar:** Para planos infinitos carregados uniformemente. A superfície gaussiana é um cilindro ou caixa retangular com faces paralelas ao plano.

**Exemplo 3.2: Campo elétrico de uma carga puntiforme usando a Lei de Gauss.** Use a Lei de Gauss para encontrar o campo elétrico a uma distância $r$ de uma carga puntiforme $Q$.

**Solução:**

1. **Simetria:** A distribuição de carga (uma carga puntiforme) tem simetria esférica.

2. **Superfície Gaussiana:** Escolhemos uma esfera de raio $r$ centrada na carga $Q$.

3. **Cálculo do Fluxo:**

   * Devido à simetria esférica, o campo elétrico $\vec{E}$ é radial e tem a mesma magnitude em todos os pontos da superfície gaussiana.

   * O vetor área $d\vec{A}$ também é radial e aponta para fora, sendo paralelo a $\vec{E}$ em todos os pontos.

   * Portanto, $\vec{E} \cdot d\vec{A} = E dA \cos(0^\circ) = E dA$.

   * $\oint \vec{E} \cdot d\vec{A} = \oint E dA = E \oint dA$.

   * A integral $\oint dA$ é a área da superfície gaussiana, que é $4\pi r^2$.

   * Então, o fluxo é $\Phi_E = E (4\pi r^2)$.

4. **Carga Envolvida:** A carga líquida dentro da superfície gaussiana é $Q_{int} = Q$.

5. **Aplicação da Lei de Gauss:**

6. $$\Phi_E = \frac{Q_{int}}{\epsilon_0}$$

7. $$E (4\pi r^2) = \frac{Q}{\epsilon_0}$$

8. $$E = \frac{Q}{4\pi\epsilon_0 r^2}$$

9. Como $k = \frac{1}{4\pi\epsilon_0}$, obtemos:

10. $$E = k \frac{Q}{r^2}$$

11. Este resultado é idêntico ao obtido pela Lei de Coulomb, demonstrando a consistência e a utilidade da Lei de Gauss. A direção do campo é radial para fora se $Q>0$ e radial para dentro se $Q<0$.



**Exercício Prático com Gabarito em Python**

**Problema:** Uma linha infinita de carga possui uma densidade linear de carga uniforme $\lambda = +2.0 \text{ nC/m}$. Use a Lei de Gauss para determinar a magnitude do campo elétrico a uma distância radial $r = 0.05 \text{ m}$ da linha.

**Solução Analítica:**

1. **Simetria:** A linha de carga infinita possui simetria cilíndrica. O campo elétrico deve apontar radialmente para fora da linha (se $\lambda > 0$) e sua magnitude deve depender apenas da distância radial $r$ da linha.

2. **Superfície Gaussiana:** Escolhemos um cilindro gaussiano de raio $r$ e comprimento $L$, coaxial com a linha de carga.

3. **Cálculo do Fluxo:** A superfície gaussiana tem três partes:

   * **Tampa superior e inferior:** O campo elétrico $\vec{E}$ é radial, enquanto o vetor área $d\vec{A}$ para as tampas é perpendicular ao eixo do cilindro (paralelo ao eixo $z$). Portanto, $\vec{E} \cdot d\vec{A} = 0$ para as tampas. O fluxo através das tampas é zero.

   * **Superfície lateral:** O campo elétrico $\vec{E}$ é perpendicular à superfície lateral e tem a mesma magnitude $E$ em todos os pontos dessa superfície. O vetor área $d\vec{A}$ também é perpendicular à superfície lateral e aponta para fora, sendo paralelo a $\vec{E}$.

      * $\Phi_{E,lateral} = \oint \vec{E} \cdot d\vec{A} = \oint E dA = E \oint dA$.

      * A integral $\oint dA$ é a área da superfície lateral do cilindro, que é $2\pi r L$.

      * Então, o fluxo através da superfície lateral é $\Phi_{E,lateral} = E (2\pi r L)$.

   * O fluxo total através da superfície gaussiana é $\Phi_E = E (2\pi r L)$.

4. **Carga Envolvida:** A carga líquida dentro da superfície gaussiana é a carga contida no comprimento $L$ da linha.

   * $Q_{int} = \lambda L$.

5. **Aplicação da Lei de Gauss:**

6. $$\Phi_E = \frac{Q_{int}}{\epsilon_0}$$

7. $$E (2\pi r L) = \frac{\lambda L}{\epsilon_0}$$

8. Cancelando $L$ de ambos os lados:

9. $$E = \frac{\lambda}{2\pi\epsilon_0 r}$$

10. Substituindo $k = \frac{1}{4\pi\epsilon_0}$, podemos escrever $E = \frac{2k\lambda}{r}$.

11. **Cálculo numérico:**

   * $\lambda = +2.0 \times 10^{-9} \text{ C/m}$

   * $r = 0.05 \text{ m}$

   * $\epsilon_0 = 8.854 \times 10^{-12} \text{ C}^2/(\text{N} \cdot \text{m}^2)$

12. $$E = \frac{2.0 \times 10^{-9} \text{ C/m}}{2\pi (8.854 \times 10^{-12} \text{ C}^2/(\text{N} \cdot \text{m}^2)) (0.05 \text{ m})}$$

13. $$E = \frac{2.0 \times 10^{-9}}{2\pi \times 8.854 \times 10^{-12} \times 0.05}$$

14. $$E \approx \frac{2.0 \times 10^{-9}}{2.784 \times 10^{-12}} \approx 718.3 \text{ N/C}$$

15. A direção do campo é radialmente para fora da linha de carga.

**Validação Numérica em Python:**

```python
import numpy as np

# Constantes físicas
epsilon_0 = 8.854e-12  # Permissividade do vácuo em C^2/(N m^2)
k = 1 / (4 * np.pi * epsilon_0)  # Constante de Coulomb

# Dados do problema
lambda_carga = 2.0e-9  # Densidade linear de carga em C/m (2 nC/m)
r_distancia = 0.05  # Distância radial em metros (5 cm)

print(f"Densidade linear de carga (lambda): {lambda_carga*1e9:.1f} nC/m")
print(f"Distância radial (r): {r_distancia:.2f} m")

# Fórmula para o campo elétrico de uma linha infinita de carga
# E = lambda / (2 * pi * epsilon_0 * r)
E_magnitude = lambda_carga / (2 * np.pi * epsilon_0 * r_distancia)

print(f"Magnitude do Campo Elétrico (E): {E_magnitude:.1f} N/C")

# Comparação com a solução analítica:
# E = 718.3 N/C
# Os resultados são consistentes.
```



**Exercício Desafio com Visualização**

**Problema:** Um plano infinito não condutor possui uma densidade superficial de carga uniforme $\sigma = +1.0 \text{ nC/m}^2$.

1. Use a Lei de Gauss para derivar a expressão para o campo elétrico em qualquer ponto fora do plano.

2. Crie um gráfico que represente o campo elétrico em função da distância $x$ ao plano, para $x > 0$.

**Solução Analítica (Parte 1):**

1. **Simetria:** Um plano infinito de carga possui simetria planar. O campo elétrico deve ser uniforme em magnitude e direção, perpendicular ao plano, e apontar para fora do plano (se $\sigma > 0$).

2. **Superfície Gaussiana:** Escolhemos um cilindro gaussiano (ou caixa retangular) que atravessa o plano. As tampas do cilindro são paralelas ao plano de carga, e a superfície lateral é perpendicular ao plano.

3. **Cálculo do Fluxo:**

   * **Superfície lateral:** O campo elétrico $\vec{E}$ é paralelo ao plano e, portanto, perpendicular ao vetor área $d\vec{A}$ da superfície lateral. Assim, $\vec{E} \cdot d\vec{A} = 0$. O fluxo através da superfície lateral é zero.

   * **Tampas (superior e inferior):** O campo elétrico $\vec{E}$ é perpendicular ao plano e, portanto, paralelo ao vetor área $d\vec{A}$ das tampas. Se a área de cada tampa é $A$, e o campo tem magnitude $E$ em cada tampa:

      * Para a tampa superior (assumindo $x>0$), $\vec{E}$ e $d\vec{A}$ apontam na mesma direção (para fora). Fluxo é $E A$.

      * Para a tampa inferior (assumindo $x<0$), $\vec{E}$ aponta na direção oposta ao $d\vec{A}$ (para fora). Mas como o campo de um plano positivo aponta para fora do plano, e o $d\vec{A}$ da tampa inferior aponta para fora, eles estão na mesma direção. Fluxo é $E A$.

      * Fluxo total através das tampas é $E A + E A = 2EA$.

   * O fluxo total através da superfície gaussiana é $\Phi_E = 2EA$.

4. **Carga Envolvida:** A carga líquida dentro da superfície gaussiana é a carga contida na área $A$ do plano que está dentro do cilindro.

   * $Q_{int} = \sigma A$.

5. **Aplicação da Lei de Gauss:**

6. $$\Phi_E = \frac{Q_{int}}{\epsilon_0}$$

7. $$2EA = \frac{\sigma A}{\epsilon_0}$$

8. Cancelando $A$ de ambos os lados:

9. $$E = \frac{\sigma}{2\epsilon_0}$$

10. Este resultado mostra que o campo elétrico de um plano infinito de carga uniforme é **constante** e **independente da distância** ao plano. A direção é perpendicular ao plano, apontando para fora se $\sigma > 0$ e para dentro se $\sigma < 0$.

**Visualização em Python (Parte 2):**

```python
import numpy as np
import matplotlib.pyplot as plt

# Constantes físicas
epsilon_0 = 8.854e-12  # Permissividade do vácuo em C^2/(N m^2)

# Dados do problema
sigma_carga = 1.0e-9  # Densidade superficial de carga em C/m^2 (1 nC/m^2)

# Função para calcular o campo elétrico de um plano infinito
def campo_eletrico_plano(sigma, epsilon_0):
   return sigma / (2 * epsilon_0)

# Calcular a magnitude do campo elétrico
E_magnitude = campo_eletrico_plano(sigma_carga, epsilon_0)

# Criar um array de distâncias x
# O campo é constante, mas vamos plotar para ilustrar a independência da distância
x_distancias = np.linspace(0.01, 0.5, 100)  # Distâncias em metros (evitar x=0)

# O campo elétrico é constante para qualquer x > 0
E_valores = np.full_like(x_distancias, E_magnitude)

# Plotar o gráfico
plt.figure(figsize=(10, 6))
plt.plot(x_distancias, E_valores, color='blue', linewidth=2)

plt.title('Campo Elétrico de um Plano Infinito de Carga Uniforme')
plt.xlabel('Distância $x$ ao Plano (m)')
plt.ylabel('Magnitude do Campo Elétrico $E$ (N/C)')
plt.grid(True, linestyle='--', alpha=0.7)
plt.ylim(0, E_magnitude * 1.2)  # Ajustar limite Y para melhor visualização
plt.axhline(E_magnitude, color='red', linestyle='--', label=f'E = {E_magnitude:.1f} N/C')
plt.legend()
plt.show()

print(f"Densidade superficial de carga (sigma): {sigma_carga*1e9:.1f} nC/m^2")
print(f"Magnitude do Campo Elétrico (E): {E_magnitude:.1f} N/C")
```

**Interpretação do Gráfico:** O gráfico mostra que a magnitude do campo elétrico de um plano infinito de carga uniforme é **constante** e não varia com a distância $x$ ao plano. Isso é uma característica única de distribuições de carga infinitas e uniformes, que simplifica enormemente o cálculo do campo elétrico. A linha horizontal azul representa essa constância, e a linha tracejada vermelha confirma o valor calculado.



**Exercícios de Fixação**

1. Um campo elétrico uniforme $\vec{E} = (200 \hat{i} + 300 \hat{j}) \text{ N/C}$ atravessa uma superfície retangular de área $0.2 \text{ m}^2$ no plano $xy$. Calcule o fluxo elétrico através desta superfície.

2. Uma carga puntiforme de $+10 \text{ nC}$ está no centro de uma esfera de raio $0.1 \text{ m}$. Calcule o fluxo elétrico total através da superfície da esfera. Se o raio da esfera fosse dobrado, como o fluxo mudaria?

3. Uma casca esférica condutora de raio interno $R_1$ e raio externo $R_2$ possui uma carga líquida $Q$. Uma carga puntiforme $q$ é colocada no centro da casca. Use a Lei de Gauss para encontrar o campo elétrico nas três regiões: $r < R_1$, $R_1 < r < R_2$, e $r > R_2$.

4. Explique por que a Lei de Gauss é particularmente útil para distribuições de carga com alta simetria, mas não é tão prática para distribuições de carga arbitrárias.

5. Um cilindro infinito de raio $R$ possui uma densidade de carga volumétrica uniforme $\rho$. Use a Lei de Gauss para encontrar o campo elétrico para $r < R$ e $r > R$.

6. Um cubo de lado $L$ está em uma região onde o campo elétrico é dado por $\vec{E} = (ax \hat{i}) \text{ N/C}$, onde $a$ é uma constante. Calcule o fluxo elétrico total através do cubo. Qual é a carga líquida dentro do cubo?



**Recursos Complementares**

* **Livro Texto:**

   * HALLIDAY, D.; RESNICK, R.; WALKER, J. **Fundamentos de Física, Volume 3: Eletromagnetismo**. 10. ed. Rio de Janeiro: LTC, 2016. (Capítulo 23: Lei de Gauss)

   * TIPLER, P. A.; MOSCA, G. **Física para Cientistas e Engenheiros, Volume 2: Eletricidade e Magnetismo, Luz**. 6. ed. Rio de Janeiro: LTC, 2009. (Capítulo 22: Lei de Gauss)

   * NUSSENZVEIG, H. M. **Curso de Física Básica, Volume 3: Eletromagnetismo**. 5. ed. São Paulo: Blucher, 2015. (Capítulo 4: Lei de Gauss)

   * GRIFFITHS, D. J. **Eletrodinâmica**. 3. ed. São Paulo: Pearson Education do Brasil, 2011. (Capítulo 2: Eletrostática, Lei de Gauss)

* **Vídeos e Simulações Online:**

   * Khan Academy: Vídeos sobre fluxo elétrico e Lei de Gauss.

   * Simulações interativas sobre Lei de Gauss e superfícies gaussianas.

* **Artigos e Textos de Apoio:**

   * Aplicações da Lei de Gauss em engenharia elétrica e física de materiais.



**Questões para Discussão**

1. O que significa um fluxo elétrico negativo através de uma superfície fechada?

2. Se o fluxo elétrico total através de uma superfície gaussiana é zero, isso implica que o campo elétrico é zero em todos os pontos da superfície? Justifique com um exemplo.

3. A Lei de Gauss é uma alternativa à Lei de Coulomb. Em que situações uma é preferível à outra?

4. Por que a escolha da superfície gaussiana é tão crucial para a aplicação prática da Lei de Gauss?

5. Discuta a relação entre o número de linhas de campo que atravessam uma superfície e o conceito de fluxo elétrico.

6. A Lei de Gauss é válida para qualquer superfície fechada, independentemente de sua forma ou tamanho. Por que, então, só a usamos para calcular o campo elétrico em casos de alta simetria?

