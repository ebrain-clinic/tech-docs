# <span style="color: #00C985;">ebrain - Documentação Técnica</span>


## <span style="color: #00C985;">Sobre</span>

Este documento apresenta os modelos de importação de dados para o sistema **ebrain**. São passíveis de serem importados dados de pacientes, profissionais, agendamentos, atendimentos, evoluções de prontuários, prescrições de medicamentos, prescrições de exames, atestados, relatórios e outros documentos, serviços ofertados pela clínica, operadoras de saúde, entre outros. Veja nas seções seguintes detalhes de cada modelo de arquivo de importação. Exemplos de arquivos de importação também estão disponíveis.

Mais informações disponíveis no site [www.ebrain.clinic](https://www.ebrain.clinic).

## <span style="color: #00C985;">Modelos</span>

Modelos de arquivos de importação disponíveis:

- [Pacientes](documentacao/view_pessoa.md)
- [Agendamento](documentacao/view_agendamento.md)
- [Evolução](documentacao/view_evolucao.md)
- [Operadora de Saúde](documentacao/view_operadora_saude.md)
- [Serviços](documentacao/view_servicos.md)
- [Prescrição de Medicamentos](documentacao/view_prescricao_medicamento.md)
- [Prescrição de Exames](documentacao/view_exames.md)

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
| timestamp                  | Formato da [ISO 8601](https://pt.wikipedia.org/wiki/ISO_8601) | 2019-01-01 00:00:00                                   |
| numeric(21,2)              | Números decimais | 10.00                                                    |
| json                       | JSON | "{"campo1": "valor1", "campo2": "valor2"}"                             |
