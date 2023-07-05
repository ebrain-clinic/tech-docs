# Prescrição de Exames
<p align="justify"> 
Descreve a estrutura de dados de prescrições de exames. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição para cada exame na prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código para a pescrição. Pode repetir, caso a prescrição seja estruturada e o campo `documento_nao_estruturado_texto` seja vazio para o primeiro caso de `prescricao_unique_cod` com a menor data em `data_prescricao`                                        |    Obrigatório             |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| exame     | varchar   | Nome do exame                               |   Obrigatório              |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |  Obrigatório               |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| exame_nome               | varchar | Nome do exame, caso a prescrição seja estruturada              | Obrigatório, se `documento_nao_estruturado_texto` estiver em branco                |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, caso a prescrição não seja estruturada                               | Obrigatório se `exame_nome` estiver em branco                |
| obs_resultado_exame     | varchar   | Observações sobre os resultados                               |                 |
| json_resultados     | varchar   | Resultados em json      |                 |

  
## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo abaixo:</p>

[Clique aqui para baixar o arquivo csv](https://drive.google.com/uc?export=download&id=120j6HA2xM2J3bv5AJN8txxMt9ZVK_lYW)
