# Conexão com Arquivos XML e JSON no Power BI

resumo do processo de importação das bases de dados da Olist nos formatos XML e JSON utilizando o Power BI Desktop.

## Importação de arquivo XML (olist_pagamentos.xml)

1. Na aba "Página Inicial", clique em "Obter dados" > "XML".
2. Selecione o arquivo `olist_pagamentos.xml`.
3. No painel lateral esquerdo, clique em "row".
4. Marque a caixa de seleção da tabela e clique em "Carregar".

Resultado: A base de dados é carregada diretamente para o modelo no Power BI.

## Importação de arquivo JSON (olist_produtos.json)

1. Clique novamente em "Obter dados" > "JSON".
2. Selecione o arquivo `olist_produtos.json`.
3. O Power BI abrirá automaticamente o Editor do Power Query.

Características:
- Primeira coluna com nomes dos campos (ex: `product_id`, `product_category_name`, etc.).
- Segunda coluna com registros no formato "Record".
