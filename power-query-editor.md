Meu guia para fazer a ETL

## 1. Remover linhas desnecessárias
Utilize a função **"Remover Linhas Superiores"** para excluir registros não estruturados, como títulos ou metadados inseridos nas primeiras linhas dos arquivos.

## 2. Promover primeira linha como cabeçalho
Use a opção **"Usar Primeira Linha como Cabeçalho"** para transformar a primeira linha de dados em nomes de colunas semânticos e apropriados.

## 3. Tratar textos com delimitadores
Acesse a aba **"Transformar" > "Extrair" > "Texto Após o Delimitador"** para limpar dados textuais, como remoção de símbolos ou prefixos (ex: "#").

## 4. Traduzir termos usando outra tabela
- Importe uma tabela de tradução (ex: CSV).
- Promova o cabeçalho se necessário.
- Utilize a função **"Mesclar Consultas"** para correlacionar os dados originais com os termos traduzidos.
- Expanda apenas a coluna de interesse, desmarcando o prefixo no nome da nova coluna.

## 5. Substituir valores manualmente
Use **"Substituir Valores"** para alterar registros específicos diretamente em colunas de texto. Ideal para casos com poucos valores distintos.

## 6. Criar coluna de exemplos
Na aba **"Adicionar Coluna"**, utilize a função **"Coluna de Exemplos"** para gerar transformações automáticas com base em entradas manuais. Esse recurso detecta padrões e aplica substituições com inteligência contextual.

## 7. Renomear e organizar colunas
Após a criação de novas colunas (ex: traduzidas), renomeie-as para facilitar a leitura e a interpretação. Remova colunas antigas se necessário.

## 8. Gerenciar etapas aplicadas
Acompanhe as **"Etapas Aplicadas"** no painel lateral. Use o botão de "X" para excluir ou ajustar etapas sem comprometer o histórico de transformações.

## 9. Criar colunas personalizadas (avançado)
Explore a função **"Coluna Personalizada"** para construir expressões utilizando a linguagem M, permitindo transformações mais complexas ou condicionais.
