| Campo                   |tipo  | Descrição                | Restrição |
|--------------------------|-|------------------------------|----|
| unique_cod            |varchar | Código único                 |Obrigatório |
| pessoa_nome           |varchar | Nome do profissional         |Obrigatório |
| profissional_nome     |varchar | Nome usado profissionalmente |Obrigatório |
| crm      |varchar | CRM do profissional          |Obrigatório |
| uf       |varchar | Sigla do estado do CRM       |Obrigatório | 
| sexo                  |varchar | Sexo do Profissional         |Obrigatório |
| cpf                   |varchar | Número do CPF                |Obrigatório |
| email                 |varchar | Email do Profissional        |Obrigatório |
| especialidades_id     |varchar | códigos das especialidades separados por ; (especificadas em [especialidades](#especialidades) )      |Obrigatório |
| agenda_coletiva       |Boolean | Se precisa de uma agenda exclusiva (false) ou não (true) |Obrigatório |
| roles_atribuidas    |varchar | papéis do usuário no sistema separados por ; (especificados em [papéis do Usuário](#papéis-do-usuário) )    | |
