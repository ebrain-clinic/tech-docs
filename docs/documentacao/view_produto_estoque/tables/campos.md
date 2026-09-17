| Campo              | Tipo    | Descrição                                                            | Restrição |
|--------------------|---------|----------------------------------------------------------------------|-----------|
| unique_cod         | varchar | Código estável da linha de estoque; normalmente upper(nome_estoque) | Obrigatório |
| nome_estoque       | varchar | Nome do estoque, com até 200 caracteres                              | Obrigatório |
| clinica_unique_cod | varchar | Código da clínica do estoque                                         |           |

A view de destino usa upper(nome_estoque) como import_id de produto_estoque. O nome normalizado deve estar associado a uma única clínica na carga. Quando a clínica não é informada, a importação usa a clínica padrão.
