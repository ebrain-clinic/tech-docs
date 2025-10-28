# Agendamento

<p align="justify"> 
Descreve a estrutura de dados de agendamento. A tabela de descrição dos campos abrange as informações do evento agendado, bem como os serviços relacionados ao agendamento, independentemente do número de serviços envolvidos. Além disso, também é registrado se o agendamento foi efetivamente realizado.
 </p>

> Nome do arquivo de importação: `import_agendamento.csv`

## Descrição dos campos

[](tables/campos.md ':include')

## Lista de Siglas e Padrões de Nomenclatura dos Campos

### registro_automatico_trigger

[](tables/registro_automatico_trigger.md ':include')

### dominio_motivo_cancelamento

[](tables/dominio_motivo_cancelamento.md ':include')


### Observação
<p align="justify"> 
É importante destacar que eventos do tipo "bloqueio" nem sempre são importados, uma vez que o sistema Ebrain já oferece funcionalidades específicas para indicar ausências. Para registros futuros, nossa equipe realizará a análise e os extrairá em uma planilha específica, permitindo que a clínica insira manualmente as ausências no sistema, garantindo maior precisão e controle.
</p> 

## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](documentacao/view_agendamento/import_agendamento.csv ':ignore')
