| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição da operadora de saúde                       |     Obrigatório            |
| nome               | varchar | Nome da operadora de saúde                                       |   Obrigatório              |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| registro_ans    | varchar     | Registro ANS da operadora de saúde                 |                 |
| codigo_na_operadora | varchar     |   Código usado na operadora                           |                 |
| versao_tiss            | varchar |    Versão do padrão TISS que a operadora usa       |                 |
| data_exclusao          | timestamp | Data de exclusão da operadora                      |                 |
| particular               | boolean | Indica se é particular                    |                 |
| cortesia     | boolean   | Indica se é cortesia                                  |                 |
