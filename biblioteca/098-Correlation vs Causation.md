---
type: mental-model
title: "Correlation vs Causation"
category:
  - pensamento-geral
origin: Statistics
author_reference: Statistical theory
domains:
  - estatística
  - pensamento crítico
tags:
  - modelo-mental
  - pensamento
  - correlação
  - causalidade
aliases:
  - Correlação vs Causalidade
  - Spurious Correlation
  - Correlation Does Not Imply Causation
created: 2025-01-27
updated: 2025-01-27
---
# [[Correlation vs Causation]]

> **Teste de Pertinência:** *Você está observando que duas variáveis se movem juntas e precisa determinar se uma causa a outra, ou se há relação causal? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Correlation (Correlação) é medida estatística que descreve extensão em que duas variáveis se movem juntas. Se uma aumenta quando outra aumenta, isso é correlação positiva; se uma aumenta enquanto outra diminui, isso é correlação negativa. Correlação não nos diz por que variáveis se movem juntas. Causation (Causalidade) significa que mudança em uma variável (causa) produz diretamente mudança em outra (efeito). Afirmações causais implicam que alterar causa alterará efeito, dado que tudo mais permanece igual.

**Explicação:**
Este modelo funciona porque reconhece que correlação não implica causalidade - pedra angular em pensamento crítico e raciocínio estatístico. **Spurious Correlation** (Correlação Espúria) é associação estatística forte entre duas variáveis que não é devido a relação causal. Geralmente causada por: variável terceira (lurking/confounding) influenciando ambas variáveis; coincidência ou artefato de dados (ex: observações não independentes, tendências comuns); relações matemáticas como razões compartilhando componente comum.

A lógica central é que através de reconhecer diferença entre correlação e causalidade, você pode evitar erros comuns ao inferir causalidade de correlação. Isto funciona porque reconhece que apenas porque duas variáveis se movem juntas não significa que uma causa outra - pode haver variável terceira influenciando ambas, ou pode ser coincidência.

Funciona porque:
- **Reconhece diferença:** Reconhece diferença entre correlação (variáveis se movem juntas) e causalidade (uma causa outra).
- **Evita erros comuns:** Evita erros comuns como assumir causalidade de correlação.
- **Identifica correlações espúrias:** Identifica correlações espúrias - associações estatísticas fortes que não são devido a relação causal.
- **Fornece estrutura para investigar causalidade:** Fornece estrutura para investigar causalidade adequadamente.

**Falácias comuns:**
- **Cum hoc ergo propter hoc:** Assumir que duas variáveis co-ocorrentes têm ligação causal.
- **Post hoc ergo propter hoc:** Inferir causalidade baseado em sequência em vez de qualquer ligação real.
- **Third-cause fallacy:** Ignorar variável externa que causa tanto A quanto B.
- **Reverse causation:** Direção que você está assumindo (A causa B) é na verdade invertida - B causa A.
- **Illusory correlations:** Laços estatísticos fortes que surgem por acaso ou artefato em vez de qualquer relação real.

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Você está observando correlação entre duas variáveis.
* **Pressuposto 2:** Você quer determinar se há relação causal entre variáveis.
* **Pressuposto 3:** Você reconhece que correlação não implica causalidade.
* **Pressuposto 4:** Você está disposto a investigar causalidade adequadamente antes de inferir causalidade.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Interpretar correlações:** Ao interpretar correlações, reconhecer que correlação não implica causalidade e investigar adequadamente antes de inferir causalidade.
- **Evitar erros comuns:** Ao evitar erros comuns, não assumir causalidade de correlação sem investigar adequadamente.
- **Investigar causalidade:** Ao investigar causalidade, usar métodos apropriados (experimentos randomizados, controle de confundidores, precedência temporal).
- **Tomar decisões informadas:** Ao tomar decisões informadas, não confundir correlação com causalidade.

**Domínios Típicos:** Estatística, Pesquisa, Pensamento Crítico, Políticas Públicas, Negócios.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Não ignorar correlações:** Não ignorar correlações completamente - podem ser úteis para identificar potenciais relações causais para investigar.
- **Não assumir que correlação nunca indica causalidade:** Não assumir que correlação nunca indica causalidade - pode indicar, mas precisa investigar adequadamente.
- **Não usar como desculpa para ignorar dados:** Não usar como desculpa para ignorar dados - correlações ainda podem ser informativas mesmo se não indicam causalidade direta.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Assumir causalidade de correlação:** Assumir que correlação implica causalidade sem investigar adequadamente.
- **Ignorar variáveis terceiras:** Ignorar variáveis terceiras que podem estar influenciando ambas variáveis.
- **Confundir correlação com causalidade:** Confundir correlação com causalidade - apenas porque duas variáveis se movem juntas não significa que uma causa outra.
- **Não investigar adequadamente:** Não investigar causalidade adequadamente antes de inferir causalidade.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está assumindo que correlação implica causalidade.
  - Você não está investigando causalidade adequadamente antes de inferir causalidade.
  - Você está ignorando variáveis terceiras que podem estar influenciando ambas variáveis.
  - Você está confundindo correlação com causalidade.

* **Evidência Prática:** 
  - Suas inferências estão incorretas porque você assumiu causalidade de correlação.
  - Você não está capturando relação real porque ignorou variáveis terceiras ou outros fatores.

## 5. Passos de Pensamento (Algoritmo)
1. **Identifique correlação:** Identifique correlação entre duas variáveis - elas se movem juntas?

2. **Reconheça que correlação não implica causalidade:** Reconheça que correlação não implica causalidade - apenas porque duas variáveis se movem juntas não significa que uma causa outra.

3. **Investigue causalidade adequadamente:** Se você quer determinar se há relação causal, investigue adequadamente:
   - **Procure teoria ou mecanismo:** Faz sentido biologicamente, socialmente, economicamente, etc.?
   - **Controle para confundidores:** Use técnicas estatísticas (regressão, estratificação) para ajustar para variáveis que podem afetar tanto A quanto B.
   - **Precedência temporal:** Causa deve preceder efeito. Útil em estudos longitudinais.
   - **Use experimentos randomizados:** Melhor forma de estabelecer causalidade (atribuir A aleatoriamente para ver efeito em B).
   - **Use frameworks de inferência causal:** Ferramentas como DAGs (Directed Acyclic Graphs), ou critérios como critérios de Bradford Hill da epidemiologia.

4. **Identifique correlações espúrias:** Identifique correlações espúrias - associações estatísticas fortes que não são devido a relação causal. Geralmente causadas por variável terceira, coincidência, ou artefato de dados.

5. **Evite falácias comuns:** Evite falácias comuns:
   - Cum hoc ergo propter hoc (assumir ligação causal de co-ocorrência)
   - Post hoc ergo propter hoc (inferir causalidade baseado em sequência)
   - Third-cause fallacy (ignorar variável externa)
   - Reverse causation (direção invertida)
   - Illusory correlations (correlações por acaso)

6. **Use correlações apropriadamente:** Use correlações para identificar potenciais relações causais para investigar, mas não assuma causalidade sem investigar adequadamente.

7. **Monitore e ajuste:** Após fazer inferência, monitore se está funcionando como esperado. Ajuste se necessário.

8. **Use apropriadamente:** Use modelo para distinguir entre correlação e causalidade e investigar causalidade adequadamente antes de inferir causalidade.

9. **Eduque outros:** Eduque outros sobre diferença entre correlação e causalidade para ajudá-los a fazer inferências mais precisas.

10. **Reconheça limitações:** Reconheça que estabelecer causalidade pode ser difícil e requer métodos apropriados - correlação sozinha não é suficiente.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao interpretar correlações e o resultado foi reconhecer que correlação não implica causalidade e investigar adequadamente antes de inferir causalidade, resultando em inferências muito mais precisas.

* **Erro:** Ignorei este modelo ao interpretar correlação e paguei o preço ao assumir causalidade de correlação sem investigar adequadamente, resultando em inferências incorretas.

* **Insight:** Descobri que correlação vs causalidade é especialmente importante para entender que apenas porque duas variáveis se movem juntas não significa que uma causa outra - pode haver variável terceira ou coincidência.

* **Aplicação prática:** Usei este modelo para melhorar interpretação de dados, descobrindo que distinguir entre correlação e causalidade e investigar causalidade adequadamente resulta em muito mais precisas inferências e decisões melhores.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Spurious Correlation]]
* [[Causal Inference]]
* [[Statistical Thinking]]
* [[Critical Thinking]]
* [[Confounding Variables]]

**Fontes:**
* Statistical theory
* Wikipedia - Correlation Does Not Imply Causation
* Research on causal inference and statistics

**Exemplos Notáveis:**
* **Vendas de sorvete e afogamentos:** Vendas de sorvete e incidentes de afogamento correlacionam porque temperatura impulsiona ambos.
* **Taxas de divórcio e consumo de margarina:** Taxas de divórcio em Maine são altamente correlacionadas com consumo de margarina nos EUA, mas não há ligação causal plausível.
* **Filmes de Nicholas Cage e afogamentos:** Lançamentos de filmes de Nicholas Cage e afogamentos em piscinas correlacionam ao longo do tempo - pura coincidência.
