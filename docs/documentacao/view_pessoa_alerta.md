# Alertas de Pacientes

<p align="justify"> 
Descreve a estrutura de dados de alertas de pacientes: informações importantes a respeito do paciente não pertencentes ao prontuário médico mas importantes para o atendimento. A tabela de descrição dos campos abrange as principais informações desses alertas.
</p>

> Nome do arquivo de importação: `import_pessoa_alerta.csv` 

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do alerta                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| data_exclusao    | timestamp     | Data de exclusão               |                 |
| descricao               | varchar | Descrição do alerta                                   |   Obrigatório              |
| concluido          | boolean     | Indica se foi concluído                  |   Obrigatório              |
| profissional_unique_cod            | varchar |  Código do profissional que escreveu o alerta         |      Obrigatório           |



## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_pessoa_alerta.csv ':ignore')