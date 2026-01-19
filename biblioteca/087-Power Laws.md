---
type: mental-model
title: "Power Laws"
category:
  - pensamento-geral
origin: Mathematics, Statistics, Vilfredo Pareto
author_reference: Pareto, Vilfredo - Pareto distribution
domains:
  - matemática
  - estatística
  - distribuições
  - desigualdade
tags:
  - modelo-mental
  - pensamento
  - leis de potência
  - distribuição de pareto
  - 80/20
aliases:
  - Leis de Potência
  - Power Law Distribution
  - Pareto Distribution
  - 80/20 Rule
created: 2025-01-27
updated: 2025-01-27
---
# [[Power Laws]]

> **Teste de Pertinência:** *Você está analisando distribuição onde poucos itens têm valores muito grandes e muitos itens têm valores pequenos, ou está tentando entender padrões de desigualdade ou concentração? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Power Laws (Leis de Potência) são distribuições de probabilidade onde probabilidade de valor x é proporcional a x^(-α), para x ≥ x_min, onde α > 1 é expoente. Distribuições de lei de potência têm cauda "pesada" ou "gorda" - valores extremos são mais prováveis que sob distribuições exponenciais ou gaussianas. Também têm invariância de escala - multiplicar x por constante reescala distribuição mas não muda sua forma (até normalização).

**Explicação:**
Este modelo funciona porque reconhece que muitos fenômenos do mundo real seguem distribuições de lei de potência em vez de distribuições normais. Em redes scale-free, graus de nós seguem distribuição de lei de potência - muitos nós têm poucas conexões, mas poucos nós (hubs) têm muitas conexões. Princípio 80/20 de Pareto é instância específica de distribuição de lei de potência - aproximadamente 80% dos efeitos vêm de 20% das causas (não precisa ser exatamente 80/20, depende do expoente).

A lógica central é que através de reconhecer que distribuição segue lei de potência, você pode entender padrões de desigualdade e concentração. Em desigualdade econômica, renda ou riqueza frequentemente seguem caudas de Pareto - pequena fração de pessoas detém grande fração de riqueza. Em redes, poucos hubs têm maioria das conexões. Isto significa que focar em poucos itens grandes pode ter impacto desproporcional.

Funciona porque:
- **Captura desigualdade:** Captura padrões onde há grande desigualdade - poucos itens grandes, muitos itens pequenos.
- **Explica concentração:** Explica por que recursos, conexões, ou influência frequentemente se concentram em poucos itens.
- **Tem invariância de escala:** Invariância de escala significa que padrão se mantém em diferentes escalas.
- **Tem cauda pesada:** Cauda pesada significa que valores extremos são mais prováveis que em distribuições normais.

**Princípio 80/20 (Pareto):**
- Nomeado após Vilfredo Pareto, que observou que cerca de 80% da terra era detida por aproximadamente 20% da população
- Regra "80/20" é instância específica de distribuição de lei de potência geral
- Não precisa ser exatamente 80/20 - depende do expoente da lei de potência

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Distribuição segue lei de potência - probabilidade é proporcional a x^(-α).
* **Pressuposto 2:** Há grande desigualdade - poucos itens grandes, muitos itens pequenos.
* **Pressuposto 1:** Padrão tem invariância de escala - se mantém em diferentes escalas.
* **Pressuposto 4:** Valores extremos são mais prováveis que em distribuições normais (cauda pesada).

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Análise de desigualdade:** Ao analisar padrões de desigualdade (riqueza, renda, influência), reconhecer que podem seguir leis de potência.
- **Análise de redes:** Ao analisar redes, reconhecer que redes scale-free têm distribuições de grau que seguem leis de potência.
- **Focar em poucos itens grandes:** Ao priorizar, reconhecer que poucos itens grandes frequentemente têm impacto desproporcional (princípio 80/20).
- **Entender concentração:** Ao entender concentração de recursos, conexões ou influência, aplicar princípios de leis de potência.
- **Aplicar princípio 80/20:** Ao aplicar princípio 80/20, reconhecer que é instância de distribuição de lei de potência.

**Domínios Típicos:** Estatística, Análise de Redes, Economia, Priorização, Desigualdade.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Quando distribuição não é de lei de potência:** Se distribuição não segue lei de potência (ex: é normal), modelo não se aplica.
- **Ajuste adequado:** Ajustar leis de potência adequadamente pode ser complicado - você frequentemente precisa ignorar partes de baixo grau da distribuição (ajuste de cauda).
- **Não assumir sempre:** Não assumir que todas as distribuições são de lei de potência - muitas são melhor ajustadas por outras distribuições de cauda pesada como log-normal.
- **Não ignorar limitações:** Não ignorar que redes verdadeiramente scale-free (com distribuições de grau seguindo leis de potência puras sobre amplas faixas) são raras.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Assumir sempre 80/20:** Assumir que princípio 80/20 sempre se aplica exatamente, quando proporções podem variar.
- **Ignorar que não é sempre lei de potência:** Assumir que todas as distribuições desiguais são leis de potência quando podem ser outras distribuições de cauda pesada.
- **Não verificar adequadamente:** Não verificar adequadamente se distribuição realmente segue lei de potência antes de aplicar modelo.
- **Ignorar limitações:** Ignorar que ajustar leis de potência adequadamente pode ser complicado e requer cuidado.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está assumindo que princípio 80/20 sempre se aplica exatamente.
  - Você não está verificando se distribuição realmente segue lei de potência.
  - Você está assumindo que todas as distribuições desiguais são leis de potência.
  - Você não está considerando limitações de ajuste.

* **Evidência Prática:** 
  - Suas análises estão incorretas porque você assumiu lei de potência quando não era apropriado.
  - Você não está capturando comportamento real porque distribuição não é de lei de potência.

## 5. Passos de Pensamento (Algoritmo)
1. **Avalie se lei de potência é apropriada:** Avalie se distribuição segue lei de potência - há grande desigualdade? Cauda pesada? Use testes ou visualizações (gráficos log-log).

2. **Identifique padrão de desigualdade:** Identifique se há padrão onde poucos itens têm valores muito grandes e muitos itens têm valores pequenos.

3. **Estime expoente:** Se lei de potência é apropriada, estime expoente α - isto determina grau de desigualdade.

4. **Aplique princípio 80/20:** Se aplicável, aplique princípio 80/20 - reconheça que poucos itens grandes frequentemente têm impacto desproporcional.

5. **Foque em poucos itens grandes:** Ao priorizar, foque em poucos itens grandes que têm maior impacto (seguindo princípio 80/20).

6. **Reconheça invariância de escala:** Reconheça que leis de potência têm invariância de escala - padrão se mantém em diferentes escalas.

7. **Considere cauda pesada:** Reconheça que leis de potência têm cauda pesada - valores extremos são mais prováveis que em distribuições normais.

8. **Aplique a análise de redes:** Se aplicável, aplique a análise de redes - redes scale-free têm distribuições de grau que seguem leis de potência.

9. **Monitore e ajuste:** Após aplicar modelo, monitore se está funcionando como esperado. Ajuste se necessário.

10. **Use apropriadamente:** Use leis de potência quando apropriado, mas não assuma que sempre se aplicam - verifique primeiro.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao priorizar esforços e o resultado foi aplicar princípio 80/20, focando em poucos itens grandes que tinham maior impacto, resultando em muito melhor uso de recursos.

* **Erro:** Ignorei este modelo ao analisar distribuição e paguei o preço ao assumir distribuição normal quando era de lei de potência, resultando em análises incorretas.

* **Insight:** Descobri que leis de potência são especialmente importantes para entender desigualdade e concentração - poucos itens grandes frequentemente têm impacto desproporcional.

* **Aplicação prática:** Usei este modelo para melhorar priorização, descobrindo que reconhecer padrões de lei de potência e focar em poucos itens grandes resulta em muito melhor uso de recursos e impacto.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Pareto Principle]]
* [[80/20 Rule]]
* [[Scale-Free Networks]]
* [[Inequality]]
* [[Heavy Tails]]

**Fontes:**
* Pareto, Vilfredo - Pareto distribution
* Wikipedia - Power Law
* Research on power laws and scale-free networks

**Exemplos Notáveis:**
* **Princípio 80/20:** Aproximadamente 80% dos efeitos vêm de 20% das causas - instância de distribuição de lei de potência.
* **Redes scale-free:** Redes onde graus de nós seguem distribuição de lei de potência - muitos nós têm poucas conexões, poucos hubs têm muitas.
