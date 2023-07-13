# Atestados Médicos
<p align="justify"> 
Descreve a estrutura de dados de emissão de atestados médicos. A tabela de descrição dos campos abrange as principais informações destas prescrições.
 </p>

 ## Descrição dos campos

| Campo                             | Tipo      | Descrição                                                                 | Restrição   |
|-----------------------------------|-----------|--------------------------------------------------------------------------|--------------|
| unique_cod                        | varchar   | Código único sem repetição para cada linha de prescrição.                 | Obrigatório |
| data_informada                    | timestamp | Data informada no documento.                                             |             |
| data_exclusao                     | timestamp | Data da exclusão do documento.                                           |             |
| pessoa_unique_cod                 | varchar   | Código do paciente vinculado ao documento.                                | Obrigatório |
| profissional_unique_cod           | varchar   | Código do profissional que fez o documento.                              | Obrigatório |
| prontuario_unique_cod             | varchar   | Código do prontuário que contém o documento.                             | Obrigatório |
| documento_texto                   | varchar   | Prescrição textual que contém o conteúdo do atestado médico.              | Obrigatório |

## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/prescricao_atestados.csv ':ignore')
