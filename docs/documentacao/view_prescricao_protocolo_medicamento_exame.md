# Prescrição de Protocolos de Medicamentos e Exames
<p align="justify"> 
Descreve a estrutura de dados de prescrições de protocolos de medicamentos e exames. A tabela de descrição dos campos abrange as principais informações dessas prescrições.
 </p>

> Nome do arquivo de importação: `import_prescricao_protocolo_medicamento_exame.csv`


## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do medicamento                     |     Obrigatório            |
| protocolo_unique_cod | varchar     | Código do protocolo. Pode repetir quando existem vários medicamentos no mesmo protocolo.                         |      Obrigatório           |
| data_registro          | timestamp     |   Data do registro                |   Obrigatório              |
| medicamento_exame_nome     | varchar   | Nome do medicamento ou exame  |               |
| medicamento_descricao     | varchar   | Descrição do medicamento                              |                 |
| medicamento_posologia     | varchar   | Posologia do medicamento                            |                |
| medicamento_composicao     |  varchar  | Composição do medicamento                     |                |
| medicamento_uso     |  varchar |  Descrição do uso. Sugestões do sistema: tópico, interno, externo, oral, nasal, intralesional, intramuscular, endovenoso               |               |
| medicamento_tarja     |  varchar  | Indica a tarja do medicamento. Sugestões: tarja vermelha, tarja preta, tarja amarela...                      |               |
| categoria_exame_medicamento     |  varchar  | Indica se é medicamento (MED) ou exame (EXA)                | Obrigatório|
| protocolo_nome     |  varchar  | Nome do protocolo| Obrigatório|
| total_referencias     |  integer  |Número de referências| |
| data_atualizacao     |  timestamp  |Data de atualização| |
| data_exclusao     |  timestamp  |Data de exclusão| |
| indicacoes_clinicas     |  varchar  |Indicações clínicas para uso do protocolo| |
| protocolo_categoria     |  varchar  |Categoria do protocolo| |
| profissional_unique_cod     |  varchar  | Código único do profissional| Obrigatório |
| visivel_para_outros_profissionais     |  boolean  |Indica se o protocolo pode ficar visível para os outros profissionais| Obrigatório |
| observacao     |  varchar  | Observações sobre o protocolo| |
| composto_por_exames     |  boolean  | Indica se o protocolo é composto por exames| |
| composto_por_medicamentos     |  boolean  | Indica se o protocolo é composto por medicamentos| |
| protocolo_especialidade     |  varchar  | especialidade do protocolo| Obrigatório |



## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_prescricao_protocolo_medicamento_exame.csv ':ignore')



