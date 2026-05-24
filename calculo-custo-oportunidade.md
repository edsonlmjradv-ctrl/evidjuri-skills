---
name: calculo-custo-oportunidade
description: Calcular o custo de oportunidade de descartar ou abandonar um processo judicial, usando fórmula de valor futuro com taxa de desconto de 12% a.a. e prazo de 3 anos. Use para estimar perda financeira, VPL, ROI forense, ativo judicial subavaliado.
---

# Habilidade: Cálculo de Custo de Oportunidade

## 1. Objetivo
Calcular quanto se perde financeiramente ao abandonar um processo (ex: execução fiscal, ação indenizatória) em vez de executá-lo até o fim.

## 2. Instruções
1. Receber o valor da causa (ou valor esperado de recuperação).
2. Aplicar taxa de êxito (IBAP) e fator de conversão (70%).
3. Calcular valor futuro: `VF = beneficio_medio * (1 + 0,12)^3`.
4. Subtrair o valor presente do benefício para obter o custo de oportunidade.
5. Formatar resposta em reais.

## 3. Exemplo
Valor da causa R$ 100.000, IBAP 60% => benefício esperado R$ 60.000. Custo = 60.000 * (1,12^3 -1) = 60.000 * 0,4049 = R$ 24.294.

## 4. Agentes
A4.01, A4.05, A4.06

## 5. Certificações
IBAP, ISO 27001
