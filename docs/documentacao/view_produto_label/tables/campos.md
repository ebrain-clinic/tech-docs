| Campo                            | Tipo      | Descrição                                                                                      | Restrição   |
|----------------------------------|-----------|------------------------------------------------------------------------------------------------|-------------|
| unique_cod                       | varchar   | Código único sem repetição do vínculo entre produto e label                                    | Obrigatório |
| data_registro                    | timestamp | Data de registro do vínculo                                                                    | Obrigatório |
| data_exclusao                    | timestamp | Data de exclusão lógica do vínculo                                                             |             |
| produto_unique_cod               | varchar   | Código único do produto relacionado (ver [produtos](documentacao/view_produto/))               | Obrigatório |
| label_unique_cod                 | varchar   | Código único da label de produto. Para labels criadas por `nome_tag`, use `nome_tag` com sufixo `-pd` | Obrigatório |
| nome_tag                         | varchar   | Nome da label exibida no sistema                                                               | Obrigatório |
