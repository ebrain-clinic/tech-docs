# Alertas de Pacientes
<p align="justify"> 
Descreve a estrutura de dados de alertas de pacientes, ou seja, quaisquer observações que o médico queira ver na hora do atendimento. A tabela de descrição dos campos abrange as principais informações destes alertas.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do alerta                     |     Obrigatório            |
| descricao               | varchar | Descriçao do alerta                                   |   Obrigatório              |
| concluido          | boolean     | Se foi concluído                  |   Obrigatório              |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| data_exclusao    | timestamp     | Data de exclusão               |                 |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| profissional_unique_cod            | varchar |  Código do profissional que escreveu o alerta         |      Obrigatório           |



## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/pessoa_alerta.csv ':ignore')