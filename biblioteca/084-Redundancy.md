---
type: mental-model
title: "Redundancy"
category:
  - pensamento-geral
origin: Engineering, Systems Design
author_reference: Engineering reliability principles
domains:
  - engenharia
  - sistemas
  - confiabilidade
  - backup
tags:
  - modelo-mental
  - pensamento
  - redundância
  - backup
  - confiabilidade
aliases:
  - Redundância
  - Backup Systems
  - Fault Tolerance
  - Reliability
created: 2025-01-27
updated: 2025-01-27
---
# [[Redundancy]]

> **Teste de Pertinência:** *Você está projetando sistema crítico e precisa garantir que sistema pode continuar operando mesmo se alguns componentes falharem, ou está tentando aumentar confiabilidade através de duplicação? Se a resposta for "Sim", este modelo é a ferramenta correta para o momento.*

## 1. Definição e Mecanismo
**O que é:**
Redundancy (Redundância) significa duplicar intencionalmente componentes ou funções críticas para que sistema possa continuar operando mesmo se algumas partes falharem. Pode incluir dados, hardware, software, caminhos de rede, fontes de energia, etc. É elemento chave de confiabilidade, tolerância a falhas e alta disponibilidade. Mas redundância deve ser bem projetada - redundância pobre pode introduzir complexidade, modos de falha comuns ou complacência.

**Explicação:**
Este modelo funciona porque reconhece que componentes falham. Ao duplicar componentes críticos, você reduz probabilidade de que falha de componente único cause falha de sistema. Com componentes redundantes em paralelo, todos os componentes devem falhar para falha total do sistema - isto aumenta MTBF (tempo médio entre falhas) do sistema. Redundância também ajuda permitindo failover - sistemas permanecem operacionais enquanto recuperação acontece.

A lógica central é que através de redundância apropriada, você pode aumentar significativamente confiabilidade e disponibilidade de sistema. No entanto, redundância deve ser bem projetada - componentes redundantes devem ser independentes (evitar modos de falha comuns), deve haver monitoramento para detectar falhas, e failover deve funcionar efetivamente. Redundância também tem trade-offs - aumenta custo, complexidade, manutenção.

Funciona porque:
- **Reduz probabilidade de falha:** Com componentes redundantes, todos devem falhar para falha total.
- **Permite failover:** Permite que sistema continue operando enquanto componentes falhados são recuperados.
- **Aumenta disponibilidade:** Aumenta fração de tempo que sistema está operacional.
- **Melhora tolerância a falhas:** Melhora capacidade de sistema de aderir a especificação mesmo com falhas.

**Tipos principais:**
- **Redundância ativa (quente ou paralela):** Todos os elementos redundantes estão rodando simultaneamente
- **Redundância em espera (fria, morna, quente):** Backup está desligado ou parcialmente rodando até ser necessário
- **N+1, N+2, 2N, 2N+1:** N+1 = um backup extra para N ativos; 2N = duplicação completa
- **Redundância modular:** DMR (dupla), TMR (tripla com votação)
- **Redundância geográfica:** Sistemas de backup localizados fisicamente separados

## 2. Pressupostos Fundamentais
*O modelo só é válido se estas premissas forem verdadeiras:*
* **Pressuposto 1:** Componentes falham - duplicar componentes críticos reduz probabilidade de falha de sistema.
* **Pressuposto 2:** Componentes redundantes devem ser independentes - evitar modos de falha comuns.
* **Pressuposto 3:** Deve haver monitoramento para detectar falhas e failover efetivo.
* **Pressuposto 4:** Redundância tem trade-offs - aumenta custo, complexidade, manutenção.

## 3. Contexto de Aplicação

### Quando Usar (Luz Verde)
* Situações onde o modelo produz boas decisões rapidamente:*
- **Sistemas críticos:** Ao projetar sistemas críticos onde falha tem consequências altas, usar redundância apropriada.
- **Alta disponibilidade:** Ao projetar sistemas que requerem alta disponibilidade, usar redundância para garantir operação contínua.
- **Tolerância a falhas:** Ao projetar sistemas que devem tolerar falhas, usar redundância para permitir operação mesmo com falhas.
- **Backup e recuperação:** Ao projetar sistemas de backup e recuperação, usar redundância para garantir que dados ou serviços podem ser recuperados.
- **Aplicar a sistemas não técnicos:** Ao aplicar a sistemas não técnicos (ex: processos, equipes), reconhecer que "redundância" pode aumentar confiabilidade.

**Domínios Típicos:** Engenharia, Sistemas, Confiabilidade, Alta Disponibilidade, Backup.

### Quando Evitar (Luz Vermelha)
* Situações onde o modelo induz ao erro ou simplifica demais a realidade:*
- **Quando custo é crítico:** Se custo é crítico e redundância adiciona custo desproporcional, pode precisar balancear.
- **Modos de falha comuns:** Se componentes redundantes compartilham dependências comuns (ex: mesma fonte de energia), ambos podem falhar juntos.
- **Complexidade excessiva:** Redundância pode adicionar complexidade que na verdade reduz confiabilidade se não for bem projetada.
- **Não como única estratégia:** Não usar redundância como única estratégia de confiabilidade - há outras (manutenção, monitoramento, etc.).

## 4. Zona de Risco (Diagnóstico)

### Uso Incorreto Comum
* Como amadores costumam distorcer esse modelo:*
- **Modos de falha comuns:** Criar redundância que compartilha dependências comuns, resultando em falha simultânea de componentes redundantes.
- **Falta de monitoramento:** Não monitorar componentes redundantes, tornando redundância inútil se você não sabe qual componente falhou.
- **Complacência:** Assumir que sistema é seguro apenas porque redundância existe, sem testar ou manter adequadamente.
- **Complexidade excessiva:** Adicionar redundância que aumenta complexidade mais que aumenta confiabilidade.

### Sinais de que Você Saiu do Modelo
* **Indicador Comportamental:** 
  - Você está criando redundância com modos de falha comuns.
  - Você não está monitorando componentes redundantes.
  - Você está assumindo que redundância sempre funciona.
  - Você está adicionando complexidade excessiva.

* **Evidência Prática:** 
  - Seus componentes redundantes falham juntos porque compartilham dependências comuns.
  - Você não sabe qual componente falhou porque não está monitorando.
  - Seu sistema falha apesar de redundância porque não foi testada ou mantida.

## 5. Passos de Pensamento (Algoritmo)
1. **Identifique componentes críticos:** Use ferramentas como FMEA para encontrar partes cuja falha tem maior impacto. Foque redundância aqui.

2. **Determine nível de redundância:** Determine nível apropriado de redundância:
   - N+1: um backup extra para N ativos
   - N+2: dois backups
   - 2N: duplicação completa
   - TMR: tripla redundância modular com votação

3. **Garanta independência:** Certifique-se de que componentes redundantes são independentes - evite pontos de falha compartilhados (fonte de energia, localização física, bugs de software). Separação geográfica, diversidade em implementação ajudam.

4. **Selecione tipo apropriado:** Selecione tipo apropriado de redundância:
   - Ativa (quente): todos rodando simultaneamente, failover imediato
   - Em espera (fria/morna/quente): backup desligado ou parcialmente rodando até necessário

5. **Implemente monitoramento:** Inclua diagnóstico, lógica de votação, auto-testes para detectar qual elemento falhou. Redundância é inútil se você não pode detectar falha.

6. **Implemente failover:** Certifique-se de que mecanismos de failover funcionam - failover automático, chaveamento de backup, e testes regulares são críticos.

7. **Teste regularmente:** Teste redundância regularmente - certifique-se de que backups funcionam, dados são válidos, failovers são rápidos.

8. **Considere degradação graciosa:** Mesmo se redundância falha parcialmente, sistema deve ainda entregar performance reduzida mas aceitável em vez de colapso total.

9. **Avalie trade-offs:** Avalie trade-offs - mais redundância aumenta custo, manutenção, consumo de energia, complexidade. Otimize baseado em requisitos.

10. **Monitore e ajuste:** Após implementar redundância, monitore se está funcionando como esperado. Ajuste se necessário.

## 6. Notas de Campo (Pessoal)
*Reflexões subjetivas, batalhas reais e cicatrizes.*

* **Experiência:** Usei isso ao projetar sistema crítico e o resultado foi implementar redundância apropriada com monitoramento e failover, resultando em sistema que continuou operando mesmo quando componentes falharam.

* **Erro:** Ignorei este modelo ao projetar sistema e paguei o preço ao não incluir redundância, resultando em falha de sistema quando componente único falhou.

* **Insight:** Descobri que redundância é especialmente importante quando consequências de falha são altas - duplicar componentes críticos reduz significativamente probabilidade de falha de sistema.

* **Aplicação prática:** Usei este modelo para melhorar confiabilidade de sistemas, descobrindo que implementar redundância apropriada com monitoramento e failover resulta em sistemas muito mais confiáveis e disponíveis.

---
## Referências e Conexões
**Modelos Relacionados:**
* [[Reliability]]
* [[Fault Tolerance]]
* [[Backup Systems]]
* [[High Availability]]
* [[Failure Modes]]

**Fontes:**
* Engineering reliability principles
* Wikipedia - Redundancy (Engineering)
* Research on system reliability and fault tolerance

**Exemplos Notáveis:**
* **Aeronaves:** Controles de voo frequentemente usam redundância modular tripla (TMR), com lógica de votação, para operações críticas para segurança.
* **Centros de dados:** Fontes de energia frequentemente em redundância N+1, 2N. Sistemas UPS, geradores. Redundância geográfica para backups através de regiões.
