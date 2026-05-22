| Campo                | Tipo      | Descrição                                                            | Restrição   |
|----------------------|-----------|----------------------------------------------------------------------|-------------|
| unique_cod           | varchar   | Código único sem repetição do produto                                | Obrigatório |
| nome                 | varchar   | Nome completo do produto                                             | Obrigatório |
| nome_curto           | varchar   | Nome curto ou comercial do produto                                   |             |
| data_registro        | timestamp | Data de registro do produto                                          | Obrigatório |
| data_exclusao        | timestamp | Data de exclusão lógica do produto                                   |             |
| controlar_estoque    | boolean   | Indica se o produto deve ser controlado no estoque                   | Obrigatório |
| nome_principio_ativo | varchar   | Nome do princípio ativo do produto                                   |             |
| clinica_unique_cod   | varchar   | Código único da clínica do cadastro, quando houver mais de uma clínica |             |
