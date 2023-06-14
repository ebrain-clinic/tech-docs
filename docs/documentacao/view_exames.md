# Prescrição de Exames
<p align="justify"> 
Neste documento, estão descritos os campos necessários para importar os dados de prescrições de exames no sistema Ebrain. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| externo_cod                 | varchar     | Código único para cada exame na prescrição                       |  Obrigatório            |
| prescricao_opcional_externo_cod     | varchar | Código opcional para a pescrição                                       |                 |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| exame     | varchar   | Nome do exame                               |                 |
| pessoa_externo_cod            | varchar | Paciente vinculado à prescrição    |                 |
| profissional_externo_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, não estruturado                               |                 |
| obs_resultado_exame     | varchar   | Observações sobre os resultados                               |                 |
| json_resultados     | varchar   | Resultados em json      |                 |

  