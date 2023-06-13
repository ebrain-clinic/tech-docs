# Evolução
<p align="justify"> 
Neste documento, estão descritos os campos necessários para importar os dados de evoluções dos pacientes no sistema Ebrain. Essas evoluções ajudam no acompanhamento dos pacientes e podem incluir, por exemplo, prontuários, anamneses e históricos. Por convenção, neste documento, estas evoluções são denominadas prontuários. É comum a descrição do prontuário estar em formato HTML e RTF.
 </p>

## Descrição dos campos

| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| externo_cod                 | varchar     | Código único do prontuário                       |     Obrigatório            |
| data_registro               | timestamp | Data e hora de registro do prontuário                                       |   Obrigatório              |
| pessoa_externo_cod          | varchar     | Código do paciente relacionado ao prontuário                          |  Obrigatório               |
| profissional_externo_cod    | varchar     | Código do profissional relacionado ao prontuário                    |     Obrigatório            |
| prontuario_diagnostico_nome | varchar     | Descrição do diagnóstico associado ao prontuário                                 |                 |
| data_atualizacao            | timestamp | Data e hora da última atualização do prontuário              |                 |
| data_exclusao               | timestamp | Data e hora de exclusão do prontuário                        |                 |
| diag_evolucao_descricao     | varchar   | Descrição do prontuário                                      | Obrigatório                |
| diag_evolucao_adendo        | boolean | Indica se existe um adendo relacionado ao prontuário           |                 |
| diag_evolucao_data_exclusao | timestamp | Data e hora de exclusão do prontuário                         |                 |


