# Prescrição de Exames
<p align="justify"> 
Descreve a estrutura de dados de prescrições de exames. A tabela de descrição dos campos abrange as principais informações dessas prescrições.
 </p>

> Nome do arquivo de importação: `import_prescricao_exame.csv`


 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição para cada exame na prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código para a pescrição. Pode repetir caso a prescrição seja estruturada. Nesse caso o campo `documento_nao_estruturado_texto` será vazio e haverá uma ou mais linhas com diferentes conteúdos no campo `exame_nome`                                        |    Obrigatório             |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |  Obrigatório               |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| exame_nome               | varchar | Nome do exame, caso a prescrição seja estruturada              | Obrigatório se `documento_nao_estruturado_texto` estiver em branco                |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, caso a prescrição não seja estruturada                               | Obrigatório se `exame_nome` estiver em branco                |
| texto_resultados     | varchar   | Resultados em formato de texto                               |                 |
| json_resultados     | varchar   | Resultados estruturados em json      |                 |
| inclusor_unique_cod            | varchar |  Código do usuário que incluiu a prescrição | |

  
## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_prescricao_exame.csv ':ignore')
