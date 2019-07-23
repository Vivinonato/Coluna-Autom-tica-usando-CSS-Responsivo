Coluna "Automática", usando CSS Responsivo
Neste tutorial, vamos usar apenas HTML e CSS para ocultar colunas de forma responsiva, sem dependências de componentes de terceiros, como jQuery, DataTables.
Eu usei seletores de classe CSS para definir a prioridade da coluna como informacao-1, informacao-2, informacao-3, informacao-4, e informacao-5 . Os estilos de exibição são adicionados a esses seletores de classe com base no tamanho da tela de mídia usando consultas de mídia CSS. Quando a tela da janela estiver diminuindo, os estilos de exibição serão aplicados às colunas da tabela com base no limite de tamanho da janela especificado na consulta de mídia.
Classe informacao da coluna no HTML
Este código HTML é usado para exibir tabelas responsivas usando os seletores de classe. Especifiquei a classe informacao para as colunas da tabela HTML para controlar a exibição, por exemplo quando o tamanho da janela é menor, a exibição da coluna será ocultada usando os seletores de classe informacao.
<thead>
 <tr>
 <th class="informacao-1" width="15%">Nome</th>
 <th class="informacao-2" width="15%">Sobrenome</th>
 <th class="informacao-3" width="15%">Estado</th>
 <th class="informacao-4" width="10%">Nascimento</th>
 <th class="informacao-5" width="15%">Falescimento</th>
 </tr>
 </thead>
 
 <tbody>
 <tr>
 <td class="informacao-1">Maria</td>
 <td class="informacao-2">Bonita</td>
 <td class="informacao-3">Bahia</td>
 <td class="informacao-4">08/03/1911</td>
 <td class="informacao-5">28/07/1938</td>
 </tr>
CSS para ocultação automática de coluna
O seguinte código CSS é usado para implementar o ocultamento automático de colunas usando consultas de mídia. Este código contém consulta de mídia para quatro telas de várias janelas, especificando os limites máximos de min. Quando o tamanho da janela cai no limite, o estilo de exibição correspondente será aplicado às colunas da tabela.


@media screen and (max-width: 900px) and (min-width: 550px) {
 .informacao-5{
 display:none;
 }
 }
 
 @media screen and (max-width: 550px) {
 .informacao-5{
 display:none;
 }
 .informacao-4{
 display:none;
 }
 }
 
 @media screen and (max-width: 300px) {
 .informacao-5{
 display:none;
 }
 .informacao-4{
 display:none;
 }
 .informacao-3{
 display:none;
 }
 .informacao-2{
 display:none;
 }
