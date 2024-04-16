# Profissionais

<p align="justify"> 
Descreve a estrutura de dados de profissionais. A tabela de descrição dos campos abrange as principais informações.
 </p>

> Nome do arquivo de importação: `import_profissional.csv`


 ## Descrição dos campos

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
| profissional_papel    |varchar | papéis do profissional no sistema separados por ; (especificados em [papéis do profissional](#papéis-do-profissional) )    | |


# Especialidades
<p align="justify"> 
Descreve as especialidades disponíveis no sistema.
 </p>

 ## Descrição dos campos
 | especialidades_id |nome_especialidade  |
|--------------------------|-----------------|
1	|Acupuntura
2	|Alergia e imunologia
3	|Anestesiologia
4	|Angiologia
5	|Cardiologia
6	|Cirurgia cardiovascular
7	|Cirurgia da mão
8	|Cirurgia de cabeça e pescoço
9	|Cirurgia do aparelho digestivo
10	|Cirurgia geral
11	|Cirurgia oncológica
12	|Cirurgia pediátrica
13	|Cirurgia plástica
14	|Cirurgia torácica
15	|Cirurgia vascular
16	|Clínica médica
17	|Coloproctologia
18	|Dermatologia
19	|Endocrinologia e metabologia
20	|Endoscopia
21	|Gastroenterologia
22	|Genética médica
23	|Geriatria
24	|Ginecologia e obstetrícia
25	|Hematologia e hemoterapia
26	|Homeopatia
27	|Infectologia
28	|Mastologia
29	|Medicina de emergência
30	|Medicina de família e comunidade
31	|Medicina do trabalho
32	|Medicina de tráfego
33	|Medicina esportiva
34	|Medicina física e reabilitação
35	|Medicina intensiva
36	|Medicina legal e perícia médica
37	|Medicina nuclear
38	|Medicina preventiva e social
39	|Nefrologia
40	|Neurocirurgia
41	|Neurologia
42	|Nutrologia
43	|Oftalmologia
44	|Oncologia clínica
45	|Ortopedia e traumatologia
46	|Otorrinolaringologia
47	|Patologia
48	|Patologia clínica/medicina laboratorial
49	|Pediatria
50	|Pneumologia
51	|Psiquiatria
52	|Radiologia e diagnóstico por imagem
53	|Radioterapia
54	|Reumatologia
55	|Urologia
56	|Acupuntura
57	|Cirurgia e traumatologia buco-maxilo-facial
58	|Dentística
59	|Disfunção temporomandibular e dor orofacial
60	|Endodontia
61	|Estomatologia
62	|Harmonização orofacial
63	|Homeopatia
64	|Implantodontia
65	|Odontogeriatria
66	|Odontologia do esporte
67	|Odontologia do trabalho
68	|Odontologia legal
69	|Odontologia para pacientes com necessidades especiais
70	|Odontopediatria
71	|Ortodontia
72	|Ortopedia funcional dos maxilares
73	|Patologia oral e maxilo facial
74	|Periodontia
75	|Prótese buco-maxilo-facial
76	|Prótese dentária
77	|Radiologia odontológica e imaginologia
78	|Saúde coletiva

# Papéis do Profissional
<p align="justify"> 
Descreve os papéis dos profissionais disponíveis no sistema.
 </p>


## Descrição dos campos

 | label | descrição  |
|--------------------------|-----------------|
ROLE_ADM	|Administrador
ROLE_ESTOQUE	|Estoque
ROLE_ORCAMENTO	|Orçamento
ROLE_GESTOR_APP	|Gestor do App
ROLE_ASSISTENTE	|Assistente de Médico
ROLE_RECEPCAO	|Recepcionista
ROLE_IMPLANTADOR	|Implantador
ROLE_FINANCEIRO	|Financeiro
ROLE_PROFISSIONAL	|Médico
ROLE_MARKETING	|Marketing



## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_profissional.csv ':ignore')
