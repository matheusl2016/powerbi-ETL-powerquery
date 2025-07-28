## 1. Avaliar quais consultas devem ser carregadas

- Nem todas as consultas precisam ser carregadas para o modelo final.
- Desabilite a carga de consultas auxiliares (como tabelas de tradução ou apoio):
  - Clique com o botão direito na consulta > **Desmarcar "Habilitar carga"**.

---

## 2. Carregar os dados

- Acesse "Página Inicial" > **Fechar e Aplicar**.
- O Power BI carregará apenas as tabelas com carga habilitada.

---

## 3. Acessar a exibição de modelo

- No painel lateral esquerdo, selecione **"Exibição de Modelo"**.
- Verifique visualmente os relacionamentos entre as tabelas do projeto.

---

## 4. Analisar e ajustar relacionamentos

- Clique nas linhas que conectam as tabelas para abrir as propriedades.
- **Verifique:**
  - Colunas utilizadas para o relacionamento
  - **Cardinalidade**: Um para muitos / Muitos para um
  - **Direção do filtro cruzado**: Apenas um sentido ou ambos

> **Boa prática**: Prefira filtros em um único sentido para evitar ambiguidade e melhorar a performance.

---

## 5. Corrigir ou criar relacionamentos manualmente

- Para ajustar um relacionamento:
  - Clique na linha > Propriedades > altere cardinalidade ou direção.
- Para criar do zero:
  - Arraste o campo de chave primária de uma tabela e solte sobre a chave estrangeira da outra.

---

## 6. Desabilitar detecção automática de relacionamentos

- Para ter controle total sobre os relacionamentos:
  - Vá em **Arquivo > Opções e Configurações > Opções**
  - Em "Arquivo Atual > Carregamento de Dados":
    - Desmarque:
      - "Importar relacionamentos de fontes de dados no primeiro carregamento"
      - "Detectar automaticamente novos relacionamentos..."

---

## 7. Testar o modelo com visuais simples

- Crie visuais como **tabelas** ou **gráficos de barras** usando campos relacionados de diferentes tabelas.
- Verifique se os dados agregam corretamente, de acordo com os filtros e relacionamentos definidos.

---

## 8. Ajustar direção do filtro quando necessário

- Se os resultados estiverem incorretos (valores repetidos ou totais errados), revise a **direção do filtro cruzado**.
- Ajuste para que a tabela de dimensão filtre corretamente a tabela de fatos.

---

## 9. Importância da modelagem para o DAX e relatórios

- Modelagem bem feita é pré-requisito para:
  - Fórmulas DAX funcionarem corretamente
  - Visualizações responderem a filtros
  - Segmentações e painéis interativos operarem como esperado
