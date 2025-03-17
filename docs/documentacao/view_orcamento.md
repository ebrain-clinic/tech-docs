# Orçamento

<p align="justify"> 
Descreve a estrutura de dados relacionada aos orçamentos, incluindo informações sobre orçamentos criados, itens associados, serviços, profissionais, pacientes, pedidos e transações financeiras. 
</p>

> Nome do arquivo de importação: `import_orcamento.csv`

## Descrição dos campos

| Campo                        | Tipo        | Descrição                                                                           | Restrição       |
|------------------------------|-------------|-------------------------------------------------------------------------------------|-----------------|
| unique_cod                   | varchar     | Código único do orçamento ou procedimento                                           | Obrigatório     |
| orcamento_unique_cod         | varchar     | Código único do orçamento original                                                  | Obrigatório     |
| data_orcamento               | timestamp   | Data de criação do orçamento                                                        | Obrigatório     |
| data_registro                | timestamp   | Data e hora de registro do orçamento                                                | Obrigatório     |
| data_validade_orcamento      | timestamp   | Data de vencimento do orçamento                                                     | Obrigatório     |
| data_exclusao                | timestamp   | Data de exclusão do orçamento                                                       |                 |
| orcamento_concluido          | boolean     | Indica se o orçamento está concluído                                                |                 |
| observacao                   | varchar     | Observações gerais do orçamento                                                     |                 |
| instrucoes_realizacao        | varchar     | Instruções para realização do orçamento                                             |                 |
| pessoa_unique_cod            | varchar     | Código único do paciente associado ao orçamento                                     | Obrigatório     |
| profissional_unique_cod      | varchar     | Código único do profissional responsável pelo orçamento                             | Obrigatório     |
| usuario_venda_unique_cod     | varchar     | Código único do usuário responsável pela venda                                      | Obrigatório     |
| clinica_unique_cod           | varchar     | Código único da clínica associada                                                   |                 |
| servico_unique_cod           | varchar     | Código único do serviço associado ao item                                           |                 |
| servico_nome                 | varchar     | Nome do serviço associado ao item                                                   |                 |
| descricao                    | varchar     | Descrição do item do orçamento                                                      | Obrigatório     |
| quantidade                   | integer     | Quantidade de itens ou procedimentos no orçamento                                   |                 |
| valor_debug                  | numeric     | Valor total do item para depuração                                                  |                 |
| valor_unitario               | numeric     | Valor unitário do item                                                              |                 |
| valor_desconto_absoluto      | numeric     | Valor absoluto do desconto aplicado ao item                                         |                 |
| ordem                        | varchar     | Ordem do pedido associado ao orçamento                                              |                 |
| total_pago                   | numeric     | Total pago pelo orçamento                                                           |                 |
| operadora_saude_unique_cod   | varchar     | Código único da operadora de saúde                                                  |                 |
| operadora_codigo_autorizacao | varchar     | Código de autorização da operadora de saúde                                         |                 |
| pacote                       | varchar     | Indica se o orçamento é parte de um pacote                                          |                 |
| cortesia                     | varchar     | Indica se o orçamento é uma cortesia                                                |                 |
| tipo_transacao               | varchar     | Tipo de transação financeira (opções: DINHEIRO, CHEQUE, PIX, CARTAO_CREDITO, CARTAO_DEBITO, BOLETO) |                 |
| data_pagamento               | date        | Data do pagamento                                                                   |                 |

## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_orcamento.csv ':ignore')

