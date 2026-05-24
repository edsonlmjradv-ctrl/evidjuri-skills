---
name: deteccao-grupo-economico
description: Detectar grupo econômico a partir de CNPJ, identificando empresas controladoras, coligadas, sócios comuns, relações societárias. Use para desconsideração inversa, responsabilização de sócios, execução contra grupo.
---

# Habilidade: Detecção de Grupo Econômico

## 1. Objetivo
Mapear empresas do mesmo grupo econômico para redirecionamento da execução.

## 2. Instruções
1. A partir do CNPJ da empresa executada, obter quadro societário.
2. Para cada sócio, buscar outras empresas em que ele participe (como sócio ou administrador).
3. Identificar também empresas controladoras e coligadas.
4. Construir um grafo de relacionamento.
5. Gerar organograma e lista de CNPJs.

## 3. Exemplo
Executada XP Ltda. Sócio único João Silva também é sócio de Alpha S/A e Beta ME. Grupo econômico mapeado.

## 4. Agentes
A5.05, A5.06, A2.01

## 5. Certificações
ISO 27001
