# Prontuário de Antecedentes
<p align="justify"> 
Descreve a estrutura de dados dos antecedentes dos pacientes que estão ligados ao prontuário médico, permitindo que os profissionais de saúde tomem decisões informadas durante o atendimento médico. A tabela de descrição dos campos abrange as principais informações desses antecedentes.
 </p>

> Nome do arquivo de importação: `import_prontuario_antecedente.csv`

## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do antecedente                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| descricao          | varchar     | Descrição dos antecedentes                        |   Obrigatório              |
| privado               | boolean | Se é privado                                  |                 |
| data_registro          | timestamp     |   Data do registro                |   Obrigatório              |
| inclusor_unique_cod            | varchar |  Código do usuário que registrou os antecedentes         |      Obrigatório           |


## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_prontuario_antecedente.csv ':ignore')
