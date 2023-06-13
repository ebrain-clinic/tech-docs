# Pessoa
<p align="justify"> 
Neste documento são descritos os campos necessários para importar os dados de pacientes no sistema Ebrain. A tabela de descrição dos campos se caracteriza por possuir os dados principais dos pacientes, incluindo endereço, telefone e dados básicos.
 </p>

## Descrição dos campos
| Campo                       | Tipo  | Descrição                                                                                        | Restrição        |
|-----------------------------|-------|--------------------------------------------------------------------------------------------------|------------------|
| externo_cod  | varchar | Chave primária da pessoa | Obrigatório |
| codigo_nas_clinicas | varchar  | Número que a clínica possa ter do cliente e que não seja a chave primária |      |
| data_registro   | timestamp  | Data de registro da pessoa                                                                      | Obrigatório      |
| tratamento                  | varchar  |   Descrição de tratamento |                  |
| nome_civil_razao_social     | varchar  | Nome civil ou razão social da pessoa                                                             | Obrigatório      |
| nome_social                 | varchar  | Nome pelo qual o paciente quer ser chamado   |     |
| data_nascimento             | date  | Data de nascimento da pessoa  | |
| sexo_biologico_ao_nascer    | varchar  | Sexo biológico ao nascer da pessoa   |       |
| cpf     | varchar  | CPF da pessoa  |       |
| rg | varchar  | RG da pessoa   |       |
| rg_orgao    | varchar  | Orgão emissor do RG   |                  |
| cns   | varchar  | Número do cartão nacional de saúde | |
| naturalidade    | varchar  | Naturalidade da pessoa |  |
| raca      | varchar  | Raça da pessoa  |                  |
| estado_civil    | varchar  | Estado civil da pessoa  |    |
| profissao_principal_id      | int   | ID da profissão principal da pessoa       |   |
| ocupacao_outros             | varchar  | Ocupação da pessoa   |       |
| local_trabalho              | varchar  | Local de trabalho da pessoa      |                  |
| obito_encerrado             | bool  | Indica se o óbito está encerrado| |
| tipo_pessoa   | varchar  | Tipo de pessoa (PF - Pessoa Física), (PJ - Pessoa Jurídica) | Obrigatório      |
| preferencial  | bool  | Indica se é preferencial  |   |
| nome_mae   | varchar  | Nome da mãe da pessoa  |       |
| nome_pai        | varchar  | Nome do pai da pessoa |                  |
| como_conheceu_detalhes      | varchar  | Detalhes de como a pessoa conheceu a clínica        |                  |
| observacoes     | varchar  | Observações sobre a pessoa  |           |
| end1_label    | varchar  | Rótulo do endereço principal                  |       |
| end1_logradouro  | varchar  | Logradouro do endereço principal           |       |
| end1_numero    | varchar  | Número que faz parte do endereço|                  |
| end1_complemento            | varchar  | Complemento do endereço principal                                                                |                  |
| end1_bairro                 | varchar  | Bairro do endereço principal                                                                     |       |
| end1_cep                    | varchar  | CEP do endereço principal                                                                        |       |
| end1_municipio_id           | int   | ID do município do endereço principal                                                            | Obrigatório      |
| end1_uf_id                  | int   | ID do estado do endereço principal                                                               | Obrigatório      |
| contato1_descricao          | varchar  | Descrição do contato 1                                                                            |                  |
| contato1_telefone_ddd       | int  | DDD do telefone do contato 1                                                                     |                  |
| contato1_telefone_numero    | int  | Número do telefone do contato 1                                                                  |                  |
| contato1_telefone_completo  | varchar  | Número completo do telefone do contato formato: (99)  99 999999999                                                         |                  |
| contato1_preferido          | bool  | Indica se o contato 1 é preferido             |         Obrigatório         |
| contato1_tipo_contato_id    | int   | ID do tipo de contato do contato 1 (1 - celular, 2 - fixo)     |      Obrigatório            |
| contato1_receber_propagandas | bool  | Indica se o contato 1 deseja receber propagandas       |     Obrigatório             |
| contato1_receber_confirmacoes| bool  | Indica se o contato 1 deseja receber confirmações       |      Obrigatório            |
| contato1_possui_whatsapp    | bool  | Indica se o contato 1 possui WhatsApp                 |         Obrigatório         |
| contato2_descricao          | varchar  | Descrição do contato 2           |                  |
| contato2_telefone_ddd       | int  | DDD do telefone do contato 2                                                                     |                  |
| contato2_telefone_numero    | int  | Número do telefone do contato 2                                                                  |                  |
| contato2_telefone_completo  | varchar  | Número completo do telefone do contato 2                                                         |                  |
| contato2_preferido          | bool  | Indica se o contato 2 é preferido         |  Obrigatório      |
| contato2_tipo_contato_id    | int   | ID do tipo de contato do contato 2 (1 - celular, 2 - fixo)    |    Obrigatório              |
| contato2_receber_propagandas | bool  | Indica se o contato 2 deseja receber propagandas               |     Obrigatório             |
| contato2_receber_confirmacoes| bool  | Indica se o contato 2 deseja receber confirmações              |        Obrigatório          |
| contato2_possui_whatsapp    | bool  | Indica se o contato 2 possui WhatsApp                    |         Obrigatório         |
| contato3_descricao | varchar | Descrição do contato 3 | |
| contato3_telefone_ddd | int | DDD do telefone do contato 3 | |
| contato3_telefone_numero | int | Número do telefone do contato 3 | |
| contato3_telefone_completo | varchar | Número completo do telefone do contato 3 | |
| contato3_preferido | bool | Indica se o contato 3 é preferido | Obrigatório |
| contato3_tipo_contato_id | int | ID do tipo de contato do contato 3 (1 - celular, 2 - fixo) | Obrigatório |
| contato3_receber_propagandas | bool | Indica se o contato 3 deseja receber propagandas | Obrigatório |
| contato3_receber_confirmacoes| bool | Indica se o contato 3 deseja receber confirmações | Obrigatório |
| contato3_possui_whatsapp | bool | Indica se o contato 3 possui WhatsApp | Obrigatório |
| contato4_descricao | varchar | Descrição do contato 4 | |
| contato4_telefone_ddd | int | DDD do telefone do contato 4 | |
| contato4_telefone_numero | int | Número do telefone do contato 4 | |
| contato4_telefone_completo | varchar | Número completo do telefone do contato 4 | |
| contato4_preferido | bool | Indica se o contato 4 é preferido | Obrigatório |
| contato4_tipo_contato_id | int | ID do tipo de contato do contato 4 (1 - celular, 2 - fixo) | Obrigatório |
| contato4_receber_propagandas | bool | Indica se o contato 4 deseja receber propagandas | Obrigatório |
| contato4_receber_confirmacoes| bool | Indica se o contato 4 deseja receber confirmações | Obrigatório |
| contato4_possui_whatsapp | bool | Indica se o contato 4 possui WhatsApp | Obrigatório |
| email1_descricao            | varchar  | Descrição do email 1      |         |
| email1_endereco              | varchar  | Endereço de email 1     |   |
| email1_preferido| bool  | Indica se o email 1 é preferido                                                            |     Obrigatório             |
| email1_receber_propagandas   | bool  | Indica se o email 1 deseja receber propagandas    |      Obrigatório            |
| email1_receber_confirmacoes  | bool  | Indica se o email 1 deseja receber confirmações    |          Obrigatório        |
| email2_descricao | varchar | Descrição do email 2 | |
| email2_endereco | varchar | Endereço de email 2 |  |
| email2_preferido| bool | Indica se o email 2 é preferido | Obrigatório |
| email2_receber_propagandas | bool | Indica se o email 2 deseja receber propagandas | Obrigatório |
| email2_receber_confirmacoes | bool | Indica se o email 2 deseja receber confirmações | Obrigatório |
| email3_descricao | varchar | Descrição do email 3 | |
| email3_endereco | varchar | Endereço de email 3 |  |
| email3_preferido| bool | Indica se o email 3 é preferido | Obrigatório |
| email3_receber_propagandas | bool | Indica se o email 3 deseja receber propagandas | Obrigatório |
| email3_receber_confirmacoes | bool | Indica se o email 3 deseja receber confirmações | Obrigatório |
| email4_descricao | varchar | Descrição do email 4 | |
| email4_endereco | varchar | Endereço de email 4 |  |
| email4_preferido| bool | Indica se o email 4 é preferido | Obrigatório |
| email4_receber_propagandas | bool | Indica se o email 4 deseja receber propagandas | Obrigatório |
| email4_receber_confirmacoes | bool | Indica se o email 4 deseja receber confirmações | Obrigatório |



## Lista de Siglas e Padrões de Nomenclatura dos Campos

### sexo_biologico_ao_nascer

| Descrição  | sigla |
|------------|-------|
| Masculino  |   M   |
| Feminino   |   F   |




### estado_civil

| Nomenclatura padrão |
|---------------------|
| CASADO              |
| SOLTEIRO            |
| DIVORCIADO          |
| VIUVO               |



## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo abaixo:</p>