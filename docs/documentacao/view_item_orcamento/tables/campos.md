| Campo                        | Tipo        | Descrição                                                                           | Restrição       |
|------------------------------|-------------|-------------------------------------------------------------------------------------|-----------------|
| unique_cod                   | varchar     | Código único do item do orçamento ou procedimento                                           | Obrigatório     |
| orcamento_unique_cod         | varchar     | Código único do orçamento original                                                  | Obrigatório     |
| descricao                    | varchar     | Descrição do item do orçamento                                                      | Obrigatório     |
| quantidade                   | integer     | Quantidade de itens ou procedimentos no orçamento                                   |                 |
| valor_unitario               | numeric     | Valor unitário do item                                                              |                 |
| valor_desconto_percentual      | numeric     | Valor percentual do desconto aplicado ao item                                         |                 |
| valor_desconto_absoluto      | numeric     | Valor absoluto do desconto aplicado ao item                                         |                 |
| valor_total_item        | numeric     | Valor total do item do orçamento                                                           |                 |
| observacoes                   | varchar     | Observações gerais do item do orçamento                                                     |                 |
| servico_unique_cod           | varchar     | Código único do serviço associado ao item                                           |                 |
