---
type: mental-model
title: "Bayes Theorem"
category:
  - pensamento-geral
origin: Mathematics, Statistics, Thomas Bayes
author_reference: Bayes, Thomas - Bayes' Theorem
domains:
  - matemática
  - estatística
  - probabilidade
tags:
  - modelo-mental
  - pensamento
  - teorema de bayes
aliases:
  - Teorema de Bayes
  - Bayesian Inference
  - Bayesian Reasoning
created: 2025-01-27
updated: 2025-01-27
---
# [[Bayes Theorem]]

> **Teste de Pertinência:** *Você está atualizando suas crenças à luz de nova evidência, ou precisa calcular probabilidade condicional de hipótese dado evidência? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Bayes' Theorem (Teorema de Bayes) é resultado fundamental em teoria de probabilidade que explica como atualizar suas crenças à luz de nova evidência. **Prior Probability (P(H))** é sua crença inicial em hipótese H antes de observar qualquer nova evidência. **Likelihood (P(E | H))** é probabilidade de observar evidência E, assumindo que hipótese H é verdadeira. **Marginal Probability (P(E))** é probabilidade total de observar evidência E, sob todas as hipóteses possíveis. **Posterior Probability (P(H | E))** é crença atualizada em hipótese H após considerar evidência E.

**Explicação:**
Este modelo funciona porque reconhece que através de começar com sua crença prévia, observar nova evidência, e então atualizar sua crença baseado em quão provável evidência é dado hipótese, você pode fazer inferências mais precisas. Processo: Comece com seu prior, o que você acredita antes de ver quaisquer novos dados. Observe nova evidência E. Atualize sua crença: Quão provável é H dado aquela evidência? Isso é seu posterior. Itere: Se mais evidência chega, posterior se torna seu novo prior.

A lógica central é que através de usar Teorema de Bayes, você pode atualizar suas crenças sistematicamente à luz de nova evidência. Isto é especialmente poderoso em campos como diagnóstico médico, aprendizado de máquina, tomada de decisão sob incerteza, e inferência científica. Funciona porque reconhece que você deve considerar não apenas quão provável evidência é dado hipótese, mas também probabilidade prévia de hipótese.

Funciona porque:
- **Atualiza crenças sistematicamente:** Atualiza crenças sistematicamente à luz de nova evidência.
- **Considera probabilidade prévia:** Considera probabilidade prévia de hipótese, não apenas quão provável evidência é dado hipótese.
- **É matematicamente rigoroso:** É matematicamente rigoroso, fornecendo forma precisa de atualizar crenças.
- **É amplamente aplicável:** É amplamente aplicável em muitos campos - diagnóstico médico, aprendizado de máquina, tomada de decisão, inferência científica.

**Fórmula:**
P(H | E) = [P(E | H) × P(H)] / P(E)

Onde:
- P(H | E) = Probabilidade posterior de H dado E
- P(E | H) = Probabilidade de E dado H (likelihood)
- P(H) = Probabilidade prévia de H
- P(E) = Probabilidade marginal de E

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Você tem probabilidade prévia de hipótese antes de observar evidência.
* **Pressuposto 2:** Você pode calcular probabilidade de observar evidência dado hipótese (likelihood).
* **Pressuposto 3:** Você pode calcular probabilidade marginal de evidência (probabilidade total sob todas as hipóteses possíveis).
* **Pressuposto 4:** Você quer atualizar sua crença em hipótese à luz de nova evidência.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Atualizar crenças:** Ao atualizar crenças à luz de nova evidência, usar Teorema de Bayes para atualizar sistematicamente.
- **Calcular probabilidades condicionais:** Ao calcular probabilidades condicionais, usar Teorema de Bayes quando você tem probabilidade prévia e likelihood.
- **Fazer inferências:** Ao fazer inferências, usar Teorema de Bayes para fazer inferências mais precisas considerando probabilidade prévia.
- **Tomar decisões sob incerteza:** Ao tomar decisões sob incerteza, usar Teorema de Bayes para atualizar crenças à medida que nova informação chega.

**Domínios Típicos:** Estatística, Probabilidade, Diagnóstico Médico, Aprendizado de Máquina, Tomada de Decisão, Inferência Científica.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Ignorar prior ("base rate fallacy"):** Mesmo com evidência forte, se prior é muito baixo, posterior pode ainda ser baixo. Não ignore prior.
- **Confundir P(A|B) com P(B|A):** Apenas porque evidência é provável dado hipótese não significa que hipótese é provável dado evidência.
- **Assumir P(E) é apenas P(E|H):** Mas evidência pode também vir sob outras hipóteses. Deve considerar todas.
- **Prior incorreto:** Se prior está incorreto, posterior também estará incorreto.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Ignorar prior:** Ignorar probabilidade prévia de hipótese - mesmo com evidência forte, se prior é muito baixo, posterior pode ainda ser baixo.
- **Confundir P(A|B) com P(B|A):** Confundir probabilidade de A dado B com probabilidade de B dado A.
- **Assumir P(E) é apenas P(E|H):** Assumir que probabilidade marginal de evidência é apenas probabilidade dado hipótese, mas evidência pode também vir sob outras hipóteses.
- **Prior incorreto:** Usar prior incorreto - se prior está incorreto, posterior também estará incorreto.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está ignorando probabilidade prévia de hipótese.
  - Você está confundindo probabilidade de A dado B com probabilidade de B dado A.
  - Você não está considerando todas as hipóteses possíveis ao calcular probabilidade marginal de evidência.
  - Você está usando prior incorreto.

* **Evidência Prática:** 
  - Suas probabilidades posteriores estão incorretas porque você ignorou prior ou usou prior incorreto.
  - Você não está capturando probabilidade real porque confundiu direções de probabilidade condicional.

## 5. Passos de Pensamento (Algoritmo)
1. **Identifique hipótese:** Identifique hipótese H que você quer atualizar.

2. **Determine probabilidade prévia:** Determine probabilidade prévia P(H) - sua crença inicial em hipótese antes de observar qualquer nova evidência.

3. **Observe evidência:** Observe nova evidência E.

4. **Calcule likelihood:** Calcule probabilidade de observar evidência dado hipótese P(E | H).

5. **Calcule probabilidade marginal:** Calcule probabilidade marginal de evidência P(E) - probabilidade total de observar evidência sob todas as hipóteses possíveis. Se H e seu complemento ¬H são apenas duas hipóteses, então P(E) = P(E | H) × P(H) + P(E | ¬H) × P(¬H).

6. **Calcule probabilidade posterior:** Calcule probabilidade posterior usando fórmula: P(H | E) = [P(E | H) × P(H)] / P(E).

7. **Use posterior como novo prior:** Se mais evidência chega, use posterior como novo prior e repita processo.

8. **Monitore e ajuste:** Após calcular probabilidade posterior, monitore se está funcionando como esperado. Ajuste se necessário.

9. **Use apropriadamente:** Use Teorema de Bayes para atualizar crenças sistematicamente à luz de nova evidência, mas reconheça limitações - você precisa de prior correto e deve considerar todas as hipóteses possíveis.

10. **Eduque outros:** Eduque outros sobre Teorema de Bayes para ajudá-los a fazer inferências mais precisas.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao atualizar crenças à luz de nova evidência e o resultado foi usar Teorema de Bayes, resultando em atualizações muito mais precisas de crenças.

* **Erro:** Ignorei este modelo ao calcular probabilidades e paguei o preço ao ignorar probabilidade prévia, resultando em probabilidades posteriores incorretas.

* **Insight:** Descobri que Teorema de Bayes é especialmente importante para entender como atualizar crenças - você deve considerar não apenas quão provável evidência é dado hipótese, mas também probabilidade prévia de hipótese.

* **Aplicação prática:** Usei este modelo para melhorar inferências, descobrindo que usar Teorema de Bayes resulta em muito mais precisas atualizações de crenças e inferências melhores.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Probability]]
* [[Conditional Probability]]
* [[Base Rate Fallacy]]
* [[Statistical Inference]]
* [[Updating Beliefs]]

**Fontes:**
* Bayes, Thomas - Bayes' Theorem
* Wikipedia - Bayes' Theorem
* Research on probability and statistical inference

**Exemplos Notáveis:**
* **Teste médico:** Suponha que há doença rara que afeta 1% de população. Prior: P(Doença) = 0.01. Se teste é 99% sensível e 95% específico, e paciente testa positivo, probabilidade posterior de que realmente tem doença é aproximadamente 16.7%, porque doença é rara e falsos positivos acontecem. Teorema de Bayes quantifica exatamente como raridade e precisão de teste interagem.
