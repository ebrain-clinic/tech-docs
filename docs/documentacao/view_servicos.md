# Serviços
<p align="justify"> 
Descreve a estrutura de dados de serviços ou procedimentos realizados pela clínica. A tabela de descrição dos campos abrange as principais informações desses serviços médicos.
 </p>

> Nome do arquivo de importação: `import_servico`

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do serviço                       |     Obrigatório            |
| nome               | varchar | Nome do serviço                                      |   Obrigatório              |
| data_inicio          | timestamp     | Data do ínicio deste serviço                   |   Obrigatório              |
| data_importacao    | timestamp     | Data que ocorreu a importação     |                 |
| data_fim | Timestamp     |   Data que o serviço parou de ser realizado        |                 |
| agendavel            | boolean |   Indica se é agendavel      |                 |
| agendavel_via_app               | boolean | Indica se é agendável via app                 |                 |
| gratuito     | boolean   | Indica se é um serviço gratuito                                  |                 |
| atende_particular     | boolean   | Indica se aceita atendimento particular                                  |                 |
| atende_convenio     | boolean   | Indica se aceita convênio médico                                 |                 |
| especialidade_id     | boolean   | Especialidade do serviço                                 |                 |
| valor_particular     |  decimal(10, 2)   | Valor do serviço particular                           |                 |


## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/servico.csv ':ignore')