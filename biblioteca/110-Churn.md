---
type: mental-model
title: "Churn"
category:
  - pensamento-geral
origin: Business, Subscription Models
author_reference: Business metrics
domains:
  - negócios
  - métricas
tags:
  - modelo-mental
  - pensamento
  - churn
aliases:
  - Taxa de Cancelamento
  - Customer Churn
  - Churn Rate
created: 2025-01-27
updated: 2025-01-27
---
# [[Churn]]

> **Teste de Pertinência:** *Você está gerenciando negócio com modelo de assinatura ou receita recorrente e precisa entender quantos clientes param de assinar e como isso afeta crescimento? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Churn (Taxa de Cancelamento) é número de clientes que param de assinar produto ou serviço. Taxa de churn é porcentagem de clientes que param de assinar durante período de tempo dado. Pode ser calculada para clientes ("logo churn") ou para receita (quanto MRR/ARR é perdido). Para negócio crescer, número de novos clientes adicionados a cada ano deve ser maior que taxa de churn.

**Explicação:**
Este modelo funciona porque reconhece que em negócios com receita recorrente, manter clientes existentes é tão importante quanto adquirir novos. Alto churn significa que receita recorrente encolhe a menos que aquisições superem perdas. Retenção impacta Customer Lifetime Value (CLV), margens, e sustentabilidade de crescimento. Isto funciona porque reconhece que é mais custoso adquirir novo cliente que manter existente, então reduzir churn pode ser mais eficiente que aumentar aquisições.

A lógica central é que através de monitorar e reduzir churn, você pode melhorar retenção e aumentar valor de longo prazo de base de clientes. Isto funciona porque reconhece que churn pode ser voluntário (cancelamentos) ou involuntário (falhas de pagamento, cartões expirados) - reduzir churn involuntário é frequentemente vitória rápida.

Funciona porque:
- **Impacta receita recorrente:** Alto churn significa que receita recorrente encolhe a menos que aquisições superem perdas.
- **Impacta CLV:** Retenção impacta Customer Lifetime Value - se churn é c por período e margem média por cliente é m, então aproximadamente LTV ≈ m ÷ c.
- **É mais eficiente:** É mais custoso adquirir novo cliente que manter existente.
- **Pode ser melhorado:** Reduzir churn involuntário (falhas de pagamento) é frequentemente vitória rápida.

**Tipos de churn:**
- **Churn voluntário:** Cancelamentos - clientes decidem cancelar.
- **Churn involuntário:** Falha de pagamento, cartões expirados, etc. - frequentemente contribui 20-40% do total de perdas de churn.

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Você tem negócio com modelo de assinatura ou receita recorrente.
* **Pressuposto 2:** Você pode rastrear quando clientes param de assinar.
* **Pressuposto 3:** Você pode distinguir entre churn voluntário e involuntário.
* **Pressuposto 4:** Você quer melhorar retenção e reduzir churn.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Monitorar retenção:** Ao monitorar retenção, usar taxa de churn para entender quantos clientes estão saindo.
- **Melhorar retenção:** Ao melhorar retenção, identificar causas de churn e tomar medidas para reduzir.
- **Calcular CLV:** Ao calcular Customer Lifetime Value, usar taxa de churn para estimar tempo médio que cliente permanece.
- **Avaliar saúde do negócio:** Ao avaliar saúde do negócio, usar taxa de churn junto com aquisições para avaliar crescimento líquido.

**Domínios Típicos:** Negócios de Assinatura, SaaS, E-commerce, Serviços Recorrentes, Gestão de Clientes.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Não é modelo de assinatura:** Se você não tem modelo de assinatura ou receita recorrente, churn pode não ser métrica relevante.
- **Não considerar contexto:** Não considerar contexto - benchmarks de churn variam muito por indústria, tipo de negócio, ARPU.
- **Focar apenas em churn:** Focar apenas em reduzir churn sem considerar outros fatores - qualidade de clientes, margens, etc.

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Focar apenas em churn total:** Focar apenas em churn total sem distinguir entre voluntário e involuntário.
- **Ignorar benchmarks:** Ignorar benchmarks apropriados - churn "bom" varia muito por indústria.
- **Não considerar qualidade:** Não considerar qualidade de clientes - reduzir churn de clientes de baixo valor pode não ser benéfico.
- **Não monitorar tendências:** Não monitorar tendências ao longo do tempo - churn pode variar sazonalmente.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está focando apenas em churn total sem distinguir entre voluntário e involuntário.
  - Você não está considerando benchmarks apropriados.
  - Você não está monitorando tendências ao longo do tempo.
  - Você não está considerando qualidade de clientes ao reduzir churn.

* **Evidência Prática:** 
  - Suas estratégias de retenção estão ineficientes porque você não distinguiu entre tipos de churn.
  - Você não está capturando realidade porque ignorou benchmarks apropriados ou tendências.

## 5. Passos de Pensamento (Algoritmo)
1. **Calcule taxa de churn:** Calcule taxa de churn:
   - **Churn de clientes:** (Número de clientes perdidos durante período) ÷ (Número de clientes no início do período)
   - **Churn de receita:** (Receita recorrente perdida) ÷ (Receita recorrente no início)

2. **Distinguir voluntário vs involuntário:** Distinguir entre churn voluntário (cancelamentos) e involuntário (falhas de pagamento, cartões expirados).

3. **Compare com benchmarks:** Compare com benchmarks apropriados:
   - B2B SaaS: ~1-4% churn mensal; churn anual de logo ~10-20%
   - B2C serviços de assinatura: Churn mensal frequentemente entre 5-10%
   - Streaming/mídia: Frequentemente 5-8% churn mensal

4. **Identifique causas:** Identifique causas de churn:
   - Churn voluntário: Onboarding pobre, suporte ao cliente, valor do produto
   - Churn involuntário: Falhas de pagamento, cartões expirados, problemas técnicos

5. **Priorize redução:** Priorize redução de churn:
   - Reduzir churn involuntário é frequentemente vitória rápida - use mecanismos de retry de pagamento, lembretes
   - Reduzir churn voluntário requer melhorar onboarding, suporte ao cliente, valor do produto

6. **Calcule CLV:** Calcule Customer Lifetime Value usando taxa de churn - se churn mensal é 5%, tempo médio de vida do cliente é aproximadamente 20 meses (1 ÷ 0.05).

7. **Monitore Net Revenue Retention:** Monitore Net Revenue Retention (NRR) - mede quanto receita de clientes existentes é retida após churn, downgrades e upgrades. Se NRR > 100%, base de clientes existentes está crescendo em receita.

8. **Considere sazonalidade:** Considere sazonalidade - churn pode aumentar em certos meses dependendo da indústria.

9. **Use para decisões:** Use análise de churn para informar decisões sobre retenção, mas não ignore outros fatores - qualidade de clientes, margens, etc.

10. **Monitore e ajuste:** Após implementar estratégias de redução de churn, monitore se estão funcionando. Ajuste se necessário.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao gerenciar negócio de assinatura e o resultado foi monitorar e reduzir churn, resultando em muito melhor retenção e crescimento.

* **Erro:** Ignorei este modelo ao gerenciar negócio e paguei o preço ao focar apenas em aquisições, ignorando churn alto que estava erodindo base de clientes.

* **Insight:** Descobri que churn é especialmente importante para negócios com receita recorrente - manter clientes existentes é tão importante quanto adquirir novos.

* **Aplicação prática:** Usei este modelo para melhorar retenção, descobrindo que monitorar e reduzir churn resulta em muito melhor valor de longo prazo de base de clientes e crescimento mais sustentável.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Customer Lifetime Value]]
* [[Retention Rate]]
* [[Net Revenue Retention]]
* [[Subscription Model]]
* [[Recurring Revenue]]

**Fontes:**
* Business metrics literature
* Wikipedia - Churn rate
* Research on customer retention and subscription businesses

**Exemplos Notáveis:**
* **B2B SaaS:** Churn mensal típico de ~1-4%; churn anual de logo ~10-20%. Churn menor em contratos enterprise.
* **B2C serviços de assinatura:** Churn mensal frequentemente entre 5-10%, embora alguns verticais (kits de refeição, caixas de consumidor) sejam muito maiores.
