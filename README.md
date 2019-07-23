Coluna "Automática", usando CSS Responsivo
Neste tutorial, vamos usar apenas HTML e CSS para ocultar colunas de forma responsiva, sem dependências de componentes de terceiros, como jQuery, DataTables.

Usei seletores de classe CSS para definir a prioridade da coluna como informacao-1, informacao-2, informacao-3, informacao-4, e informacao-5 . Os estilos de exibição são adicionados a esses seletores de classe com base no tamanho da tela de mídia usando consultas de mídia CSS. Quando a tela da janela estiver diminuindo, os estilos de exibição serão aplicados às colunas da tabela com base no limite de tamanho da janela especificado na consulta de mídia.


Classe informacao da coluna no HTML
Este código HTML é usado para exibir tabelas responsivas usando os seletores de classe. Especifiquei a classe informacao para as colunas da tabela HTML para controlar a exibição, por exemplo quando o tamanho da janela é menor, a exibição da coluna será ocultada usando os seletores de classe informacao.

 
CSS para ocultação automática de coluna
O seguinte código CSS é usado para implementar o ocultamento automático de colunas usando consultas de mídia. Este código contém consulta de mídia para quatro telas de várias janelas, especificando os limites máximos de min. Quando o tamanho da janela cai no limite, o estilo de exibição correspondente será aplicado às colunas da tabela.

