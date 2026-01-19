---
type: mental-model
title: "Survivorship Bias"
category:
  - pensamento-geral
origin: Statistics, Logic
author_reference: Abraham Wald, statistical analysis
domains:
  - estatística
  - lógica
  - tomada de decisão
  - análise
tags:
  - modelo-mental
  - pensamento
  - viés de sobrevivência
  - lógica
  - estatística
aliases:
  - Viés de Sobrevivência
  - Survivor Bias
  - Selection Bias
created: 2025-01-27
updated: 2025-01-27
---
# [[Survivorship Bias]]

> **Teste de Pertinência:** *Você está analisando apenas casos de sucesso e ignorando casos de falha que não são visíveis, ou está superestimando quão replicável sucesso é porque só vê histórias de sucesso? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Survivorship Bias (Viés de Sobrevivência) é erro lógico onde você se concentra em pessoas ou coisas que "sobreviveram" algum processo e inadvertidamente ignora aquelas que não sobreviveram - tipicamente porque não são visíveis. Isto leva a conclusões falsas porque você está analisando apenas subconjunto de dados, não conjunto completo. Você vê apenas sucessos e ignora maioria invisível de falhas.

**Explicação:**
Este modelo funciona porque reconhece que quando analisamos apenas sobreviventes (sucessos), perdemos informação crítica sobre não-sobreviventes (falhas). Isto leva a superestimar quão replicável sucesso é. Se apenas sucessos são visíveis, é tentador acreditar que seus caminhos (desistir, tomar riscos, certa sorte) são geralmente replicáveis. Mas frequentemente não são - muitos tentaram mesmas coisas e falharam, mas não são visíveis.

A lógica central é que para entender verdadeiramente o que funciona, você precisa ver tanto sucessos quanto falhas. Se você só vê sucessos, você pode:
- **Superestimar replicabilidade:** Acreditar que caminhos de sucesso são geralmente replicáveis quando não são
- **Mal alocar esforço ou recursos:** Perseguir estratégias que funcionaram para vencedores visíveis, ignorando que muitas tentativas similares falharam
- **Criar narrativas falsas:** Assumir que "grit", "paixão" ou "grande visão" são suficientes, ignorando variáveis silenciosas como privilégio, sistemas de suporte, ou simplesmente estar no lugar certo na hora certa

Funciona porque:
- **Apenas sucessos são visíveis:** Falhas frequentemente não são visíveis - empresas que falham fecham silenciosamente, pessoas que não têm sucesso não fazem manchetes.
- **Cria narrativas enganosas:** Histórias de sucesso criam narrativas sobre o que "faz" alguém ter sucesso, ignorando que muitos com mesmas características falharam.
- **Superestima probabilidade de sucesso:** Se você só vê sucessos, superestima probabilidade de sucesso.
- **Ignora base rates:** Não considera taxas base (taxas gerais de falha versus sucesso) - apenas estuda exemplos bem-sucedidos.

**Exemplo clássico - Aviões da Segunda Guerra:**
Durante Segunda Guerra Mundial, analistas militares observaram que aviões retornando tinham dano pesado em asas, caudas e fuselagens. Pensaram em adicionar blindagem lá. Estatístico Abraham Wald apontou que sobreviventes são aviões que *puderam* retornar - áreas com menos buracos são aquelas que, quando atingidas, causaram aviões a caírem. Então aqueles eram os pontos que militares reforçaram.

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Apenas sobreviventes (sucessos) são visíveis - não-sobreviventes (falhas) frequentemente não são visíveis.
* **Pressuposto 2:** Analisar apenas sobreviventes leva a conclusões falsas porque você está analisando apenas subconjunto de dados.
* **Pressuposto 3:** Para entender verdadeiramente o que funciona, você precisa ver tanto sucessos quanto falhas.
* **Pressuposto 4:** Superestimar replicabilidade de sucesso porque só vê histórias de sucesso leva a má alocação de esforço ou recursos.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Análise de sucesso:** Ao analisar o que leva ao sucesso, buscar ativamente dados sobre falhas - não apenas sucessos.
- **Tomada de decisão:** Ao tomar decisões baseadas em histórias de sucesso, reconhecer que você pode estar ignorando falhas invisíveis.
- **Avaliação de estratégias:** Ao avaliar estratégias (modelos de negócios, hábitos, decisões), identificar falhas ocultas bem como sucessos visíveis.
- **Aprendizado:** Ao aprender de exemplos, buscar exemplos de falha também - não apenas sucessos.
- **Análise de dados:** Ao analisar dados, reconhecer quando você pode estar analisando apenas subconjunto (sobreviventes) e não conjunto completo.

**Domínios Típicos:** Análise de Dados, Tomada de Decisão, Aprendizado, Avaliação de Estratégias, Estatística.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Quando dados completos estão disponíveis:** Se você tem acesso a dados completos (sucessos e falhas), viés de sobrevivência não se aplica.
- **Não como desculpa para não aprender:** Não usar modelo como desculpa para não aprender de exemplos de sucesso.
- **Não ignorar lições de sucesso:** Não ignorar que há lições valiosas a aprender de sucessos - apenas reconheça que você precisa ver falhas também.
- **Não assumir que sempre existe:** Não assumir que viés de sobrevivência sempre existe - em alguns contextos, dados completos podem estar disponíveis.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Superestimar replicabilidade:** Acreditar que caminhos de sucesso são geralmente replicáveis porque só vê sucessos.
- **Mal alocar esforço:** Perseguir estratégias que funcionaram para vencedores visíveis, ignorando que muitas tentativas similares falharam.
- **Criar narrativas falsas:** Assumir que características de sucesso (grit, paixão, visão) são suficientes, ignorando variáveis silenciosas.
- **Ignorar base rates:** Não considerar taxas base (taxas gerais de falha versus sucesso) - apenas estudar exemplos bem-sucedidos.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está analisando apenas sucessos e ignorando falhas.
  - Você está superestimando quão replicável sucesso é.
  - Você está perseguindo estratégias baseadas apenas em sucessos visíveis.
  - Você não está considerando taxas base de falha versus sucesso.

* **Evidência Prática:** 
  - Suas análises estão incorretas porque você está analisando apenas subconjunto de dados.
  - Você está mal alocando esforço porque persegue estratégias que funcionaram para vencedores visíveis mas ignoram falhas.
  - Você superestima probabilidade de sucesso porque só vê sucessos.

## 5. Passos de Pensamento (Algoritmo)
1. **Reconheça viés de sobrevivência:** Ao analisar sucessos, reconheça que você pode estar analisando apenas sobreviventes e ignorando não-sobreviventes que não são visíveis.

2. **Busque ativamente dados sobre falhas:** Não apenas sucessos - busque ativamente dados sobre falhas. O que você não está vendo? Quem tentou e falhou?

3. **Use taxas base:** Use taxas base (taxas gerais de falha versus sucesso) em vez de apenas estudar exemplos bem-sucedidos. Qual é taxa geral de sucesso?

4. **Questione histórias de sucesso:** Ao ver histórias de sucesso, questione: O que não estamos vendo? Que riscos, privilégios ou boa sorte ajudaram essa pessoa/empresa que não são óbvios?

5. **Identifique falhas ocultas:** Ao avaliar estratégias (modelos de negócios, hábitos, decisões), identifique falhas ocultas bem como sucessos visíveis. Isto dá imagem mais clara do que funciona e do que não funciona.

6. **Considere o que não sobreviveu:** Ao analisar sobreviventes, considere o que não sobreviveu e por quê. Isto pode revelar informação crítica.

7. **Avalie replicabilidade realisticamente:** Após ver tanto sucessos quanto falhas, avalie realisticamente quão replicável sucesso é. Não superestime baseado apenas em sucessos visíveis.

8. **Use em análise de dados:** Ao analisar dados, reconheça quando você pode estar analisando apenas subconjunto (sobreviventes) e não conjunto completo. Ajuste análise accordingly.

9. **Monitore e ajuste:** Após fazer análises, monitore se viés de sobrevivência estava afetando conclusões. Ajuste se necessário.

10. **Balance sucessos e falhas:** Encontre balance apropriado - aprenda de sucessos, mas também veja falhas para entender verdadeiramente o que funciona.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao analisar estratégias de negócios e o resultado foi buscar ativamente dados sobre falhas, não apenas sucessos, resultando em análise muito mais realista do que funciona.

* **Erro:** Ignorei este modelo ao aprender de histórias de sucesso e paguei o preço ao superestimar quão replicável sucesso era, resultando em estratégias que não funcionaram porque ignorei falhas invisíveis.

* **Insight:** Descobri que viés de sobrevivência é especialmente poderoso quando apenas sucessos são visíveis - empresas que falham fecham silenciosamente, pessoas que não têm sucesso não fazem manchetes.

* **Aplicação prática:** Usei este modelo para melhorar tomada de decisão, descobrindo que buscar ativamente dados sobre falhas e usar taxas base resulta em análises muito mais realistas e decisões muito melhores.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Selection Bias]]
* [[Base Rate Fallacy]]
* [[Confirmation Bias]]
* [[Sampling Bias]]
* [[Data Analysis]]

**Fontes:**
* Wald, Abraham - Statistical analysis of aircraft damage (WWII)
* Wikipedia - Survivorship Bias
* Research on statistical biases and logical fallacies

**Exemplos Notáveis:**
* **Aviões da Segunda Guerra:** Analistas observaram dano em aviões retornando e pensaram em adicionar blindagem lá. Wald apontou que áreas com menos buracos são aquelas que, quando atingidas, causaram aviões a caírem - então aqueles eram pontos a reforçar.
* **Dropouts de faculdade:** Histórias sobre Bill Gates, Steve Jobs e Mark Zuckerberg deixam impressão de que desistir de faculdade é caminho para sucesso massivo. Mas enquanto essas pessoas fizeram manchetes, são outliers - muitos que desistiram não tiveram sucesso, mas não são visíveis.
