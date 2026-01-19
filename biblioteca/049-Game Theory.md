---
type: mental-model
title: "Game Theory"
category:
  - pensamento-geral
origin: John von Neumann, Oskar Morgenstern (1944), John Nash
author_reference: von Neumann & Morgenstern - "Theory of Games and Economic Behavior", John Nash
domains:
  - estratégia
  - economia
  - relações
  - cooperação
tags:
  - modelo-mental
  - pensamento
  - estratégia
  - economia
  - cooperação
  - competição
aliases:
  - Teoria dos Jogos
  - Strategic Decision Making
  - Nash Equilibrium
created: 2025-01-27
updated: 2025-01-27
---
# [[Game Theory]]

> **Teste de Pertinência:** *Você está em uma situação onde seu resultado depende não apenas de suas ações, mas também das ações de outros, e precisa pensar estrategicamente sobre como outros podem responder? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Game Theory (Teoria dos Jogos) é o estudo de situações estratégicas onde sucesso de um participante depende não apenas de suas próprias ações, mas também das ações de outros participantes. Força jogadores a pensar não apenas sobre suas opções, mas sobre o que outros são provavelmente fazer, já que seus resultados dependem de todas as escolhas.

**Explicação:**
Este modelo funciona porque reconhece que em muitas situações, seu resultado depende de ações de outros. Isto significa que você deve pensar estrategicamente - não apenas sobre o que você fará, mas sobre o que outros farão em resposta, e como suas ações afetarão respostas deles. Uma vez que um equilíbrio de Nash é alcançado, ninguém tem incentivo para mudar estratégia sozinho. Isto torna previsibilidade possível em configurações estratégicas.

A lógica central é que equilíbrio de Nash - um perfil de estratégia onde nenhum jogador pode melhorar seu payoff desviando unilateralmente, assumindo que estratégias de outros jogadores permanecem fixas - fornece ponto de estabilidade. Uma vez alcançado, ninguém tem incentivo para mudar, criando previsibilidade. Isto permite análise de situações competitivas, cooperativas, ou mistas.

Funciona porque:
- **Força antecipação de ações de outros:** Força você a pensar não apenas sobre suas opções, mas sobre o que outros são prováveis fazer.
- **Cria estabilidade:** Uma vez que equilíbrio é alcançado, ninguém tem incentivo para mudar estratégia sozinho.
- **Permite análise estratégica:** Fornece framework para analisar situações onde resultados dependem de múltiplos participantes.
- **Explica cooperação e competição:** Ajuda a entender quando cooperação emerge vs quando competição domina.

**Conceitos principais:**
- **Nash Equilibrium:** Perfil de estratégia onde nenhum jogador pode melhorar desviando unilateralmente
- **Estratégias dominantes:** Estratégias que são melhores independentemente do que outros fazem
- **Jogos cooperativos vs não cooperativos:** Se jogadores podem fazer acordos vinculantes vs não
- **Informação completa vs incompleta:** Se todos sabem payoffs e estratégias vs não

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Seu resultado depende não apenas de suas ações, mas também das ações de outros participantes.
* **Pressuposto 2:** Jogadores são racionais e agem para maximizar seus payoffs.
* **Pressuposto 3:** Jogadores sabem estrutura do jogo (estratégias disponíveis, payoffs) e que outros são racionais.
* **Pressuposto 4:** É possível identificar equilíbrios onde nenhum jogador quer desviar unilateralmente.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Situações competitivas:** Em situações competitivas onde você precisa antecipar ações de competidores.
- **Negociação:** Ao negociar, pensar sobre como outra parte pode responder a suas ofertas.
- **Estratégia de negócios:** Ao desenvolver estratégia de negócios, considerar como competidores podem responder.
- **Cooperação:** Ao considerar cooperação, analisar incentivos e quando cooperação é estável.
- **Políticas públicas:** Ao desenvolver políticas, considerar como diferentes atores podem responder estrategicamente.

**Domínios Típicos:** Estratégia, Economia, Negociação, Políticas, Cooperação, Competição.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Quando racionalidade perfeita não se aplica:** Se jogadores não são perfeitamente racionais ou têm racionalidade limitada, modelo pode não se aplicar.
- **Quando informação é muito incompleta:** Se informação sobre payoffs ou estratégias é muito incompleta, análise pode ser muito incerta.
- **Quando emoções dominam:** Se emoções ou fatores não racionais dominam decisões, modelo pode não capturar comportamento real.
- **Jogos muito complexos:** Se jogo é extremamente complexo com muitos jogadores e estratégias, análise pode ser impraticável.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Assumir racionalidade perfeita:** Assumir que todos são perfeitamente racionais quando na verdade têm racionalidade limitada.
- **Ignorar múltiplos equilíbrios:** Alguns jogos têm múltiplos equilíbrios - não reconhecer isso pode levar a previsões ambíguas.
- **Assumir que equilíbrios são socialmente ótimos:** Equilíbrios podem ser ineficientes (ex: Dilema do Prisioneiro) - não assumir que são socialmente ótimos.
- **Ignorar informação incompleta:** Assumir informação completa quando informação é incompleta, levando a análise incorreta.
- **Não considerar refinamentos:** Para jogos sequenciais, não considerar refinamentos como equilíbrio perfeito de subjogo.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está assumindo que todos são perfeitamente racionais.
  - Você não está reconhecendo quando há múltiplos equilíbrios.
  - Você está assumindo que equilíbrios são sempre socialmente ótimos.
  - Você está ignorando informação incompleta.

* **Evidência Prática:** 
  - Suas previsões estão incorretas porque você assumiu racionalidade perfeita.
  - Você não consegue prever comportamento porque há múltiplos equilíbrios possíveis.
  - Seus resultados são ineficientes porque você não considerou como melhorar além de equilíbrio.

## 5. Passos de Pensamento (Algoritmo)
1. **Defina jogadores, estratégias e payoffs:** Identifique quem são os jogadores, que estratégias cada um tem disponível, e quais são os payoffs para cada combinação de estratégias.

2. **Construa matriz de payoff ou forma extensiva:** Para jogos simultâneos, construa matriz de payoff. Para jogos sequenciais, construa árvore de forma extensiva.

3. **Identifique melhor resposta:** Para cada jogador, identifique melhor resposta para cada possível estratégia dos outros.

4. **Encontre equilíbrios de Nash:** Encontre perfis de estratégia onde todo jogador está jogando melhor resposta - estes são equilíbrios de Nash.

5. **Considere refinamentos (se sequencial):** Se jogo é sequencial, considere refinamentos como equilíbrio perfeito de subjogo, que requer que estratégias sejam equilíbrio de Nash em todo subjogo.

6. **Analise resultados:** Analise equilíbrios - são únicos ou múltiplos? São eficientes ou ineficientes? Qual é mais provável de ser jogado?

7. **Considere informação:** Determine se informação é completa (todos sabem payoffs e estratégias) ou incompleta (alguns jogadores têm informação privada).

8. **Avalie se cooperação é possível:** Determine se situação permite cooperação ou se é puramente competitiva. Analise incentivos para cooperar vs competir.

9. **Use para previsão e estratégia:** Use análise de teoria dos jogos para prever comportamento de outros e desenvolver sua própria estratégia.

10. **Monitore e ajuste:** Após implementar estratégia, monitore se outros se comportam como previsto. Ajuste análise se necessário.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao negociar um acordo importante e o resultado foi pensar sobre como outra parte provavelmente responderia a diferentes ofertas, permitindo estratégia mais efetiva.

* **Erro:** Ignorei este modelo ao tomar decisão competitiva e paguei o preço ao não antecipar como competidores responderiam, resultando em resultado pior que poderia ter sido.

* **Insight:** Descobri que teoria dos jogos é especialmente útil em situações onde há interdependência estratégica - onde seu resultado depende criticamente de ações de outros.

* **Aplicação prática:** Usei este modelo para melhorar tomada de decisão estratégica, descobrindo que pensar explicitamente sobre como outros podem responder resulta em decisões muito melhores do que focar apenas em suas próprias ações.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Nash Equilibrium]]
* [[Prisoner's Dilemma]]
* [[Cooperation]]
* [[Strategic Thinking]]
* [[Zero-Sum Games]]

**Fontes:**
* von Neumann, John; Morgenstern, Oskar - "Theory of Games and Economic Behavior" (1944)
* Nash, John - Nash Equilibrium
* Wikipedia - Game Theory
* Research on strategic decision-making

**Exemplos Notáveis:**
* **Dilema do Prisioneiro:** Equilíbrio é ambos confessarem - mesmo que ambos ficando silenciosos daria melhor resultado coletivo - porque confessar é estratégia dominante.
* **Jogos de coordenação:** Múltiplos equilíbrios de estratégia pura podem existir - escolhas dependem de expectativas sobre ações de outros.
