# Planos de Operadoras de Saúde
<p align="justify"> 
Descreve a estrutura de dados de planos de operadoras de saúde. A tabela de descrição dos campos abrange as principais informações dessas entidades.
 </p>

> Nome do arquivo de importação: `import_operadora_saude_plano.csv`

 ## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único, sem repetição, do plano da operadora de saúde                       |     Obrigatório            |
| nome               | varchar | Nome do plano da operadora de saúde                                       |   Obrigatório              |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| operadora_saude_unique_cod    | varchar     | Código da operadora de saúde                |     Obrigatório            |



## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_operadora_saude_plano.csv ':ignore')