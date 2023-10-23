# <span style="color: #00C985;">ebrain - Documentação Técnica</span>


## <span style="color: #00C985;">Sobre</span>

Este documento apresenta os modelos de dados do sistema **ebrain**. São passíveis de serem exportados e importados dados de pacientes, profissionais, agendamentos, atendimentos, evoluções de prontuários, prescrições de medicamentos, prescrições de exames, atestados, relatórios e outros documentos, serviços ofertados pela clínica, operadoras de saúde, entre outros. Exemplos de arquivos também estão disponíveis.

Mais informações disponíveis no site [www.ebrain.clinic](https://www.ebrain.clinic).

## <span style="color: #00C985;">Formato e codificação de arquivos</span>

Todos os arquivos devem ser salvos em [formato CSV](https://pt.wikipedia.org/wiki/Comma-separated_values), ou seja, arquivo texto simples separados por vírgulas, e codificados no padrão [Unicode UTF-8](https://pt.wikipedia.org/wiki/UTF-8).

Os arquivos CSV podem ser gerados pela equipe de tecnologia responsável pelo software atual, ou manualmente a partir de uma planilha Excel criada pelo cliente. Em todos os casos, use os arquivos de exemplo disponíveis em cada página de Modelo.

## <span style="color: #00C985;">Tipos de dados</span>

Os tipos descritos nos modelos são definidos conforme o seguinte padrão:

| Tipo                       | Domínio | Exemplo                                                           |
|----------------------------|-------- | ------------------------------------------------------------------|
| varchar                    | Conjunto de caracteres na codificação UTF-8        | "texto"                |
| int                        | Números inteiros, sem indicação de decimais   | 1                           |
| boolean                    | `true` ou `false` | true                                                 |
| date                       | Formato YYYY-MM-DD | 2019-01-01                                                     |
| timestamp                  | Formato da [ISO 8601](https://pt.wikipedia.org/wiki/ISO_8601) | 2019-01-01 18:30:55                                   |
| numeric(21,2)              | Números decimais | 10.00                                                    |
| json                       | JSON | "{"campo1": "valor1", "campo2": "valor2"}"                             |

### <span style="color: #00C985;">Campos `unique_cod`</span>

Os campos `unique_cod` representam chaves primárias, e devem representar uma única linha (tupla ou registro) no arquivo de modelo.

Campos como `pessoa_unique_cod`, `profissional_unique_cod`, entre outros com o mesmo sufixo, representam ligações (chaves estrangeiras), e devem ser preenchidos com o valor do campo `unique_cod` do arquivo de modelo correspondente.