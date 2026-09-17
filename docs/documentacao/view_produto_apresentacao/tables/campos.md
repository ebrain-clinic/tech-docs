| Campo                  | Tipo      | Descrição                                                                  | Restrição   |
|------------------------|-----------|----------------------------------------------------------------------------|-------------|
| unique_cod             | varchar   | Código único sem repetição da apresentação do produto                       | Obrigatório |
| nome                   | varchar   | Nome da apresentação                                                        | Obrigatório |
| unidade                | varchar   | Unidade da apresentação como um todo. Ex.: Frasco, Ampola, Caixa, Unidade   | Obrigatório |
| generico               | boolean   | Indica se a apresentação é de produto genérico                              | Obrigatório |
| produto_unique_cod     | varchar   | Código único do produto relacionado (ver [produtos](documentacao/view_produto/)) | Obrigatório |
| quantidade             | decimal   | Quantidade da fração contida na apresentação                                | Obrigatório |
| data_exclusao          | timestamp | Data de exclusão lógica da apresentação                                     |             |
| fracao_unidade         | varchar   | Unidade da fração (unidade de saída) da apresentação. Ex.: Unidade, mL, Comprimido |             |
| uso_fracionado         | boolean   | Indica se a apresentação permite uso fracionado                             | Obrigatório |
| clinica_unique_cod     | varchar   | Código único da clínica do cadastro, quando houver mais de uma clínica      |             |
| laboratorio_unique_cod | varchar   | Código único do laboratório relacionado (ver [laboratórios](documentacao/view_laboratorio/)) |             |
| laboratorio_nome       | varchar   | Nome do laboratório, usado para localizar um laboratório existente pelo nome |             |
| nome_estoque           | varchar   | Nome do estoque (até 200 caracteres); alimenta produto_estoque.nome. A identidade externa do estoque é upper(nome_estoque), única na carga e associada a uma única clínica. | Obrigatório quando houver limites de estoque |
| quant_estoque_minimo    | decimal   | Quantidade mínima; alimenta produto_estoque_alerta.quant_estoque_minimo      |             |
| quant_estoque_maximo    | decimal   | Quantidade máxima; alimenta produto_estoque_alerta.quant_estoque_maximo      |             |
| data_registro          | timestamp | Data do registro do alerta; alimenta produto_estoque_alerta.data_registro. Quando ausente, usa a data/hora da importação. |             |

Cada unique_cod identifica uma apresentação e seu alerta de estoque. O vínculo produto_apresentacao_id é resolvido pelo unique_cod em import_externo; produto_estoque_id é resolvido por upper(nome_estoque). A clínica é resolvida por clinica_unique_cod; quando não informado, utiliza a clínica padrão da importação. Sem nome_estoque, nenhum estoque ou alerta é criado. Reimportações reutilizam os IDs de import_externo e inserem somente registros novos, sem alterar alertas já existentes.
