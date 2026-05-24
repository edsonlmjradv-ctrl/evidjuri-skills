---
name: deteccao-divergencia-documental
description: Comparar petição inicial com documentos anexados para identificar divergências de datas, nomes, valores ou cláusulas. Use quando precisar detectar inconsistências, diferenças documentais, conflitos entre inicial e provas, ou score de divergência.
---

# Habilidade: Detecção de Divergência Documental

## 1. Objetivo
Identificar automaticamente inconsistências entre a narrativa da petição inicial e os documentos juntados (contratos, notas, laudos).

## 2. Instruções
1. Extrair texto da petição inicial e dos principais documentos anexos.
2. Identificar campos-chave: datas, nomes das partes, valores, cláusulas contratuais.
3. Comparar os valores (ex: data na inicial vs. data no contrato). Calcular diferença percentual.
4. Atribuir score de divergência (0–100). Se score >= 70, disparar alerta.
5. Gerar relatório indicando a(s) divergência(s) e sua gravidade (leve, média, grave).
6. Sugerir emenda da inicial se ainda houver prazo.

## 3. Exemplo
Entrada: inicial diz "contrato assinado em 10/01/2024"; contrato anexado tem data 15/02/2024. Saída: `{"divergencia": "data", "score": 85, "gravidade": "grave"}`.

## 4. Agentes
A1.23, A2.01, A3.11

## 5. Certificações
ISO 27001
