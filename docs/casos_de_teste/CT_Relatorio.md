Casos de Teste - Gerar Relatório 

<details>
  <summary>CT18 - Visualização de relatório com sucesso</summary>
  <table>
    <thead>
      <tr align="center">
        <th colspan="2">CT18 - Visualização de relatório com sucesso</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Objetivo</strong></td>
        <td>Verificar se o administrador consegue visualizar corretamente os dados do relatório de Transferências ou Retiradas com movimentações registradas.</td>
      </tr>
      <tr>
        <td><strong>Pré-condições</strong></td>
        <td>
          - Usuário autenticado com perfil de Administrador.<br>
          - Existem movimentações registradas no sistema (transferências ou retiradas).
        </td>
      </tr>
      <tr>
        <td><strong>Entradas</strong></td>
        <td>Seleção da aba desejada: "Transferências" ou "Retiradas".</td>
      </tr>
      <tr>
        <td><strong>Passos</strong></td>
        <td>
          1. Acessar o menu “Relatórios” na página inicial.<br>
          2. Selecionar a aba “Transferências” ou “Retiradas”.<br>
          3. Aguardar a exibição dos dados em tela.
        </td>
      </tr>
      <tr>
        <td><strong>Resultado Esperado</strong></td>
        <td>
          - O sistema exibe os dados registrados com as seguintes colunas: Produto, Quantidade, Origem, Destino, Usuário, Data e Observações.<br>
          - O botão “Exportar para CSV” deve estar habilitado, mas **não é clicado neste teste**.<br>
          - A visualização dos dados deve ser clara e completa para o administrador.
        </td>
      </tr>
      <tr>
        <td><strong>Resultado Obtido</strong></td>
        <td>[Preencher após a execução do teste]</td>
      </tr>
      <tr>
        <td><strong>Status</strong></td>
        <td>[Passou / Falhou / Bloqueado]</td>
      </tr>
      <tr>
        <td><strong>Observações</strong></td>
        <td>[Inserir observações, se necessário]</td>
      </tr>
    </tbody>
  </table>
</details>

<details><summary>CT19 - Visualizar relatório de retiradas sem registros</summary>
<table>
<thead>
<tr align="center">
<th colspan="2">CT19 - Visualizar relatório de retiradas sem registros</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Objetivo</strong></td>
<td>Verificar se o sistema informa corretamente a ausência de registros na aba “Retiradas” do relatório.</td>
</tr>
<tr>
<td><strong>Pré-condições</strong></td>
<td>Administrador autenticado. Nenhuma retirada registrada no sistema.</td>
</tr>
<tr>
<td><strong>Entradas</strong></td>
<td>Seleção da aba “Retiradas”.</td>
</tr>
<tr>
<td><strong>Passos</strong></td>
<td>
1. Acessar o menu “Relatórios”.<br>
2. Selecionar aba “Retiradas”.
</td>
</tr>
<tr>
<td><strong>Resultado Esperado</strong></td>
<td>
- Sistema exibe a mensagem “Nenhuma retirada encontrada”.<br>
- Botão “Exportar para CSV” não é exibido ou aparece desabilitado.
</td>
</tr>
<tr>
<td><strong>Resultado Obtido</strong></td>
<td>[Preencher durante a execução]</td>
</tr>
<tr>
<td><strong>Status</strong></td>
<td>[Passou / Falhou / Bloqueado]</td>
</tr>
<tr>
<td><strong>Observações</strong></td>
<td>[Comentários adicionais, se necessário]</td>
</tr>
</tbody>
</table>
</details>

<details><summary>CT20 - Tentativa de exportação com relatório vazio</summary>
<table>
<thead>
<tr align="center">
<th colspan="2">CT20 - Tentativa de exportação com relatório vazio</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Objetivo</strong></td>
<td>Garantir que o botão de exportação permaneça desabilitado quando não houver dados disponíveis para exibição.</td>
</tr>
<tr>
<td><strong>Pré-condições</strong></td>
<td>Administrador autenticado. Nenhum dado disponível para o tipo de relatório selecionado.</td>
</tr>
<tr>
<td><strong>Entradas</strong></td>
<td>Seleção da aba “Retiradas” (sem registros).</td>
</tr>
<tr>
<td><strong>Passos</strong></td>
<td>
1. Acessar o menu “Relatórios”.<br>
2. Selecionar aba “Retiradas”.<br>
3. Verificar o estado do botão “Exportar para CSV”.
</td>
</tr>
<tr>
<td><strong>Resultado Esperado</strong></td>
<td>
- Botão “Exportar para CSV” está desabilitado.<br>
- Nenhuma ação de download ocorre.<br>
- Mensagem de ausência de dados é exibida.
</td>
</tr>
<tr>
<td><strong>Resultado Obtido</strong></td>
<td>[Preencher durante a execução]</td>
</tr>
<tr>
<td><strong>Status</strong></td>
<td>[Passou / Falhou / Bloqueado]</td>
</tr>
<tr>
<td><strong>Observações</strong></td>
<td>[Comentários adicionais, se necessário]</td>
</tr>
</tbody>
</table>
</details>

<details><summary>CT21 - Falha na exportação do relatório</summary>
<table>
<thead>
<tr align="center">
<th colspan="2">CT21 - Falha na exportação do relatório</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Objetivo</strong></td>
<td>Verificar o comportamento do sistema quando ocorre uma falha técnica durante a tentativa de exportação de um relatório com dados.</td>
</tr>
<tr>
<td><strong>Pré-condições</strong></td>
<td>Administrador autenticado. Dados disponíveis para exportação. Conexão instável ou erro interno no sistema.</td>
</tr>
<tr>
<td><strong>Entradas</strong></td>
<td>Seleção da aba “Transferências” com dados. Clique no botão “Exportar para CSV”.</td>
</tr>
<tr>
<td><strong>Passos</strong></td>
<td>
1. Acessar o menu “Relatórios”.<br>
2. Selecionar aba “Transferências”.<br>
3. Clicar no botão “Exportar para CSV”.<br>
4. Durante a exportação, ocorre erro simulado.
</td>
</tr>
<tr>
<td><strong>Resultado Esperado</strong></td>
<td>
- Sistema exibe mensagem de erro.<br>
- Exportação é cancelada.<br>
- Administrador é orientado a tentar novamente.
</td>
</tr>
<tr>
<td><strong>Resultado Obtido</strong></td>
<td>[Preencher durante a execução]</td>
</tr>
<tr>
<td><strong>Status</strong></td>
<td>[Passou / Falhou / Bloqueado]</td>
</tr>
<tr>
<td><strong>Observações</strong></td>
<td>[Comentários adicionais, se necessário]</td>
</tr>
</tbody>
</table>
</details>

<details><summary>CT22 - Exportação de relatório com sucesso</summary>
<table>
<thead>
<tr align="center">
<th colspan="2">CT22 - Exportação de relatório com sucesso</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Objetivo</strong></td>
<td>Validar se o administrador consegue exportar corretamente os dados do relatório em formato CSV.</td>
</tr>
<tr>
<td><strong>Pré-condições</strong></td>
<td>Administrador autenticado. Há movimentações registradas no sistema na aba selecionada (“Transferências” ou “Retiradas”).</td>
</tr>
<tr>
<td><strong>Entradas</strong></td>
<td>Seleção da aba com dados disponíveis. Clique no botão “Exportar para CSV”.</td>
</tr>
<tr>
<td><strong>Passos</strong></td>
<td>
1. Acessar o menu “Relatórios”.<br>
2. Selecionar a aba “Transferências” ou “Retiradas”.<br>
3. Verificar se os dados foram carregados corretamente.<br>
4. Clicar no botão “Exportar para CSV”.<br>
5. Confirmar o início e o término do download.
</td>
</tr>
<tr>
<td><strong>Resultado Esperado</strong></td>
<td>
- O botão “Exportar para CSV” está habilitado.<br>
- O arquivo é baixado automaticamente no formato `.csv`.<br>
- O conteúdo do arquivo corresponde aos dados exibidos na tela, com colunas como: Produto, Quantidade, Origem, Destino, Usuário, Data, Observações.
</td>
</tr>
<tr>
<td><strong>Resultado Obtido</strong></td>
<td>[Preencher durante a execução]</td>
</tr>
<tr>
<td><strong>Status</strong></td>
<td>[Passou / Falhou / Bloqueado]</td>
</tr>
<tr>
<td><strong>Observações</strong></td>
<td>[Ex: nome do arquivo gerado, estrutura do CSV, problemas de formatação, etc.]</td>
</tr>
</tbody>
</table>
</details>


