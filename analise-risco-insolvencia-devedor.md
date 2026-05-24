---
name: analise-risco-insolvencia-devedor
description: Analisar risco de insolvência do devedor usando score Serasa, SPC, consulta CNPJ, ações de falência. Use para recuperação judicial, probabilidade de calote, risco de crédito, execução frustrada.
---

# Habilidade: Análise de Risco de Insolvência do Devedor

## 1. Objetivo
Estimar a probabilidade de o devedor não pagar a condenação.

## 2. Instruções
1. Obter CNPJ/CPF do devedor.
2. Consultar bases de crédito (simulação: score 0-1000).
3. Verificar existência de processos de falência ou recuperação judicial.
4. Calcular risco: baixo (score > 600), médio (score 300-600), alto (score < 300 ou falência).
5. Ajustar o VPL do processo com fator de recuperação (ex: 0,6 para alto risco).

## 3. Exemplo
Devedor score Serasa 250 e em RJ. Risco alto. Fator de recuperação 0,2. VPL reduzido drasticamente.

## 4. Agentes
A4.72, A4.73, A5.05

## 5. Certificações
IBAP
