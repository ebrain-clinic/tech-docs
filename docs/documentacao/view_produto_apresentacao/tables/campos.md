| Campo                  | Tipo      | Descrição                                                                  | Restrição   |
|------------------------|-----------|----------------------------------------------------------------------------|-------------|
| unique_cod             | varchar   | Código único sem repetição da apresentação do produto                       | Obrigatório |
| nome                   | varchar   | Nome da apresentação                                                        | Obrigatório |
| unidade                | varchar   | Unidade da apresentação como um todo. Ex.: Frasco, Ampola, Caixa, Unidade   | Obrigatório |
| generico               | boolean   | Indica se a apresentação é de produto genérico                              | Obrigatório |
| produto_unique_cod     | varchar   | Código único do produto relacionado (ver [produtos](documentacao/view_produto/)) | Obrigatório |
| quantidade             | decimal   | Quantidade da fração contida na apresentação                                | Obrigatório |
| data_exclusao          | timestamp | Data de exclusão lógica da apresentação                                     |             |
| fracao_unidade         | varchar   | Unidade da fração (unidade de saída) da apresentação. Ex.: Unidade, mL, Comprimido |             |
| uso_fracionado         | boolean   | Indica se a apresentação permite uso fracionado                             | Obrigatório |
| clinica_unique_cod     | varchar   | Código único da clínica do cadastro, quando houver mais de uma clínica      |             |
| laboratorio_unique_cod | varchar   | Código único do laboratório relacionado (ver [laboratórios](documentacao/view_laboratorio/)) |             |
| laboratorio_nome       | varchar   | Nome do laboratório, usado para localizar um laboratório existente pelo nome |             |
