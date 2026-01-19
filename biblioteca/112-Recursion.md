---
type: mental-model
title: "Recursion"
category:
  - pensamento-geral
origin: Computer Science, Mathematics
author_reference: Computer science theory
domains:
  - ciência da computação
  - matemática
tags:
  - modelo-mental
  - pensamento
  - recursão
aliases:
  - Recursão
  - Recursive Thinking
  - Recursive Function
created: 2025-01-27
updated: 2025-01-27
---
# [[Recursion]]

> **Teste de Pertinência:** *Você está tentando resolver problema que pode ser naturalmente quebrado em subproblemas menores e similares, e precisa de função que chame a si mesma? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Recursion (Recursão) é quebrar problema em passos simples chamados funções. Essas funções podem chamar a si mesmas. Função recursiva é função que chama a si mesma - diretamente ou via outra função. Você usa recursão quando problema pode ser naturalmente quebrado em subproblemas menores e similares (dividir e conquistar, travessias de árvore/grafo, etc.).

**Explicação:**
Este modelo funciona porque reconhece que muitos problemas têm estrutura recursiva natural - solução para problema maior pode ser expressa em termos de soluções para versões menores do mesmo problema. Cada função recursiva tipicamente tem duas partes-chave: **Base Case (Caso Base)** - forma mais simples do problema que pode ser resolvida diretamente sem mais recursão, diz à função recursiva quando parar, prevenindo loops infinitos; **Recursive Case (Caso Recursivo)** - parte que quebra problema original em uma ou mais instâncias menores do mesmo problema, cada chamada recursiva deve mover em direção a caso base.

A lógica central é que através de usar recursão, você pode resolver problemas complexos de forma elegante e concisa. Isto funciona porque reconhece que estrutura recursiva de problema reflete estrutura recursiva de solução. Funciona especialmente bem para problemas que têm estrutura hierárquica ou podem ser naturalmente divididos em subproblemas similares.

Funciona porque:
- **Reflete estrutura natural:** Reflete estrutura recursiva natural de muitos problemas.
- **É elegante e conciso:** Permite soluções elegantes e concisas para problemas complexos.
- **Facilita divisão:** Facilita dividir problema em subproblemas menores e similares.
- **É matematicamente elegante:** É matematicamente elegante - muitas definições matemáticas são recursivas.

**Componentes principais:**
- **Base Case:** Caso mais simples que pode ser resolvido diretamente.
- **Recursive Case:** Quebra problema em instâncias menores do mesmo problema.
- **Call Stack:** Cada chamada recursiva cria novo frame na pilha, armazenando argumentos, variáveis locais, e onde retornar.

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Problema pode ser naturalmente quebrado em subproblemas menores e similares.
* **Pressuposto 2:** Existe caso base que pode ser resolvido diretamente sem recursão.
* **Pressuposto 3:** Cada passo recursivo move em direção a caso base (prova de terminação).
* **Pressuposto 4:** Recursos computacionais (profundidade de pilha, memória) são suficientes para recursão.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Problemas com estrutura recursiva:** Ao resolver problemas com estrutura recursiva natural (árvores, grafos, fatorial, etc.), usar recursão.
- **Dividir e conquistar:** Ao usar técnica de dividir e conquistar, recursão é natural.
- **Travessias de árvore/grafo:** Ao fazer travessias de árvore ou grafo, recursão é frequentemente mais elegante.
- **Definições matemáticas recursivas:** Ao implementar definições matemáticas recursivas, usar recursão.

**Domínios Típicos:** Ciência da Computação, Programação, Matemática, Estruturas de Dados, Algoritmos.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Sem caso base adequado:** Sem caso base adequado, recursão nunca termina - levando a recursão infinita ou erros de estouro de pilha.
- **Profundidade muito grande:** Se profundidade de recursão é muito grande, pode causar estouro de pilha.
- **Pode ser ineficiente:** Recursão pode ser ineficiente em termos de espaço (pilha) e tempo (overhead de chamadas de função).
- **Iteração pode ser melhor:** Para alguns problemas, iteração pode ser mais eficiente ou mais clara que recursão.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Esquecer caso base:** Esquecer de definir caso base adequado - recursão nunca termina.
- **Caso base não alcançável:** Caso base não é alcançável - cada passo recursivo não move em direção a caso base.
- **Profundidade muito grande:** Usar recursão quando profundidade é muito grande, causando estouro de pilha.
- **Não considerar eficiência:** Não considerar que recursão pode ser ineficiente - iteração pode ser melhor.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está esquecendo de definir caso base adequado.
  - Você não está garantindo que cada passo recursivo move em direção a caso base.
  - Você está usando recursão quando profundidade é muito grande.
  - Você não está considerando eficiência - iteração pode ser melhor.

* **Evidência Prática:** 
  - Seu programa entra em loop infinito ou estoura pilha porque você não definiu caso base adequado.
  - Sua solução é ineficiente porque você usou recursão quando iteração seria melhor.

## 5. Passos de Pensamento (Algoritmo)
1. **Identifique versão mais simples:** Identifique versão mais simples do problema - quais entradas permitem que você responda imediatamente?

2. **Defina caso(s) base:** Defina caso(s) base - quais condições devem causar retorno direto?

3. **Defina caso recursivo:** Defina caso recursivo - como você reduz ou simplifica problema? (Geralmente modificando argumentos.)

4. **Garanta progressão:** Garanta que cada passo recursivo move em direção a caso base - prova de terminação.

5. **Combine resultados:** Combine resultados (se necessário) de chamadas recursivas para construir resposta ao problema original.

6. **Verifique terminação:** Verifique que recursão termina - caso base é alcançável e cada passo move em direção a ele.

7. **Considere eficiência:** Considere eficiência - recursão pode ser ineficiente em termos de espaço (pilha) e tempo. Considere se iteração seria melhor.

8. **Teste em casos pequenos:** Teste em casos pequenos - rastreie manualmente para verificar que funciona corretamente.

9. **Monitore profundidade:** Monitore profundidade de recursão - se muito grande, considere iteração ou otimização (ex: tail recursion).

10. **Use apropriadamente:** Use recursão quando problema tem estrutura recursiva natural, mas reconheça limitações - pode ser ineficiente ou causar estouro de pilha se profundidade é muito grande.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao resolver problema com estrutura recursiva e o resultado foi usar recursão, resultando em solução muito mais elegante e concisa.

* **Erro:** Ignorei este modelo ao resolver problema e paguei o preço ao esquecer caso base, resultando em recursão infinita e estouro de pilha.

* **Insight:** Descobri que recursão é especialmente importante para problemas com estrutura recursiva natural - reflete estrutura do problema na estrutura da solução.

* **Aplicação prática:** Usei este modelo para melhorar programação, descobrindo que usar recursão quando apropriado resulta em muito mais elegantes e concisas soluções para problemas complexos.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Algorithms]]
* [[Data Structures]]
* [[Divide and Conquer]]
* [[Base Case]]
* [[Call Stack]]

**Fontes:**
* Computer science theory
* Wikipedia - Recursion
* Research on recursive algorithms and problem solving

**Exemplos Notáveis:**
* **Fatorial:** função factorial(n): se n == 0 retorna 1 (caso base), senão retorna n * factorial(n-1) (caso recursivo).
* **Travessia de árvore:** Se nó é null (caso base), retorna; senão atravessa filhos recursivamente.
