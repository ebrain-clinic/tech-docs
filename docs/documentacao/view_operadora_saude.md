# Operadora de saúde
<p align="justify"> 
Descreve a estrutura de dados de operadoras de saúde, como convênios, planos de saúde, estruturas semelhantes. A tabela de descrição dos campos abrange as principais informações destas estidades.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| externo_cod                 | varchar     | Código único sem repetição da operadora de saúde                       |     Obrigatório            |
| nome               | varchar | Nome da operadora de saúde                                       |   Obrigatório              |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| registro_ans    | varchar     | Registro ANS da operadora de saúde                 |                 |
| codigo_na_operadora | varchar     |   Código usado na operadora                           |                 |
| versao_tiss            | varchar |    Versão do padrão TISS que a operadora usa       |                 |
| particular               | boolean | Indica se é particular                    |                 |
| cortesia     | boolean   | Indica se é cortesia                                  |                 |


## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/operadora_saude.csv ':ignore')