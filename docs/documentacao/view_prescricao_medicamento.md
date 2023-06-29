# Prescrição de Medicamentos
<p align="justify"> 
Este documento descreve os campos necessários para importar os dados de prescrições de medicamento no sistema Ebrain. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único para cada medicamento na prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código da pescrição                                       |  Obrigatório               |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |   Obrigatório              |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |  Obrigatório               |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, não estruturado                               |                 |
| medicamento_nome     | varchar   | Nome do medicamento                               |                 |
| medicamento_descricao     | varchar   | Descrição do medicamento                              |                 |
| medicamento_posologia     | varchar   | Posologia do medicamento                               |                 |
| medicamento_composicao     |  varchar  | Composição do medicamento                        |                 |
| medicamento_uso     |  varchar |  Descrição do uso. Sugestões do sistema: tópico, interno, externo, oral, nasal, intralesional, intramuscular, endovenoso               |                 |
| medicamento_tarja     |  varchar  | Indica a tarja do medicamento. Sugestões: tarja vermelha, tarja preta, tarja amarela...                      |                 |

## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo abaixo:</p>

[Clique aqui para baixar o arquivo csv](https://drive.google.com/uc?export=download&id=1Y2oRkr6LkonyFtLaKompIE4wjeBKk2yv)
