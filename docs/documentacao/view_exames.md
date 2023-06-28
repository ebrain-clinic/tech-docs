# Prescrição de Exames
<p align="justify"> 
Este documento descreve os campos necessários para importar os dados de prescrições de exames no sistema Ebrain. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único para cada exame na prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código opcional para a pescrição                                       |    Obrigatório             |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| exame     | varchar   | Nome do exame                               |                 |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |                 |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, não estruturado                               |                 |
| obs_resultado_exame     | varchar   | Observações sobre os resultados                               |                 |
| json_resultados     | varchar   | Resultados em json      |                 |

  
## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo abaixo:</p>

[Clique aqui para baixar o arquivo csv](https://drive.google.com/uc?export=download&id=120j6HA2xM2J3bv5AJN8txxMt9ZVK_lYW)
