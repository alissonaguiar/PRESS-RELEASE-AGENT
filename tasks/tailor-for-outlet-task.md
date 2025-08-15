# Tarefa: tailor-for-outlet

## Finalidade

Adaptar um Press Release geral para um tipo de veículo de mídia específico, ajustando o ângulo, tom, linguagem e ênfase para maximizar a relevância e o apelo para os jornalistas e o público daquele veículo.

---

## Entradas

- `press_release_text`: O texto do Press Release original e genérico.
- `outlet_type`: O tipo de veículo de mídia para o qual a adaptação será feita (Ex: "Blog de Tecnologia", "Jornal de Negócios", "Revista de Varejo", "Portal de Notícias Local").
- `announcement_profile`: O perfil original do anúncio para manter o contexto da mensagem central.

---

## Dados Internos a Consultar

- `.bmad-core/data/media-outlet-types.md`: Essencial para esta tarefa. Este arquivo contém as características, interesses e o público de cada tipo de veículo.
- `.bmad-core/data/pr-style-guide.md`: Para garantir que a essência da marca seja mantida, mesmo com as adaptações.

---

## Processamento (Passo a Passo Agentic)

1.  **Análise do Veículo de Mídia (Outlet):**
    * Receba o `outlet_type` e consulte o arquivo `.bmad-core/data/media-outlet-types.md` para extrair o perfil completo:
        * **Público-alvo:** Quem são os leitores? (Ex: Desenvolvedores, C-levels, consumidores).
        * **Interesses Principais:** Que tipo de histórias eles cobrem? (Ex: Inovação técnica, impacto financeiro, tendências de consumo).
        * **Tom de Voz Preferido:** (Ex: Técnico e direto, formal e analítico, leve e aspiracional).

2.  **Definição do Novo Ângulo Noticioso:**
    * **Reflexão:** Com base no perfil do veículo, qual é o aspecto mais interessante do meu anúncio para *este* público?
    * **Exemplo de Raciocínio:**
        * **Anúncio:** "Empresa X lança software de IA que reduz custos logísticos".
        * **Para um `Blog de Tecnologia`:** O ângulo é a *inovação*. "Como funciona o algoritmo de IA preditiva?".
        * **Para um `Jornal de Negócios`:** O ângulo é o *impacto financeiro*. "Qual o ROI e a vantagem competitiva que essa redução de custos gera?".
        * **Para um `Portal de Notícias Local`:** O ângulo é o *impacto local*. "A Empresa X, sediada em Porto Alegre, está contratando engenheiros para esta nova tecnologia?".

3.  **Reescrita Estratégica do Conteúdo:**
    * O agente não deve apenas substituir palavras, mas reestruturar a informação.
    * **Headline e Subheadline:** Crie novos títulos que reflitam o ângulo definido.
    * **Parágrafo de Abertura (Lede):** Reescreva o primeiro parágrafo para destacar imediatamente a informação mais relevante para aquele público.
    * **Corpo do Texto:** Reordene os parágrafos. Traga os detalhes técnicos para o início para o blog de tecnologia; comece com os números de negócio para o jornal financeiro. Remova ou resuma informações menos relevantes para aquele público.
    * **Citação:** Se possível, ajuste levemente a citação para alinhar-se ao novo ângulo. (Ex: Para o blog de tecnologia, a citação do CEO pode ser trocada por uma do CTO).

4.  **Ajuste de Tom e Linguagem:**
    * Adapte o vocabulário. Use termos mais técnicos para o público especializado. Use uma linguagem mais focada em benefícios para o público consumidor.
    * Garanta que o tom geral (formal, casual, analítico) corresponda ao que o veículo de mídia espera.

---

## Saída Esperada

-   Um documento Markdown contendo a versão completamente reescrita e adaptada do Press Release.
-   Opcionalmente, o agente pode incluir uma breve "Nota de Adaptação" no início, explicando as principais mudanças realizadas e o porquê. Exemplo:

    ```markdown
    **Nota de Adaptação para: Jornal de Negócios**
    *O foco foi ajustado para o impacto financeiro e estratégico do anúncio. O headline foi reescrito para destacar o ROI, e os parágrafos que detalham o benefício para a margem operacional foram priorizados no texto.*

    ---
    
    # [Novo Headline Focado em Negócios]
    ... (resto do PR adaptado) ...
    ```