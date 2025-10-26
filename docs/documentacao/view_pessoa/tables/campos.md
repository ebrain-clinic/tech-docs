| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição da pessoa | Obrigatório |
| codigo_nas_clinicas | varchar | Número que a clínica possa ter do cliente e que não seja a chave primária |  |
| data_registro | timestamp | Data de registro da pessoa | Obrigatório |
| tratamento | varchar | Descrição de tratamento |  |
| nome_civil_razao_social | varchar | Nome civil da pessoa ou razão social da empresa | Obrigatório |
| nome_social | varchar | Nome pelo qual o paciente quer ser chamado |  |
| data_nascimento | date | Data de nascimento da pessoa |  |
| sexo_biologico_ao_nascer | varchar | Sexo biológico ao nascer da pessoa |  |
| cpf | varchar | CPF da pessoa |  |
| rg | varchar | RG da pessoa |  |
| rg_orgao | varchar | Orgão emissor do RG |  |
| cns | varchar | Número do cartão nacional de saúde |  |
| naturalidade | varchar | Naturalidade da pessoa |  |
| nacionalidade | varchar | Nacionalidade da pessoa |  |
| escolaridade | varchar | Escolaridade da pessoa, conforme tabela própria em `escolaridade` |  |
| raca | varchar | Raça da pessoa |  |
| estado_civil | varchar | Estado civil da pessoa |  |
| nome_conjuge | varchar | Nome do cônjuge |  |
| profissao | varchar | Nome da profissão da pessoa (com base no CBO - IBGE) |  |
| ocupacao_outros | varchar | Ocupação da pessoa |  |
| local_trabalho | varchar | Local de trabalho da pessoa |  |
| obito_encerrado | boolean | Indica se o óbito está encerrado |  |
| tipo_pessoa | varchar | Tipo de pessoa (`PF`: Pessoa Física), (`PJ`: Pessoa Jurídica) | Obrigatório |
| preferencial | boolean | Indica se é preferencial |  |
| tipo_sanguineo | varchar | Tipo sanguíneo da pessoa, conforme tabela própria em `tipo_sanguineo` |  |
| nome_mae | varchar | Nome da mãe da pessoa |  |
| nome_pai | varchar | Nome do pai da pessoa |  |
| como_conheceu_detalhes | varchar | Detalhes de como a pessoa conheceu a clínica |  |
| observacoes | varchar | Observações sobre a pessoa |  |
| end1_label | varchar | Rótulo do endereço principal |  |
| end1_logradouro | varchar | Logradouro do endereço principal |  |
| end1_numero | varchar | Número que faz parte do endereço |  |
| end1_complemento | varchar | Complemento do endereço principal |  |
| end1_bairro | varchar | Bairro do endereço principal |  |
| end1_cep | varchar | CEP do endereço principal |  |
| end1_municipio_codigo_ibge | int | ID do município do endereço principal, conforme tabela de códigos dos municípios do IBGE, disponível [aqui](https://www.ibge.gov.br/explica/codigos-dos-municipios). | Obrigatório se end1_municipio_nome nulo |
| end1_municipio_nome | varchar | Nome do município do endereço principal. É extraído da base da Ebrain através do município fornecido. | Obrigatório se end1_municipio_id nulo |
| end1_uf_sigla | varchar | Sigla da Unidade da Federação do endereço principal, conforme tabela de domínio | Obrigatório |
| end1_cidade_nome_internacional | varchar | Nome da cidade do endereço caso seja um endereço internacional |  |
| end1_pais_unique_cod | int | Código identificador do país do endereço caso seja um endereço internacional |  |
| contato1_descricao | varchar | Descrição do contato 1 |  |
| contato1_telefone_ddd | int | DDD do telefone do contato 1 |  |
| contato1_num_ddi | int | DDI do telefone do contato 1 |  |
| contato1_telefone_numero | int | Número do telefone do contato 1 |  |
| contato1_telefone_completo | varchar | Número completo do telefone do contato formato: (99)  99 999999999 |  |
| contato1_preferido | boolean | Indica se o contato 1 é preferido | Obrigatório se `contato1_telefone_numero` preenchido |
| contato1_tipo_contato_id | int | ID do tipo de contato do contato 1 (1 - celular, 2 - fixo) | Obrigatório se `contato1_telefone_numero` preenchido |
| contato1_receber_propagandas | boolean | Indica se o contato 1 deseja receber propagandas | Obrigatório se `contato1_telefone_numero` preenchido |
| contato1_receber_confirmacoes | boolean | Indica se o contato 1 deseja receber confirmações | Obrigatório se `contato1_telefone_numero` preenchido |
| contato1_possui_whatsapp | boolean | Indica se o contato 1 possui WhatsApp | Obrigatório se `contato1_telefone_numero` preenchido |
| contato2_descricao | varchar | Descrição do contato 2 |  |
| contato2_telefone_ddd | int | DDD do telefone do contato 2 |  |
| contato2_num_ddi | int | DDI do telefone do contato 2 |  |
| contato2_telefone_numero | int | Número do telefone do contato 2 |  |
| contato2_telefone_completo | varchar | Número completo do telefone do contato 2 |  |
| contato2_preferido | boolean | Indica se o contato 2 é preferido | Obrigatório |
| contato2_tipo_contato_id | int | ID do tipo de contato do contato 2 (1 - celular, 2 - fixo) | Obrigatório se `contato2_telefone_numero` preenchido |
| contato2_receber_propagandas | boolean | Indica se o contato 2 deseja receber propagandas | Obrigatório se `contato2_telefone_numero` preenchido |
| contato2_receber_confirmacoes | boolean | Indica se o contato 2 deseja receber confirmações | Obrigatório se `contato2_telefone_numero` preenchido |
| contato2_possui_whatsapp | boolean | Indica se o contato 2 possui WhatsApp | Obrigatório se `contato2_telefone_numero` preenchido |
| contato3_descricao | varchar | Descrição do contato 3 |  |
| contato3_telefone_ddd | int | DDD do telefone do contato 3 |  |
| contato3_num_ddi | int | DDI do telefone do contato 3 |  |
| contato3_telefone_numero | int | Número do telefone do contato 3 |  |
| contato3_telefone_completo | varchar | Número completo do telefone do contato 3 |  |
| contato3_preferido | boolean | Indica se o contato 3 é preferido | Obrigatório |
| contato3_tipo_contato_id | int | ID do tipo de contato do contato 3 (1 - celular, 2 - fixo) | Obrigatório se `contato3_telefone_numero` preenchido |
| contato3_receber_propagandas | boolean | Indica se o contato 3 deseja receber propagandas | Obrigatório se `contato3_telefone_numero` preenchido |
| contato3_receber_confirmacoes | boolean | Indica se o contato 3 deseja receber confirmações | Obrigatório se `contato3_telefone_numero` preenchido |
| contato3_possui_whatsapp | boolean | Indica se o contato 3 possui WhatsApp | Obrigatório |
| contato4_descricao | varchar | Descrição do contato 4 |  |
| contato4_telefone_ddd | int | DDD do telefone do contato 4 |  |
| contato4_num_ddi | int | DDI do telefone do contato 4 |  |
| contato4_telefone_numero | int | Número do telefone do contato 4 |  |
| contato4_telefone_completo | varchar | Número completo do telefone do contato 4 |  |
| contato4_preferido | boolean | Indica se o contato 4 é preferido | Obrigatório |
| contato4_tipo_contato_id | int | ID do tipo de contato do contato 4 (1 - celular, 2 - fixo) | Obrigatório se `contato4_telefone_numero` preenchido |
| contato4_receber_propagandas | boolean | Indica se o contato 4 deseja receber propagandas | Obrigatório se `contato4_telefone_numero` preenchido |
| contato4_receber_confirmacoes | boolean | Indica se o contato 4 deseja receber confirmações | Obrigatório se `contato4_telefone_numero` preenchido |
| contato4_possui_whatsapp | boolean | Indica se o contato 4 possui WhatsApp | Obrigatório |
| email1_descricao | varchar | Descrição do email 1 |  |
| email1_receber_propagandas | boolean | Indica se o email 1 deseja receber propagandas | Obrigatório se `email1_endereco` preenchido |
| email1_receber_confirmacoes | boolean | Indica se o email 1 deseja receber confirmações | Obrigatório se `email1_endereco` preenchido |
| email2_descricao | varchar | Descrição do email 2 |  |
| email2_receber_propagandas | boolean | Indica se o email 2 deseja receber propagandas | Obrigatório se `email2_endereco` preenchido |
| email2_receber_confirmacoes | boolean | Indica se o email 2 deseja receber confirmações | Obrigatório se `email2_endereco` preenchido |
| operadora_saude1_unique_cod | varchar | Código único da operadora de saúde 1 | Obrigatório se `operadora_saude1_plano_unique_cod` preenchido |
| operadora_saude1_numero | varchar | Número da carteirinha da operadora de saúde 1 |  |
| operadora_saude1_validade | date | Data da validade da operadora de saúde 1 |  |
| operadora_saude1_nome_operadora | varchar | Nome da operadora de saúde 1 | Obrigatório se `operadora_saude1_plano_unique_cod` preenchido |
| operadora_saude1_detalhes | varchar | Detalhes da operadora de saúde 1 |  |
| operadora_saude1_plano_unique_cod | varchar | Código único do plano de saúde da operadora 1 |  |
| operadora_saude1_nome_plano | varchar | Nome do plano de saúde da operadora 1 |  |
| operadora_saude2_unique_cod | varchar | Código único da operadora de saúde 2 | Obrigatório se `operadora_saude2_plano_unique_cod` preenchido |
| operadora_saude2_numero | varchar | Número da carteirinha da operadora de saúde 2 |  |
| operadora_saude2_validade | date | Data da validade da operadora de saúde 2 |  |
| operadora_saude2_nome_operadora | varchar | Nome da operadora de saúde 2 | Obrigatório se `operadora_saude2_plano_unique_cod` preenchido |
| operadora_saude2_detalhes | varchar | Detalhes da operadora de saúde 2 |  |
| operadora_saude2_plano_unique_cod | varchar | Código único do plano de saúde da operadora 2 |  |
| operadora_saude2_nome_plano | varchar | Nome do plano de saúde da operadora 2 |  |
| operadora_saude3_unique_cod | varchar | Código único da operadora de saúde 3 | Obrigatório se `operadora_saude3_plano_unique_cod` preenchido |
| operadora_saude3_numero | varchar | Número da carteirinha da operadora de saúde 3 |  |
| operadora_saude3_validade | date | Data da validade da operadora de saúde 3 |  |
| operadora_saude3_nome_operadora | varchar | Nome da operadora de saúde 3 | Obrigatório se `operadora_saude3_plano_unique_cod` preenchido |
| operadora_saude3_detalhes | varchar | Detalhes da operadora de saúde 3 |  |
| operadora_saude3_plano_unique_cod | varchar | Código único do plano de saúde da operadora 3 |  |
| operadora_saude3_nome_plano | varchar | Nome do plano de saúde da operadora 3 |  |
| clinica_unique_cod | varchar | Código único da clínica | Obrigatório caso haja mais de uma clínica |