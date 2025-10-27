| Campo                       | Tipo        | Descrição                                                                                     | Restrição       |
|-----------------------------|-------------|---------------------------------------------------------------------------------------------|-----------------|
| unique_cod                  | varchar     | Código único da clínica                                                                     | Obrigatório     |
| principal                   | boolean     | Indica se é a clínica principal                                                            |         |
| nome                        | varchar     | Nome oficial da clínica                                                                    | Obrigatório     |
| nome_fantasia               | varchar     | Nome fantasia da clínica                                                                   |         |
| cpf                         | varchar     | CPF associado à clínica (se aplicável)                                                    |         |
| cnpj                        | varchar     | CNPJ da clínica                                                                            |      |
| cnes                        | varchar     | Código CNES da clínica                                                                     |         |
| email_contato_principal     | varchar     | E-mail de contato principal da clínica                                                    |         |
| telefone_contato_principal  | varchar     | Telefone de contato principal da clínica                                                  |         |
| data_registro               | timestamp   | Data de registro da clínica                                                                | Obrigatório     |
| horario_comercial_inicio    | time        | Horário de início do funcionamento comercial                                               |         |
| horario_comercial_fim       | time        | Horário de término do funcionamento comercial                                              |         |
| end1_logradouro             | varchar     | Logradouro do endereço principal da clínica                                                |         |
| end1_numero                 | varchar     | Número do endereço principal da clínica                                                   |         |
| end1_complemento            | varchar     | Complemento do endereço principal da clínica                                              |         |
| end1_bairro                 | varchar     | Bairro do endereço principal da clínica                                                   |         |
| end1_cep                    | varchar     | CEP do endereço principal da clínica                                                      |         |
| end1_municipio              | varchar     | Nome do município do endereço principal da clínica                                         |         |
| end1_uf_id                  | varchar     | Sigla do estado (UF) do endereço principal da clínica                                      |         |
| clinica_especialidade       | varchar     | Especialidades associadas à clínica                                                       | Obrigatório        |
