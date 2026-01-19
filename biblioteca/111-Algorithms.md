---
type: mental-model
title: "Algorithms"
category:
  - pensamento-geral
origin: Computer Science
author_reference: Computer science theory
domains:
  - ciência da computação
  - resolução de problemas
tags:
  - modelo-mental
  - pensamento
  - algoritmos
aliases:
  - Algoritmos
  - Algorithmic Thinking
  - Problem Solving
created: 2025-01-27
updated: 2025-01-27
---
# [[Algorithms]]

> **Teste de Pertinência:** *Você está tentando resolver problema e precisa de conjunto de instruções que tome entrada inicial e estado, execute número finito de operações e produza saída? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Algorithms (Algoritmos) são forma de computadores processarem dados. Conjunto de instruções que toma entrada inicial e estado, executa número finito de operações e produz saída. Algoritmo eventualmente terá ponto de parada. Algoritmo é sequência bem definida de passos computacionais que transforma entrada em saída.

**Explicação:**
Este modelo funciona porque reconhece que problemas complexos podem ser resolvidos através de quebrar em passos menores e mais gerenciáveis. Algoritmos fornecem estrutura sistemática para resolver problemas, garantindo que solução seja correta, eficiente, e possa ser executada de forma consistente. Isto funciona porque reconhece que através de definir claramente passos e condições, você pode resolver problemas de forma reproduzível e verificável.

A lógica central é que através de usar algoritmos, você pode resolver problemas de forma sistemática e eficiente. Isto funciona porque reconhece que diferentes abordagens algorítmicas (força bruta, dividir e conquistar, guloso, programação dinâmica, etc.) têm diferentes trade-offs em termos de complexidade de tempo, complexidade de espaço, e simplicidade.

Funciona porque:
- **Fornece estrutura sistemática:** Fornece estrutura sistemática para resolver problemas.
- **Garante correção:** Garante que solução seja correta se algoritmo é bem projetado.
- **Permite análise de eficiência:** Permite análise de eficiência - complexidade de tempo e espaço podem ser analisadas.
- **É reproduzível:** É reproduzível - mesmo algoritmo produz mesmo resultado para mesma entrada.

**Técnicas algorítmicas principais:**
- **Força Bruta:** Tentar tudo - sempre funciona, mas frequentemente muito lento.
- **Dividir e Conquistar:** Dividir problema em subproblemas menores, resolvê-los, então combinar.
- **Algoritmos Gulosos:** Fazer melhor escolha a cada passo esperando ótimo global.
- **Programação Dinâmica:** Lidar com subproblemas sobrepostos, armazenar resultados para evitar recomputação.
- **Backtracking / Branch and Bound:** Explorar escolhas, podar quando não mais viável.
- **Heurísticas / Aproximação:** Quando não existe algoritmo exato rápido - fornecer soluções "boas o suficiente".

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Problema pode ser definido claramente com entrada e saída bem especificadas.
* **Pressuposto 2:** Existe solução algorítmica para problema (pode ser aproximada se exata não existe).
* **Pressuposto 3:** Algoritmo tem ponto de parada bem definido.
* **Pressuposto 4:** Recursos computacionais (tempo, espaço) são limitados e devem ser considerados.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Resolver problemas:** Ao resolver problemas, usar pensamento algorítmico para quebrar problema em passos menores.
- **Otimizar soluções:** Ao otimizar soluções, analisar complexidade de tempo e espaço para escolher algoritmo mais eficiente.
- **Projetar sistemas:** Ao projetar sistemas, usar algoritmos apropriados para diferentes partes do sistema.
- **Aprender padrões:** Ao aprender padrões algorítmicos, reconhecer quando aplicar diferentes técnicas.

**Domínios Típicos:** Ciência da Computação, Programação, Resolução de Problemas, Otimização, Análise de Dados.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Problemas mal definidos:** Se problema não pode ser definido claramente, pode não ser apropriado para abordagem algorítmica.
- **Não considerar trade-offs:** Não considerar trade-offs - melhorar tempo pode aumentar espaço, ou vice-versa.
- **Ignorar contexto:** Ignorar contexto - algoritmo mais eficiente teoricamente pode não ser melhor na prática devido a constantes ou características de dados.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Usar algoritmo ineficiente:** Usar algoritmo ineficiente quando existe melhor opção.
- **Não analisar complexidade:** Não analisar complexidade de tempo e espaço antes de escolher algoritmo.
- **Ignorar casos extremos:** Ignorar casos extremos ou edge cases ao projetar algoritmo.
- **Não testar adequadamente:** Não testar algoritmo adequadamente em diferentes entradas.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está usando algoritmo ineficiente quando existe melhor opção.
  - Você não está analisando complexidade antes de escolher algoritmo.
  - Você está ignorando casos extremos ao projetar algoritmo.
  - Você não está testando algoritmo adequadamente.

* **Evidência Prática:** 
  - Sua solução está muito lenta ou usando muito espaço porque você escolheu algoritmo ineficiente.
  - Seu algoritmo falha em casos extremos porque você não os considerou.

## 5. Passos de Pensamento (Algoritmo)
1. **Entenda problema:** Leia cuidadosamente, talvez mais de uma vez. Certifique-se de saber exatamente qual entrada você recebe, qual saída precisa, e quaisquer restrições.

2. **Analise restrições e objetivos:** Analise tamanho de entrada, limites de tempo e memória, se soluções aproximadas são aceitáveis.

3. **Brainstorm abordagens possíveis:** Pense em diferentes estratégias gerais - força bruta, dividir e conquistar, guloso, programação dinâmica, etc.

4. **Selecione abordagem baseado em eficiência:** Avalie cada ideia em termos de complexidade de tempo, complexidade de espaço, simplicidade vs correção.

5. **Projete algoritmo:** Descreva em pseudocódigo primeiro. Quebre em passos claros ou módulos (funções). Use estruturas de dados apropriadas.

6. **Analise algoritmo:** Calcule pior caso, caso médio de tempo de execução. Calcule uso de espaço. Considere custos ocultos.

7. **Implemente:** Codifique solução cuidadosamente. Use modularidade e nomes de variáveis claros.

8. **Teste em entradas pequenas:** Rastreie manualmente algoritmo em casos simples e extremos. Escreva casos de teste.

9. **Benchmark e otimize:** Se está muito lento ou usando muito espaço, identifique gargalos, use estruturas de dados ou algoritmos mais rápidos.

10. **Analise trade-offs de eficiência:** Às vezes melhorar tempo aumenta espaço, ou vice-versa. Seja consciente de classes de complexidade.

11. **Reflita e aprenda:** Após resolver, pergunte o que poderia ser melhorado? Outra abordagem poderia ser mais rápida ou simples?

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao resolver problema e o resultado foi usar pensamento algorítmico, resultando em solução muito mais sistemática e eficiente.

* **Erro:** Ignorei este modelo ao resolver problema e paguei o preço ao usar algoritmo ineficiente, resultando em solução muito lenta.

* **Insight:** Descobri que algoritmos são especialmente importantes para resolver problemas de forma sistemática - diferentes abordagens têm diferentes trade-offs em termos de eficiência.

* **Aplicação prática:** Usei este modelo para melhorar resolução de problemas, descobrindo que usar pensamento algorítmico resulta em muito mais sistemáticas e eficientes soluções.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Data Structures]]
* [[Recursion]]
* [[Complexity Analysis]]
* [[Problem Solving]]
* [[Efficiency]]

**Fontes:**
* Computer science theory
* Wikipedia - Algorithm
* Research on algorithmic problem solving

**Exemplos Notáveis:**
* **Ordenação:** Algoritmos como Merge Sort (dividir e conquistar) vs Bubble Sort (força bruta) - diferentes complexidades de tempo.
* **Busca:** Algoritmos como Binary Search (O(log n)) vs Linear Search (O(n)) - diferentes eficiências.
