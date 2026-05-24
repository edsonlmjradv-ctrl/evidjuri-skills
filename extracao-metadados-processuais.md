---
name: extracao-metadados-processuais
description: Extrair metadados judiciais como número CNJ, classe judicial, partes, valor da causa, órgão julgador, datas de autuação e citação, movimentações. Use quando solicitado extrair, coletar, obter dados do processo, metadados do sistema PJe, consultar autos, analisar cabeçalho processual, puxar informações de um processo, ou quando precisar de estruturação inicial para qualquer análise jurídica automatizada.
---

# Habilidade: Extração de Metadados Processuais

## 1. Objetivo
Extrair de forma estruturada, confiável e auditável todos os metadados essenciais de um processo judicial.

## 2. Instruções Detalhadas
### 2.1 Entrada esperada
- Número CNJ, link para consulta processual pública, texto copiado do andamento, ou JSON parcial.

### 2.2 Passos
1. Validar CNJ (módulo 11).
2. Normalizar dados: remover formatação, converter datas para ISO, extrair CPF/CNPJ.
3. Mapear campos obrigatórios: cnj, classe, polo_ativo, polo_passivo, valor_causa, orgao_julgador, data_autuacao, data_citacao, ultima_movimentacao, dias_parado.
4. Tratar erros: CNJ inválido, falta de dados, indisponibilidade de fonte.
5. Registrar log.

### 2.3 Exemplo de entrada
```
Processo: 1030244-75.2026.8.11.0041 (2ª VARA ESP. DA FAZENDA PÚBLICA DE CUIABÁ)
Valor da causa: R$ 1.200.000,00
Autor: JOAQUIM MARTINS SPADONI
```

### 2.4 Exemplo de saída (JSON)
```json
{
  "cnj": "1030244-75.2026.8.11.0041",
  "classe": "DESAPROPRIAÇÃO",
  "polo_ativo": [{"nome": "JOAQUIM MARTINS SPADONI", "documento": null}],
  "polo_passivo": [{"nome": "MUNICÍPIO DE CUIABÁ", "documento": null}],
  "valor_causa": 1200000.00,
  "orgao_julgador": "2ª VARA ESP. DA FAZENDA PÚBLICA DE CUIABÁ",
  "data_autuacao": "2026-02-15",
  "data_citacao": null,
  "ultima_movimentacao": {"texto": "Conclusos para decisão", "data": "2026-05-10"},
  "dias_parado": 15
}
```

## 3. Agentes EvidJuri
A1.01, A1.02, A1.03, A1.04, A1.05, A1.06, A1.07, A1.08

## 4. Certificações
ISO 27001, LGPD
