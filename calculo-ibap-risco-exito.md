---
name: calculo-ibap-risco-exito
description: Calcular o Índice de Aproveitamento (IBAP) – probabilidade de êxito de 0 a 100 – baseado em jurisprudência dominante, qualidade da prova e nulidades. Use para risco de êxito, chance de ganhar a causa, score preditivo.
---

# Habilidade: Cálculo do Índice de Aproveitamento (IBAP)

## 1. Objetivo
Fornecer um score objetivo de probabilidade de êxito para uma demanda judicial.

## 2. Instruções
1. Coletar jurisprudência do tribunal sobre o tema (últimos 2 anos).
2. Calcular taxa de sucesso (procedência total + parcial / total).
3. Ajustar por fatores: qualidade da prova documental, existência de perícia favorável, nulidades, prescrição.
4. Normalizar para 0–100.
5. Retornar IBAP e nível de confiança.

## 3. Exemplo
Ação de indenização por danos em transportadora: jurisprudência 70% de procedência parcial, provas robustas, sem nulidades => IBAP 78.

## 4. Agentes
A4.05, A2.02, A2.01

## 5. Certificações
IBAP (certificação própria), OEA (equidade)
