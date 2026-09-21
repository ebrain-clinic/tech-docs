| Campo                            | Tipo      | Descrição                                                               | Restrição |
|----------------------------------|-----------|-------------------------------------------------------------------------|-----------|
| unique_cod                       | varchar   | Código estável do alerta                                                | Obrigatório |
| produto_apresentacao_unique_cod | varchar   | Código da apresentação relacionada                                      | Obrigatório |
| produto_estoque_unique_cod       | varchar   | Código externo estável do estoque relacionado                           | Obrigatório |
| quant_estoque_minimo             | decimal   | Limite mínimo de quantidade                                             |           |
| quant_estoque_maximo             | decimal   | Limite máximo de quantidade                                             |           |
| data_registro                    | timestamp | Data do registro; quando ausente, usa a data/hora da importação         | Obrigatório |

Os vínculos são resolvidos por produto_apresentacao_unique_cod e produto_estoque_unique_cod via import_externo. Os limites são opcionais, mas pelo menos um deve ser informado. A tabela de destino não possui unicidade no par apresentação/estoque, portanto esta superview preserva alertas distintos para a mesma apresentação em estoques diferentes.
