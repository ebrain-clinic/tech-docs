# Evolução
<p align="justify"> 
Descreve a estrutura de dados de evoluções dos pacientes. As evoluções representam o histórico do prontuário médico dos pacientes e podem incluir, por exemplo, anamneses, procedimentos realizados, históricos e observações em geral. Por convenção, neste documento, essas evoluções são denominadas prontuários. 
 </p>
 A descrição do prontuário deve estar preferencialmente no formato de texto puro, sem formatação, embora descrições no formato HTML e RTF também sejam aceitas. Neste caso, o conteúdo do prontuário será convertido para texto simples, sem formatação, antes de ser importado.

> Nome do arquivo de importação: `import_evolucao.csv`


## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição                        |     Obrigatório            |
| data_registro               | timestamp | Data e hora de registro do prontuário                                       |   Obrigatório              |
| pessoa_unique_cod          | varchar     | Código do paciente relacionado ao prontuário                          |  Obrigatório               |
| profissional_unique_cod    | varchar     | Código do profissional relacionado à prescrição da evolução |     Obrigatório se inclusor_unique_cod nulo |
| prontuario_diagnostico_nome | varchar     | Descrição do diagnóstico associado ao prontuário. Exemplo: Queda de cabelo. As evoluções de um mesmo diagnóstico serão agrupadas no prontuário do cliente                                 |                 |
| data_atualizacao            | timestamp | Data e hora da última atualização do prontuário              |                 |
| data_exclusao               | timestamp | Data e hora de exclusão do prontuário                        |                 |
| diag_evolucao_descricao     | varchar   | Evolução em si. Preferencialmente em formato texto simples.                                      | Obrigatório                |
| diag_evolucao_descricao_html     | varchar   | Evolução no formato HTML                             | Opcional                |
| diag_evolucao_adendo        | boolean | Indica se existe um complemento relacionado ao prontuário           |                 |
| diag_evolucao_data_exclusao | timestamp | Data e hora de exclusão do prontuário                         |                 |
| inclusor_unique_cod    | varchar     | Código do usuário relacionado à prescrição da evolução | Obrigatório se profissional_unique_cod nulo |




## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_evolucao.csv ':ignore')
