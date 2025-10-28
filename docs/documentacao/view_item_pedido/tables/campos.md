| Campo                          | Tipo      | Descrição                                                            | Restrição   |
|--------------------------------|-----------|----------------------------------------------------------------------|-------------|
| unique_cod                     | varchar   | Código único do item do pedido                                       | Obrigatório |
| ordem                          | integer   | Ordem do item no pedido                                              |             |
| pedido_unique_cod              | varchar   | Código único do pedido ao qual o item pertence                       | Obrigatório |
| item_orcamento_unique_cod      | varchar   | Código único do item de orçamento relacionado                        |             |
| descricao                      | varchar   | Descrição do item                                                    |             |
| quantidade                     | numeric   | Quantidade do serviço no item                                        | Obrigatório |
| data_registro                  | timestamp | Data e hora de registro do item                                      | Obrigatório |
| data_limite_consumo            | timestamp | Data limite para consumo do item                                     |             |
| quantidade_execucao_pendente   | numeric   | Quantidade ainda não executada do item                               |             |
| valor_unitario                 | numeric   | Valor unitário do item                                               |             |
| valor_desconto_percentual      | numeric   | Percentual de desconto aplicado ao item                              |             |
| valor_desconto_absoluto        | numeric   | Valor absoluto de desconto aplicado ao item                          |             |
| valor_total_item               | numeric   | Valor total do item (após descontos)                                 |             |
| servico_unique_cod             | varchar   | Código único do serviço associado ao item                            | Obrigatório |
