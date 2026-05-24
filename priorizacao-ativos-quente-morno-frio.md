---
name: priorizacao-ativos-quente-morno-frio
description: Priorizar ativos judiciais com scores quentes (alta urgência), mornos (média) e frios (baixa), baseado em risco, tempo parado, valor e chance de êxito. Use para gestão de carteira, fila de execução, triagem.
---

# Habilidade: Priorização de Ativos (Quente/Morno/Frio)

## 1. Objetivo
Ajudar escritórios a decidir qual processo priorizar.

## 2. Instruções
1. Para cada processo, calcular score combinado: tempo parado (40%), risco de êxito (30%), valor da causa (20%), existência de urgência (10%).
2. Normalizar para 0-100.
3. Classificar: score >=80 = quente, 55-79 = morno, <55 = frio.
4. Sugerir ação: quente -> revisão imediata, morno -> revisão semanal, frio -> revisão quinzenal.

## 3. Exemplo
Processo com IBAP 90%, valor R$ 1M, parado 90 dias => score 85 -> quente.

## 4. Agentes
A1.07, A4.05, A1.04

## 5. Certificações
IBAP
