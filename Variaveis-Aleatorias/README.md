# Estatistica

## Variáveis Aleatórias
Uma variável aleatória é uma função que associa um valor numérico a cada resultado em um espaço amostral de um experimento aleatório. Elas podem ser categorizadas em duas principais categorias: contínuas e discretas.

### Variáveis Aleatórias Discretas
- Uma variável aleatória discreta assume um número finito ou contável de valores. Exemplos típicos incluem o número de crianças em uma família, o número de defeitos em uma peça de produção ou o resultado de um lançamento de dados.

<b> Características Principais: </b>

1. Função de Probabilidade (p(x)):

- A função de probabilidade p(x) associa a cada valor da variável discreta x uma probabilidade P(X = x).
Exemplo: Para um dado justo de seis faces, P(X = x) = 1/6 para x = 1, 2, 3, 4, 5, 6.

2. Função de Distribuição Acumulada (F(x)):

- A função de distribuição acumulada F(x) dá a probabilidade de que a variável aleatória X assuma um valor menor ou igual a x.
F(x) = P(X ≤ x) = Σ p(k) para k ≤ x.

3. Esperança (Valor Esperado, E(X)):

- É a média ponderada dos valores possíveis da variável, onde os pesos são as probabilidades.
E(X) = Σ [x * p(x)].

4. Variância (Var(X)):

- Mede a dispersão dos valores da variável em relação à média.
Var(X) = E[(X - E(X))^2] = Σ [(x - E(X))^2 * p(x)].


<b>Exemplos de Distribuições Discretas:</b>
- Binomial: Modela o número de sucessos em uma sequência de ensaios de Bernoulli.
- Poisson: Modela o número de eventos ocorrendo em um intervalo fixo de tempo ou espaço.

  
### Variáveis Aleatórias Contínuas

- Uma variável aleatória contínua pode assumir qualquer valor dentro de um intervalo contínuo. Exemplos incluem a altura de pessoas, o tempo necessário para completar uma tarefa, ou a temperatura em um dia específico.

<b> Características Principais: </b>

1. Função Densidade de Probabilidade (f(x)):

- A função densidade de probabilidade f(x) descreve a probabilidade de a variável aleatória assumir um valor específico.
Embora a probabilidade de qualquer ponto específico seja zero, a área sob a curva f(x) entre dois pontos a e b representa a probabilidade de X estar entre a e b.
P(a ≤ X ≤ b) = ∫[a, b] f(x) dx.

2. Função de Distribuição Acumulada (F(x)):

- A função de distribuição acumulada F(x) dá a probabilidade de que a variável aleatória X seja menor ou igual a x.
F(x) = P(X ≤ x) = ∫[-∞, x] f(t) dt.

3. Esperança (Valor Esperado, E(X)):

- É a média ponderada dos valores possíveis da variável, onde os pesos são as probabilidades.
E(X) = ∫[-∞, ∞] x * f(x) dx.

4. Variância (Var(X)):

Mede a dispersão dos valores da variável em relação à média.
Var(X) = E[(X - E(X))^2] = ∫[-∞, ∞] (x - E(X))^2 * f(x) dx.

<b>Exemplos de Distribuições Contínuas:</b>
- Normal (Gaussiana): Modela fenômenos naturais e muitas outras variáveis; tem a famosa curva em forma de sino.
- Exponencial: Modela o tempo entre eventos em um processo de Poisson.
- Uniforme: Todos os intervalos de mesmo tamanho dentro do intervalo têm a mesma probabilidade.

  
### Comparação Entre Variáveis Discretas e Contínuas

1. Dominio:

- Discretas: Valores isolados, geralmente inteiros.
- Contínuas: Qualquer valor em um intervalo (podem incluir frações e decimais).

  
2. Cálculo de Probabilidades:

- Discretas: Soma das probabilidades de pontos específicos.
- Contínuas: Área sob a curva da função densidade de probabilidade.
  
3. Distribuição:

- Discretas: Função de probabilidade e distribuição acumulada através de somas.
- Contínuas: Função densidade de probabilidade e distribuição acumulada através de integrais.
  
### Aplicações Práticas

<b>Em Ciência de Dados:</b>
- Modelagem Preditiva: Compreender o tipo de variável (discreta ou contínua) é crucial para escolher o modelo estatístico ou de machine learning adequado.
- Análise Estatística: Ferramentas estatísticas diferentes são usadas para variáveis contínuas e discretas (e.g., testes de hipóteses, intervalos de confiança).
- Preprocessamento de Dados: Tratamento adequado de variáveis para alimentar algoritmos, como normalização para variáveis contínuas ou codificação para variáveis discretas.

