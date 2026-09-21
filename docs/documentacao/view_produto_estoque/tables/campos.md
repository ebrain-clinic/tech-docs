| Campo              | Tipo    | Descrição                                                            | Restrição |
|--------------------|---------|----------------------------------------------------------------------|-----------|
| unique_cod         | varchar | Código único do estoque                                              | Obrigatório |
| nome_estoque       | varchar | Nome do estoque, com até 200 caracteres                              | Obrigatório e único por clínica |
| clinica_unique_cod | varchar | Código único da clínica à qual o estoque pertence                    |           |

O `nome_estoque` pode se repetir quando os estoques pertencem a clínicas diferentes. Na mesma clínica, não são permitidos nomes iguais, desconsiderando espaços no início ou no fim e diferenças entre letras maiúsculas e minúsculas. Quando `clinica_unique_cod` não é informado, o estoque pertence à clínica padrão e o nome também deve ser único nela.
