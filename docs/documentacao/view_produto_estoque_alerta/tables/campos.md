| Campo                            | Tipo      | Descrição                                                               | Restrição |
|----------------------------------|-----------|-------------------------------------------------------------------------|-----------|
| unique_cod                       | varchar   | Código único do alerta                                                  | Obrigatório |
| produto_apresentacao_unique_cod | varchar   | Código único da apresentação relacionada                                | Obrigatório |
| produto_estoque_unique_cod       | varchar   | Código único do estoque relacionado                                     | Obrigatório |
| quant_estoque_minimo             | decimal   | Limite mínimo de quantidade                                             |           |
| quant_estoque_maximo             | decimal   | Limite máximo de quantidade                                             |           |
| data_registro                    | timestamp | Data do registro; quando ausente, usa a data/hora da importação         | Obrigatório |

`produto_apresentacao_unique_cod` e `produto_estoque_unique_cod` devem corresponder, respectivamente, aos códigos informados nos arquivos de apresentações e estoques. Os limites são opcionais, mas pelo menos um entre `quant_estoque_minimo` e `quant_estoque_maximo` deve ser informado. Uma apresentação pode ter alertas em estoques diferentes, e cada alerta deve possuir seu próprio `unique_cod`.
