| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição da pessoa | Obrigatório |
| codigo_nas_clinicas | varchar | Número que a clínica possa ter do cliente e que não seja a chave primária |  |
| data_registro | timestamp | Data de registro da pessoa | Obrigatório |
| data_exclusao | timestamp | Data de exclusão da pessoa |  |
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
| nacionalidade | varchar | Nacionalidade da pessoa. Exemplos: "AUSTRÁLIA" ou "BRASIL" |  |
| escolaridade | varchar | Escolaridade da pessoa, conforme tabela própria em `escolaridade` |  |
| raca | varchar | Raça da pessoa |  |
| estado_civil | varchar | Estado civil da pessoa |  |
| nome_conjuge | varchar | Nome do cônjuge |  |
| profissao_principal | varchar | Nome da profissão da pessoa (com base no CBO - IBGE) |  |
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
| end1_municipio_codigo_ibge | int | ID do município do endereço principal, conforme tabela de códigos dos municípios do IBGE, disponível [aqui](https://www.ibge.gov.br/explica/codigos-dos-municipios). |  |
| end1_municipio_nome | varchar | Nome do município do endereço principal. É extraído da base da Ebrain através do município fornecido. |  |
| end1_uf_sigla | varchar | Sigla da Unidade da Federação do endereço principal, conforme tabela de domínio |  |
| end1_cidade_nome_internacional | varchar | Nome da cidade do endereço caso seja um endereço internacional |  |
| end1_pais | varchar | Código identificador do país do endereço caso seja um endereço internacional |  |
| endereco_instagram | varchar | Endereço do Instagram da pessoa |  |
| endereco_facebook | varchar | Endereço do Facebook da pessoa |  |
| endereco_twitter | varchar | Endereço do Twitter da pessoa |  |
| clinica_unique_cod | varchar | Código único da clínica | Obrigatório caso haja mais de uma clínica |
| pessoa_indicacao_unique_cod | varchar | Código único da pessoa que indicou o paciente |  |
