Registrar Saída para Demonstrador

<details><summary>UC4 - Registrar Saída para Demonstrador</summary> <table> <thead> <tr align="center"> <th colspan="2">UC4 - Registrar Saída para Demonstrador</th> </tr> </thead> <tbody> <tr> <td width=2500px><strong>Ator Principal</strong></td> <td width=7500px>Estoquista</td> </tr> <tr> <td><strong>Pré-condições</strong></td> <td> - Estoquista deve estar autenticado no sistema.<br> - Produtos disponíveis no estoque para saída.<br> - Estoque atualizado e consistente. </td> </tr> <tr> <td><strong>Pós-condições</strong></td> <td> - Produto marcado como "em demonstração" e saída registrada.<br> - Estoque atualizado refletindo a saída.<br> - Registro da movimentação salvo para auditoria. </td> </tr> <tr> <td><strong>Fluxo Principal</strong></td> <td> 1. Estoquista acessa a funcionalidade "Registrar Saída para Demonstrador".<br> 2. Sistema exibe lista de produtos disponíveis para saída.<br> 3. Estoquista seleciona o produto e a quantidade para saída.<br> 4. Estoquista confirma a saída para demonstrador.<br> 5. Sistema valida a quantidade disponível.<br> 6. Sistema atualiza o estoque, marcando o produto como "em demonstração".<br> 7. Sistema registra a saída no histórico de movimentações.<br> 8. Sistema exibe mensagem de confirmação da operação.<br>

O caso de uso termina com o produto registrado para demonstração e estoque atualizado.
</td> </tr> <tr> <td><strong>Fluxos Alternativos</strong></td> <td> 3.A Produto já reservado para outro demonstrador:<br> 3.A.1 Sistema exibe mensagem informando que o produto está reservado.<br> 3.A.2 Estoquista pode selecionar outro produto ou cancelar a operação.<br> 3.A.3 Se selecionar outro produto, retorna ao passo 3.<br> </td> </tr> <tr> <td><strong>Fluxos de Exceção</strong></td> <td> 5.A Quantidade insuficiente no estoque:<br> 5.A.1 Sistema exibe mensagem de erro.<br> 5.A.2 Estoquista pode ajustar a quantidade ou cancelar a operação.<br>

6.A Erro ao atualizar o estoque:<br>
6.A.1 Sistema informa o erro.<br>
6.A.2 Operação é cancelada e estoque permanece inalterado.<br>
6.A.3 Estoquista é orientado a tentar novamente.<br>
</td> </tr> </tbody> </table> </details>