---
name: simulacao-acordo-antecipado
description: Comparar oferta de acordo com o VPL esperado do litígio, aplicando taxa de desconto de 12% a.a. e probabilidade de êxito. Use para decidir se aceita acordo, contraoferta, break-even, negociação antecipada.
---

# Habilidade: Simulação de Acordo Antecipado

## 1. Objetivo
Ajudar a parte a decidir matematicamente se deve aceitar uma oferta de acordo.

## 2. Instruções
1. Calcular VPL do litígio (valor esperado descontado).
2. Calcular VPL da oferta (se parcelada, descontar).
3. Se VPL_oferta >= 0,8 * VPL_litígio, recomendar aceitar. Senão, sugerir contraoferta no valor de VPL_litígio * 0,8.
4. Apresentar análise em tabela.

## 3. Exemplo
VPL litígio R$ 200.000. Oferta R$ 150.000 à vista => VPL oferta = 150.000. 150.000 / 200.000 = 0,75 => abaixo do limiar. Sugerir contraoferta de R$ 160.000.

## 4. Agentes
A4.09, A4.06, A4.05

## 5. Certificações
IBAP
