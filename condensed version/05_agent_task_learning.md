# Tarefa: refine-output

## Finalidade

Refinar uma saída de texto gerada anteriormente com base no feedback específico do usuário. Esta tarefa dota o agente da capacidade de aprender, corrigir e se adaptar em tempo real, melhorando a qualidade final e o alinhamento com as expectativas do usuário.

---

## Entradas

- `original_output`: O bloco de texto que o agente gerou (Ex: um rascunho de post para LinkedIn).
- `user_feedback`: A instrução de correção do usuário (Ex: "O tom está muito formal, deixe mais casual", "Adicione esta estatística: 'crescimento de 50%'", "Seja mais direto no CTA").

---

## Processamento (Passo a Passo Agentic)

1.  **Análise do Feedback:**
    * Decomponha a instrução do `user_feedback` para entender a intenção principal:
        * **Ajuste de Tom:** Mudar o estilo (formal, casual, técnico, etc.).
        * **Adição/Remoção de Conteúdo:** Inserir ou remover informações específicas.
        * **Mudança de Foco/Ênfase:** Dar mais destaque a um ponto específico.
        * **Simplificação/Detalhamento:** Tornar o texto mais conciso ou mais explicativo.

2.  **Aplicação da Correção:**
    * Releia o `original_output`.
    * Reescreva o texto, tratando a instrução do usuário como a diretriz mais importante, sobrepondo-se às regras originais da tarefa se necessário.

3.  **Geração da Nova Versão:**
    * Apresente a nova versão do texto que incorpora o feedback.

4.  **Confirmação (Opcional):**
    * Pergunte se a nova versão atende melhor à expectativa. Ex: "Com base no seu feedback, ajustei o tom para ser mais direto. Esta versão está mais alinhada com o que você precisa?".

---

## Saída Esperada

-   O bloco de texto reescrito, refletindo as correções solicitadas pelo usuário.