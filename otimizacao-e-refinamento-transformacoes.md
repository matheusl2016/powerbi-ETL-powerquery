
## 1. Renomear consultas e colunas

- **Consultas**: Dê nomes claros e semânticos às consultas. Clique com o botão direito na consulta > "Renomear".
- **Colunas**: Padronize os nomes das colunas (por exemplo, `order_id` para `ID_Pedido`) garantindo consistência entre diferentes tabelas.

## 2. Selecionar apenas as colunas necessárias

- Remova colunas irrelevantes para o objetivo analítico.
- Use "Remover Outras Colunas" após selecionar as desejadas com Ctrl.
- A exclusão cria uma etapa rastreável ("Colunas Removidas") que pode ser desfeita ou modificada.

## 3. Refatorar etapas aplicadas

- Elimine etapas redundantes (ex: "Tipo Alterado", "Tipo Alterado1").
- Unifique etapas semelhantes no **Editor Avançado** para deixar o código mais limpo e performático.
- Corrija referências entre etapas para evitar erros cíclicos.

## 4. Utilizar o Editor Avançado para controle total

- Acesse o Editor Avançado pela aba "Página Inicial".
- As transformações são declaradas no bloco `let` e finalizadas no `in`.
- É possível copiar, colar e reaproveitar o código em outras consultas ou projetos.

## 5. Duplicar ou referenciar consultas

- **Duplicar**: copia toda a estrutura e etapas aplicadas.
- **Referenciar**: cria uma nova consulta baseada na anterior, sem duplicar carga de dados. Ideal para desmembrar análises mantendo performance.

## 6. Renomear e documentar etapas aplicadas

- Renomeie etapas com nomes mais descritivos clicando com o botão direito > "Renomear".
- Adicione **descrições** nas etapas aplicadas para facilitar o entendimento futuro:
  - Clique com o botão direito sobre uma etapa > "Propriedades..." > adicione a descrição.

## 7. Boas práticas de encerramento do tratamento

- Verifique se etapas redundantes foram removidas.
- Certifique-se de que os nomes das colunas e consultas são consistentes.
- Mantenha apenas os dados essenciais para o objetivo analítico.
- Adicione comentários e estrutura lógica no Editor Avançado para facilitar manutenção futura.
