# Prontuário de Alergia
<p align="justify"> 
Descreve a estrutura de dados dos antecedentes dos pacientes, os quais estão ligados ao prontuário médico, permitindo que os profissionais de saúde tomem decisões informadas durante o atendimento médico. A tabela de descrição dos campos abrange as principais informações desses antecedentes.
 </p>

> Nome do arquivo de importação: `import_prontuario_alergia`

## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição da alergia                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| nome          | varchar     | Nome da alergia                        |   Obrigatório              |
| observacao    |  varchar    | Observações à respeito da alergia               |                 |
| relevante_prescricoes               | boolean | Se possui prescrições relevantes                                  |   Obrigatório              |
| data_registro          | timestamp     |   Data do registro                |   Obrigatório              |
| data_fim |timestamp | Data fim da alergia | |
| profissional_unique_cod            | varchar |  Código do profissional que registrou as alergias         |      Obrigatório           |


## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/prontuario_alergia.csv ':ignore')