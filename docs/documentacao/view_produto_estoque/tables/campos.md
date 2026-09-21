| Campo              | Tipo    | Descrição                                                            | Restrição |
|--------------------|---------|----------------------------------------------------------------------|-----------|
| unique_cod         | varchar | Código externo estável do estoque                                    | Obrigatório |
| nome_estoque       | varchar | Nome do estoque, com até 200 caracteres                              | Obrigatório e único por clínica |
| clinica_unique_cod | varchar | Código da clínica do estoque                                         |           |

A view de destino usa unique_cod como import_id de produto_estoque e como código externo no import_externo. Dentro do mesmo tenant, estoques distintos podem ter o mesmo nome normalizado por `upper(btrim(nome_estoque))` somente quando pertencem a clínicas diferentes. A repetição na mesma clínica é um erro. Quando a clínica não é informada, a importação usa a clínica padrão, que também participa dessa validação.
