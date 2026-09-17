| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do template de documento | Obrigatório |
| nome | varchar | Nome usado para identificar o template | Obrigatório |
| tipo | varchar | Categoria do documento gerado pelo template (ver [valores possíveis](documentacao/view_documento_template/#tipo)) | Obrigatório |
| data_exclusao | timestamp | Data e hora de exclusão lógica do template | |
| data_registro | timestamp | Data e hora de registro do template | Obrigatório |
| conteudo_titulo | varchar | Título padrão apresentado no documento | |
| conteudo_body | text | Conteúdo do template, podendo conter texto formatado em HTML e variáveis de substituição | Obrigatório |
| profissional_unique_cod | varchar | Código único do profissional proprietário do template (ver [Usuários](documentacao/view_user/)) | |
