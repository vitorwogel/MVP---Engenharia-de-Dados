
# 📘 Catálogo de Dados

Abaixo estão descritas as tabelas utilizadas no projeto, com suas colunas, descrições e tipos de dados estimados:

---

### `tabela_fato`

| Campo                                | Descrição                                                                                      | Tipo    |
|--------------------------------------|------------------------------------------------------------------------------------------------|---------|
| ano_e_mes_do_lancamento              | Ano e mês de referência da despesa.                                                            | STRING  |
| codigo_orgao_superior               | Código do órgão superior responsável pela despesa.                                            | INTEGER |
| nome_orgao_superior                 | Nome do órgão superior responsável pela despesa.                                              | STRING  |
| codigo_orgao_subordinado           | Código do órgão subordinado responsável pela despesa.                                         | INTEGER |
| nome_orgao_subordinado             | Nome do órgão subordinado responsável pela despesa.                                           | STRING  |
| codigo_unidade_gestora             | Código da Unidade Gestora (UG) responsável pela despesa.                                      | INTEGER |
| nome_unidade_gestora               | Nome da Unidade Gestora responsável pela despesa.                                             | STRING  |
| codigo_gestao                       | Código da gestão.                                                                             | FLOAT   |
| nome_gestao                         | Nome da gestão.                                                                               | STRING  |
| codigo_unidade_orcamentaria        | Código da Unidade Orçamentária responsável pela despesa.                                      | INTEGER |
| nome_unidade_orcamentaria          | Nome da Unidade Orçamentária responsável pela despesa.                                        | STRING  |
| codigo_funcao                      | Código da Função orçamentária da despesa.                                                     | INTEGER |
| nome_funcao                        | Nome da Função orçamentária da despesa.                                                       | STRING  |
| codigo_subfucao                    | Código da Subfunção orçamentária da despesa.                                                  | INTEGER |
| nome_subfuncao                     | Nome da Subfunção orçamentária da despesa.                                                    | STRING  |
| codigo_programa_orcamentario       | Código do Programa em que foi classificada a despesa.                                         | INTEGER |
| nome_programa_orcamentario         | Nome do Programa em que foi classificada a despesa.                                           | STRING  |
| codigo_acao                         | Código da Ação Orçamentária relacionada à despesa.                                            | STRING  |
| nome_acao                           | Nome da Ação Orçamentária relacionada à despesa.                                              | STRING  |
| codigo_grupo_de_despesa            | Código do Grupo de Despesa que classifica o tipo de gasto realizado.                         | INTEGER |
| nome_grupo_de_despesa              | Nome do Grupo de Despesa que classifica o tipo de gasto realizado.                           | STRING  |
| valor_empenhado_rs                 | Valor empenhado (R$). Reserva orçamentária criada para uma obrigação futura de pagamento.     | FLOAT   |
| valor_liquidado_rs                 | Valor liquidado (R$). Valor verificado após entrega do bem/serviço e reconhecimento da dívida.| FLOAT   |
| valor_pago_rs                      | Valor pago (R$). Valor efetivamente transferido ao credor.                                     | FLOAT   |
| valor_restos_a_pagar_inscritos_rs | Valor de despesas empenhadas, mas não pagas até 31/12, inscritas como restos a pagar.         | FLOAT   |
| valor_restos_a_pagar_cancelado_rs | Valor dos restos a pagar que foram cancelados.                                                 | FLOAT   |
| valor_restos_a_pagar_pagos_rs     | Valor pago de restos a pagar anteriormente inscritos.                                          | FLOAT   |
| codigo_ano_mes                     | Identificador numérico do ano e mês (formato AAAAMM).                                          | INTEGER |

### data_cleaned['codigo_gestao']

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_gestao | Código identificador relacionado à entidade. | INTEGER |

### data_cleaned['nome_gestao']

| Campo | Descrição | Tipo |
|-------|-----------|------|
| nome_gestao | Nome relacionado à entidade. | STRING |

### data_cleaned['nome_orgao_subordinado']

| Campo | Descrição | Tipo |
|-------|-----------|------|
| nome_orgao_subordinado | Nome relacionado à entidade. | STRING |

### data_cleaned[col]

| Campo | Descrição | Tipo |
|-------|-----------|------|
| col | Descrição não especificada. | STRING |

### dim_orgao_superior

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_orgao_superior | Código identificador relacionado à entidade. | INTEGER |
| nome_orgao_superior | Nome relacionado à entidade. | STRING |

### dim_orgao_subordinado

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_orgao_subordinado | Código identificador relacionado à entidade. | INTEGER |
| nome_orgao_subordinado | Nome relacionado à entidade. | STRING |

### dim_gestao

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_gestao | Código identificador relacionado à entidade. | INTEGER |
| nome_gestao | Nome relacionado à entidade. | STRING |

### dim_unidade_gestora

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_unidade_gestora | Código identificador relacionado à entidade. | INTEGER |
| nome_unidade_gestora | Nome relacionado à entidade. | STRING |

### dim_programa_orcamentario

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_programa_orcamentario | Código identificador relacionado à entidade. | INTEGER |
| nome_programa_orcamentario | Nome relacionado à entidade. | STRING |

### dim_unidade_orcamentaria

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_unidade_orcamentaria | Código identificador relacionado à entidade. | INTEGER |
| nome_unidade_orcamentaria | Nome relacionado à entidade. | STRING |

### dim_funcao

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_funcao | Código identificador relacionado à entidade. | INTEGER |
| nome_funcao | Nome relacionado à entidade. | STRING |

### dim_subfuncao

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_subfucao | Código identificador relacionado à entidade. | INTEGER |
| nome_subfuncao | Nome relacionado à entidade. | STRING |

### dim_acao

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_acao | Código identificador relacionado à entidade. | STRING |
| nome_acao | Nome relacionado à entidade. | STRING |

### dim_despesa

| Campo | Descrição | Tipo |
|-------|-----------|------|
| codigo_grupo_de_despesa | Código identificador relacionado à entidade. | INTEGER |
| nome_grupo_de_despesa | Nome relacionado à entidade. | STRING |

