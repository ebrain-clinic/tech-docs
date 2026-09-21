| Campo              | Tipo    | Descrição                                                            | Restrição |
|--------------------|---------|----------------------------------------------------------------------|-----------|
| unique_cod         | varchar | Código externo estável do estoque                                    | Obrigatório |
| nome_estoque       | varchar | Nome do estoque, com até 200 caracteres                              | Obrigatório |
| clinica_unique_cod | varchar | Código da clínica do estoque                                         |           |

A view de destino usa unique_cod como import_id de produto_estoque e como código externo no import_externo. Estoques distintos podem ter o mesmo nome. Quando a clínica não é informada, a importação usa a clínica padrão.
