# Prescrição de Medicamentos
<p align="justify"> 
Descreve a estrutura de dados de prescrições de medicamentos. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição para cada linha de prescrição                       |  Obrigatório            |
| prescricao_unique_cod     | varchar | Código da pescrição. Pode repetir caso a prescrição seja estruturada. Nesse caso o campo `documento_nao_estruturado_texto` será vazio e haverá uma ou mais linhas com diferentes conteúdos no campo `medicamento_nome`                                       |  Obrigatório               |
| data_prescricao          | timestamp     | Data da pescrição                |                 |
| data_registro    | timestamp     | Data em que ocorreu o registro   | Obrigatório                |
| data_exclusao | timestamp     |   Data da exclusão da prescrição       |                 |
| pessoa_unique_cod            | varchar | Paciente vinculado à prescrição    |   Obrigatório              |
| profissional_unique_cod               | varchar | Código do profissional que fez a prescrição              |  Obrigatório               |
| documento_nao_estruturado_texto     | varchar   | Documento de prescrição textual,  caso a prescrição não seja estruturada                                |  Obrigatório se `medicamento_nome` estiver em branco                |
| medicamento_nome     | varchar   | Nome do medicamento, no caso de prescrição estruturada                               |  Obrigatório se `documento_nao_estruturado_texto` estiver em branco               |
| medicamento_descricao     | varchar   | Descrição do medicamento, no caso de prescrição estruturada                              | Não deve ser informado se `documento_nao_estruturado_texto` for preenchido                |
| medicamento_posologia     | varchar   | Posologia do medicamento, no caso de prescrição estruturada                               | Não deve ser informado se `documento_nao_estruturado_texto` for preenchido                |
| medicamento_composicao     |  varchar  | Composição do medicamento, no caso de prescrição estruturada                        | Não deve ser informado se `documento_nao_estruturado_texto` for preenchido                |
| medicamento_uso     |  varchar |  Descrição do uso, no caso de prescrição estruturada. Sugestões do sistema: tópico, interno, externo, oral, nasal, intralesional, intramuscular, endovenoso               | Não deve ser informado se `documento_nao_estruturado_texto` for preenchido                |
| medicamento_tarja     |  varchar  | Indica a tarja do medicamento, no caso de prescrição estruturada. Sugestões: tarja vermelha, tarja preta, tarja amarela...                      | Não deve ser informado se `documento_nao_estruturado_texto` for preenchido                |

## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/prescricao_medicamento.csv ':ignore')