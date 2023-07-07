# Prescrição de Relatórios Médicos
<p align="justify"> 
Descreve a estrutura de dados de prescrições de relatórios médicos. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                             | Tipo      | Descrição                                                                 | Restrição   |
|-----------------------------------|-----------|--------------------------------------------------------------------------|---------------|
| unique_cod                        | varchar   | Código único sem repetição para cada linha de prescrição.                 | Obrigatório |
| data_informada                    | timestamp | Data informada na prescrição.                                             |             |
| data_exclusao                     | timestamp | Data da exclusão da prescrição.                                           |             |
| data_importacao                   | timestamp | Data em que ocorreu a importação do registro.                             | Obrigatório |
| pessoa_unique_cod                 | varchar   | Código do paciente vinculado à prescrição.                                | Obrigatório |
| profissional_unique_cod           | varchar   | Código do profissional que fez a prescrição.                              | Obrigatório |
| prontuario_unique_cod             | varchar   | Código do prontuário que contém a prescrição.                             | Obrigatório |
| documento_texto                   | varchar   | Prescrição textual que contém o conteúdo do relatório médico.             | Obrigatório |

## Arquivo
<p align="justify">Realize o dowload do arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/prescricao_relatorios.csv ':ignore')
