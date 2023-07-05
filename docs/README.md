# <span style="color: #00C985;">ebrain - Documentação Técnica</span>


## <span style="color: #00C985;">Sobre</span>

Este documento apresenta os modelos de importação de dados para o sistema **ebrain**. Os dados importados referem-se a:

- pacientes
- profissionais
- agendamentos
- atendimentos
- evoluções de prontuários
- prescrições de medicamentos
- prescrições de exames
- atestados, relatórios e outros documentos
- serviços ofertados pela clínica
- operadoras de saúde

## <span style="color: #00C985;">Modelos</span>

- [Pacientes](documentacao/view_pessoa.md)
- [Agendamento](documentacao/view_agendamento.md)
- [Evolução](documentacao/view_evolucao.md)
- [Operadora de Saúde](documentacao/view_operadora_saude.md)
- [Serviços](documentacao/view_servicos.md)
- [Prescrição de Medicamentos](documentacao/view_prescricao_medicamento.md)
- [Prescrição de Exames](documentacao/view_exames.md)

## <span style="color: #00C985;">Observações Gerais de Tipo</span>

Todos os arquivos devem ser codificados no padrão **Unicode UTF-8**.

Os tipos são definidos conforme a tabela abaixo:

| Tipo                       | Domínio | Exemplo                                                           |
|----------------------------|-------- | ------------------------------------------------------------------|
| varchar                    | Conjunto de caracteres na codificação UTF-8        | "texto"                |
| int                        | Números inteiros        | 1                                                 |
| boolean                       | `true` ou `false` | true                                                 |
| date                       | YYYY-MM-DD | 2019-01-01                                                     |
| timestamp                  | Formato da ISO 8601 | 2019-01-01 00:00:00                                   |
| numeric(21,2)              | Números decimais | 10.00                                                    |
| json                       | JSON | {"campo1": "valor1", "campo2": "valor2"}                             |
