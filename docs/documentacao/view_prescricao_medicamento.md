# Prescrição de Medicamentos
<p align="justify"> 
Neste documento, estão descritos os campos necessários para importar os dados de prescrições de medicamento no sistema Ebrain. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| externo_cod                 | varchar     | Código único para cada medicamento na prescrição                       |  Obrigatório            |
| prescricao_opcional_externo_cod     | varchar | Código opcional para a pescrição                                       |                 |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| pessoa_externo_cod            | varchar | Paciente vinculado à prescrição    |                 |
| profissional_externo_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, não estruturado                               |                 |
| medicamento_nome     | varchar   | Nome do medicamento                               |                 |
| medicamento_descricao     | varchar   | Descrição do medicamento                              |                 |
| medicamento_posologia     | varchar   | Posologia do medicamento                               |                 |
| medicamento_composicao     |  varchar  | Composição do medicamento                        |                 |
| medicamento_uso     |  varchar |  Descrição do uso. Sugestões do sistema: tópico, interno, externo, oral, nasal, intralesional, intramuscular, endovenoso               |                 |
| medicamento_tarja     |  varchar  | Indica a tarja do medicamento                     |                 |
