---
type: mental-model
title: "Standard Deviation"
category:
  - pensamento-geral
origin: Statistics
author_reference: Statistical theory
domains:
  - estatística
  - análise de dados
tags:
  - modelo-mental
  - pensamento
  - desvio padrão
aliases:
  - Desvio Padrão
  - Variability
  - Spread
created: 2025-01-27
updated: 2025-01-27
---
# [[Standard Deviation]]

> **Teste de Pertinência:** *Você está analisando conjunto de dados e precisa medir espalhamento de valores e quão longe de "normal" estes valores estão? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Standard Deviation (Desvio Padrão) é usado em estatística para medir espalhamento de valores e quão longe de "normal" estes valores estão. Ao encontrar Desvio Padrão, podemos saber o que é "normal" para dado conjunto de valores, e o que está acima ou abaixo desta faixa normal. Desvio padrão é raiz quadrada de variância - média das diferenças quadradas da média.

**Explicação:**
Este modelo funciona porque reconhece que apenas saber média de conjunto de dados não é suficiente - você também precisa saber quão espalhados estão os valores. Desvio padrão fornece medida de variabilidade ou dispersão. Se desvio padrão é pequeno, pontos de dados estão próximos da média; se grande, estão mais espalhados. Isto funciona porque reconhece que em distribuição normal (em forma de sino), cerca de 68% dos valores caem dentro de ±1 desvio padrão da média, cerca de 95% dentro de ±2 desvios padrão.

A lógica central é que através de usar desvio padrão junto com média, você obtém visão mais completa de distribuição de dados. Isto funciona porque reconhece que desvio padrão tem mesmas unidades que dados (ao contrário de variância que tem unidades ao quadrado), tornando mais fácil de interpretar.

Funciona porque:
- **Mede variabilidade:** Fornece medida de variabilidade ou dispersão de dados.
- **Tem mesmas unidades:** Tem mesmas unidades que dados (ao contrário de variância), tornando mais fácil de interpretar.
- **Usado com média:** Frequentemente usado com média para descrever distribuição.
- **Fornece regras práticas:** Em distribuição normal, fornece regras práticas (68% dentro de ±1σ, 95% dentro de ±2σ).

**Fórmulas:**
- **Variância populacional:** σ² = Σ (Xi - μ)² / N
- **Desvio padrão populacional:** σ = √σ²
- **Variância amostral (não viesada):** s² = Σ (xi - x̄)² / (n-1)
- **Desvio padrão amostral:** s = √s²

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Você tem conjunto de dados numéricos.
* **Pressuposto 2:** Você quer medir variabilidade ou dispersão de dados.
* **Pressuposto 3:** Média é medida relevante de centro (pode não ser apropriado se distribuição é muito assimétrica).
* **Pressuposto 4:** Você pode calcular diferenças de valores da média e elevar ao quadrado.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Medir variabilidade:** Ao medir variabilidade ou dispersão de dados, usar desvio padrão junto com média.
- **Entender distribuição:** Ao entender distribuição de dados, usar desvio padrão para entender espalhamento.
- **Identificar outliers:** Ao identificar outliers, valores que estão a mais de 2 ou 3 desvios padrão da média podem ser considerados outliers.
- **Comparar variabilidade:** Ao comparar variabilidade entre diferentes conjuntos de dados, usar desvio padrão (ou coeficiente de variação se médias diferem muito).

**Domínios Típicos:** Estatística, Análise de Dados, Controle de Qualidade, Pesquisa, Ciência.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Distribuições muito assimétricas:** Se distribuição é muito assimétrica, média e desvio padrão podem não ser medidas apropriadas - mediana e IQR podem ser melhores.
- **Outliers extremos:** Se há outliers extremos, desvio padrão pode ser muito afetado - IQR pode ser mais robusto.
- **Não considerar contexto:** Não considerar contexto - desvio padrão sozinho não conta história completa.
- **Assumir normalidade:** Assumir que distribuição é normal quando pode não ser - regras práticas (68%, 95%) só se aplicam a distribuições normais.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Assumir normalidade:** Assumir que distribuição é normal quando pode não ser - regras práticas só se aplicam a distribuições normais.
- **Ignorar outliers:** Ignorar que outliers extremos podem afetar desvio padrão significativamente.
- **Usar sem considerar assimetria:** Usar desvio padrão sem considerar se distribuição é assimétrica - mediana e IQR podem ser melhores.
- **Não considerar contexto:** Não considerar contexto - desvio padrão sozinho não conta história completa.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está assumindo que distribuição é normal quando pode não ser.
  - Você não está considerando se distribuição é assimétrica.
  - Você está ignorando outliers que podem afetar desvio padrão.
  - Você não está considerando contexto ao interpretar desvio padrão.

* **Evidência Prática:** 
  - Suas interpretações estão incorretas porque você assumiu normalidade quando distribuição não era normal.
  - Você não está capturando variabilidade real porque ignorou assimetria ou outliers.

## 5. Passos de Pensamento (Algoritmo)
1. **Obtenha conjunto de dados:** Obtenha conjunto de dados numéricos.

2. **Calcule média:** Calcule média (μ para população, x̄ para amostra).

3. **Calcule diferenças:** Calcule diferenças de cada valor da média.

4. **Eleve ao quadrado:** Eleve diferenças ao quadrado.

5. **Calcule variância:** Calcule variância:
   - População: σ² = Σ (Xi - μ)² / N
   - Amostra: s² = Σ (xi - x̄)² / (n-1)

6. **Calcule desvio padrão:** Calcule desvio padrão como raiz quadrada de variância:
   - População: σ = √σ²
   - Amostra: s = √s²

7. **Interprete:** Interprete desvio padrão:
   - Pequeno: pontos de dados estão próximos da média
   - Grande: pontos de dados estão mais espalhados
   - Em distribuição normal: ~68% dentro de ±1σ, ~95% dentro de ±2σ

8. **Considere distribuição:** Considere se distribuição é normal ou assimétrica - se muito assimétrica, mediana e IQR podem ser melhores.

9. **Considere outliers:** Considere se há outliers que podem afetar desvio padrão - IQR pode ser mais robusto.

10. **Use junto com média:** Use desvio padrão junto com média para obter visão mais completa de distribuição.

11. **Monitore e ajuste:** Após calcular desvio padrão, monitore se está funcionando como esperado. Ajuste se necessário.

12. **Use apropriadamente:** Use desvio padrão para medir variabilidade, mas reconheça limitações - pode não ser apropriado se distribuição é muito assimétrica ou há outliers extremos.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao analisar dados e o resultado foi usar desvio padrão junto com média, resultando em visão muito mais completa de distribuição de dados.

* **Erro:** Ignorei este modelo ao analisar dados e paguei o preço ao focar apenas em média, ignorando variabilidade, resultando em análise incompleta.

* **Insight:** Descobri que desvio padrão é especialmente importante para entender variabilidade - apenas saber média não é suficiente, você também precisa saber quão espalhados estão os valores.

* **Aplicação prática:** Usei este modelo para melhorar análise de dados, descobrindo que usar desvio padrão junto com média resulta em muito mais completa compreensão de distribuição e melhor capacidade de identificar padrões ou anomalias.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Normal Distribution]]
* [[Variance]]
* [[Mean Median Mode]]
* [[Variability]]
* [[Statistical Dispersion]]

**Fontes:**
* Statistical theory
* Wikipedia - Standard deviation
* Research on statistics and data analysis

**Exemplos Notáveis:**
* **Distribuição normal:** Em distribuição normal, cerca de 68% dos valores caem dentro de ±1 desvio padrão da média, cerca de 95% dentro de ±2 desvios padrão.
* **Identificar outliers:** Valores que estão a mais de 2 ou 3 desvios padrão da média podem ser considerados outliers.
