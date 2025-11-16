| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição para cada exame na prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código para a pescrição. Pode repetir caso a prescrição seja estruturada. Nesse caso o campo `documento_nao_estruturado_texto` será vazio e haverá uma ou mais linhas com diferentes conteúdos no campo `exame_nome`                                        |    Obrigatório             |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| data_atualizacao | timestamp | Data da última atualização da prescrição |  |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |  Obrigatório               |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |                 |
| exame_nome               | varchar | Nome do exame, caso a prescrição seja estruturada              | Obrigatório se `documento_nao_estruturado_texto` estiver em branco                |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual, caso a prescrição não seja estruturada                               | Obrigatório se `exame_nome` estiver em branco                |
| texto_resultados     | varchar   | Resultados em formato de texto                               |                 |
| json_resultados     | varchar   | Resultados estruturados em json      |                 |
| observacao | varchar | Observações adicionais sobre a prescrição |  |
| inclusor_unique_cod            | varchar |  Código do usuário que incluiu a prescrição | |
| prontuario_especialidade_cod | int | Código da especialidade de prontuário associada (se houver) |  |
