---
type: mental-model
title: "Regression to the Mean"
category:
  - pensamento-geral
origin: Statistics, Francis Galton
author_reference: Galton, Francis - Regression toward mediocrity
domains:
  - estatística
  - análise de dados
tags:
  - modelo-mental
  - pensamento
  - regressão à média
aliases:
  - Regressão à Média
  - Regression toward the Mean
  - Statistical Regression
created: 2025-01-27
updated: 2025-01-27
---
# [[Regression to the Mean]]

> **Teste de Pertinência:** *Você está observando valor extremo em medição e precisa entender que valor tende a estar mais próximo da média quando medido novamente, devido a efeito estatístico puro? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Regression to the Mean (Regressão à Média) descreve tendência para medições extremas em conjunto de dados serem seguidas por outras que estão mais próximas da média, se você medir mesmo fenômeno novamente. É efeito puramente estatístico - enraizado em variabilidade aleatória e erro de medição - e não implica causa ou melhoria por si só. O que sobe deve descer. Anomalia em estatística (valor extremo), tenderá a estar mais próxima da média na próxima vez que for medido. Se, quando medido segunda vez, valor é encontrado mais extremo, então valor original provavelmente estava mais próximo.

**Explicação:**
Este modelo funciona porque reconhece que maioria das medições do mundo real pode ser decomposta em duas partes: componente verdadeiro e estável ("sinal") e componente variável e imprevisível ("ruído"). Valores extremos são frequentemente aqueles onde ruído desempenhou papel grande. Quando re-medido, ruído é improvável de replicar da mesma forma, então resultado tende a ser puxado de volta em direção ao sinal (ou seja, mais próximo da média). Isto funciona porque reconhece que quando você toma medidas repetidas, correlação entre elas é frequentemente menos que perfeita. Quanto menor esta correlação, maior possibilidade de regressão à média.

A lógica central é que através de reconhecer regressão à média, você pode evitar atribuir falsamente causa a mudanças que são apenas flutuação natural. Isto funciona porque reconhece que sem contabilizar regressão à média, você pode falsamente acreditar que tratamento ou intervenção "causou" melhoria quando mudança foi apenas flutuação natural.

Funciona porque:
- **Reconhece variabilidade aleatória:** Reconhece que valores extremos frequentemente incluem componente de variabilidade aleatória.
- **Evita atribuição falsa de causa:** Ajuda a evitar atribuir falsamente causa a mudanças que são apenas flutuação natural.
- **É efeito estatístico puro:** É efeito puramente estatístico - não implica causa ou melhoria.
- **Funciona em ambas direções:** Extremos baixos tendem a aumentar, extremos altos tendem a diminuir - em direção à média.

**Por que acontece:**
- **Sinal + Ruído:** Maioria das medições pode ser decomposta em sinal (verdadeiro, estável) e ruído (variável, imprevisível).
- **Correlação imperfeita:** Quando você toma medidas repetidas, correlação entre elas é frequentemente menos que perfeita.
- **Ruído não replica:** Ruído é improvável de replicar da mesma forma, então resultado tende a regressar em direção ao sinal.

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Você está observando valor extremo em medição.
* **Pressuposto 2:** Você está medindo mesmo fenômeno novamente.
* **Pressuposto 3:** Há componente de variabilidade aleatória ou erro de medição.
* **Pressuposto 4:** Correlação entre medidas repetidas é menos que perfeita.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Interpretar mudanças extremas:** Ao interpretar mudanças extremas, reconhecer que regressão à média pode explicar parte da mudança.
- **Evitar atribuição falsa de causa:** Ao evitar atribuir falsamente causa, reconhecer que regressão à média pode explicar melhorias que são apenas flutuação natural.
- **Designar estudos:** Ao designar estudos, usar grupos de controle, ter medidas de baseline, e randomização são formas de proteger contra interpretação errônea.
- **Entender flutuação natural:** Ao entender flutuação natural, reconhecer que valores extremos tendem a regressar à média.

**Domínios Típicos:** Estatística, Pesquisa, Medicina, Esportes, Análise de Dados.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Regressão não é força:** Regressão não é força ou causa - não "puxa" coisas de volta. É sobre probabilidade e expectativa.
- **Não implica retorno perfeito:** Não implica que cada caso retorna exatamente à média - apenas que mudança média de extremos será em direção à média.
- **Não ignorar causas reais:** Não ignorar causas reais de mudança - regressão à média pode explicar parte, mas pode haver causas reais também.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Atribuir falsamente causa:** Atribuir falsamente causa a mudanças que são apenas regressão à média.
- **Ignorar em design de estudos:** Ignorar regressão à média em design de estudos - pode ameaçar validade interna.
- **Assumir retorno perfeito:** Assumir que cada caso retorna exatamente à média - apenas mudança média de extremos será em direção à média.
- **Ignorar causas reais:** Ignorar causas reais de mudança - regressão à média pode explicar parte, mas pode haver causas reais também.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está atribuindo falsamente causa a mudanças que são apenas regressão à média.
  - Você não está considerando regressão à média em design de estudos.
  - Você está assumindo que cada caso retorna exatamente à média.
  - Você está ignorando causas reais de mudança.

* **Evidência Prática:** 
  - Suas interpretações estão incorretas porque você atribuiu falsamente causa a mudanças que eram apenas regressão à média.
  - Você não está capturando realidade porque ignorou regressão à média ou causas reais.

## 5. Passos de Pensamento (Algoritmo)
1. **Identifique valor extremo:** Identifique valor extremo em medição - está muito acima ou abaixo da média?

2. **Reconheça regressão à média:** Reconheça que valor extremo tende a estar mais próximo da média quando medido novamente, devido a efeito estatístico puro.

3. **Considere sinal vs ruído:** Considere que medição pode ser decomposta em sinal (verdadeiro, estável) e ruído (variável, imprevisível) - valores extremos frequentemente incluem componente grande de ruído.

4. **Evite atribuição falsa de causa:** Evite atribuir falsamente causa a mudanças que são apenas regressão à média - melhorias podem ser apenas flutuação natural.

5. **Use grupos de controle:** Em estudos, use grupos de controle para proteger contra interpretação errônea de regressão à média.

6. **Use medidas de baseline:** Use medidas de baseline - ter medida inicial ajuda a entender se mudança é regressão à média ou causa real.

7. **Use randomização:** Use randomização - ajuda a garantir que grupos são comparáveis e que diferenças não são apenas regressão à média.

8. **Considere correlação:** Considere correlação entre medidas repetidas - quanto menor correlação, maior possibilidade de regressão à média.

9. **Monitore e ajuste:** Após interpretar mudanças, monitore se está funcionando como esperado. Ajuste se necessário.

10. **Use apropriadamente:** Use reconhecimento de regressão à média para evitar atribuição falsa de causa, mas não ignore causas reais - regressão à média pode explicar parte, mas pode haver causas reais também.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao interpretar mudanças extremas e o resultado foi reconhecer regressão à média, resultando em interpretação muito mais precisa e evitando atribuição falsa de causa.

* **Erro:** Ignorei este modelo ao interpretar melhorias e paguei o preço ao atribuir falsamente causa a mudanças que eram apenas regressão à média.

* **Insight:** Descobri que regressão à média é especialmente importante para entender que valores extremos tendem a regressar à média - é efeito estatístico puro, não causa.

* **Aplicação prática:** Usei este modelo para melhorar interpretação de dados, descobrindo que reconhecer regressão à média resulta em muito mais precisas interpretações e melhor capacidade de evitar atribuição falsa de causa.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Normal Distribution]]
* [[Statistical Regression]]
* [[Extreme Outcomes]]
* [[Measurement Error]]
* [[Correlation]]

**Fontes:**
* Galton, Francis - Regression toward mediocrity
* Wikipedia - Regression toward the mean
* Research on statistical phenomena and research design

**Exemplos Notáveis:**
* **Testes acadêmicos:** Suponha que estudantes refazem exame. Aqueles que pontuaram muito alto primeira vez são propensos a pontuar menor segunda vez, e vice-versa, porque pontuações iniciais podem ter sido aumentadas ou diminuídas por sorte.
* **Atletismo:** Atleta tem jogo excepcional (muito acima de sua média). Sua próxima performance frequentemente é menos extrema, simplesmente porque condições favoráveis (sorte, matchup, condição de pico) não são garantidas.
