# Tarefa: create-faq

## Finalidade

Antecipar e formular respostas claras para as perguntas mais prováveis que jornalistas, analistas e stakeholders possam ter após lerem o Press Release. O objetivo é garantir a consistência da mensagem, preparar os porta-vozes e facilitar a criação de matérias pela imprensa.

---

## Entradas

- `press_release_text`: O conteúdo completo do Press Release que foi gerado.
- `announcement_profile`: O perfil do anúncio, para entender o contexto, a audiência e os objetivos.
- `quantity` (opcional): Número de pares de Pergunta e Resposta a serem gerados (padrão: 5).

---

## Dados Internos a Consultar

- O próprio `press_release_text` é a fonte primária de informação para as respostas.
- (Opcional) `.bmad-core/data/company-competitive-landscape.md`: Para antecipar perguntas sobre concorrentes.

---

## Processamento (Passo a Passo Agentic)

1.  **Análise Crítica do Comunicado:**
    * Leia o `press_release_text` com um olhar cético e curioso, como um jornalista faria.
    * Identifique as principais afirmações, dados, novidades e qualquer ponto que possa gerar dúvida ou necessitar de mais detalhes.

2.  **Brainstorming de Perguntas (Simulando Personas):**
    * Adote diferentes perspectivas para formular as perguntas:
        * **O Jornalista Esclarecedor:** Foca em entender os detalhes. ("O que exatamente o novo produto faz?", "Quando estará disponível para o consumidor?").
        * **O Jornalista Cético:** Questiona o "porquê" e o impacto real. ("Por que lançar isso agora?", "Qual o diferencial real em relação ao que já existe no mercado?").
        * **O Analista de Negócios:** Foca no mercado e na estratégia. ("Qual o impacto esperado nas receitas?", "Como isso posiciona a empresa frente à concorrência?").
        * **O Consumidor Final:** Foca nos benefícios práticos. ("Como isso vai facilitar a minha vida?", "Quanto vai custar?").

3.  **Seleção e Formulação das Perguntas:**
    * Com base no brainstorming, selecione as `quantity` perguntas mais relevantes e prováveis.
    * Redija as perguntas de forma clara e direta, como seriam feitas em uma entrevista.

4.  **Redação das Respostas:**
    * Para cada pergunta, elabore uma resposta concisa, direta e informativa.
    * **Regra de Ouro:** A resposta deve ser consistente com o `press_release_text` e nunca contradizê-lo.
    * Use a resposta como uma oportunidade para reforçar a `key_message` do anúncio.
    * Mantenha o tom de voz definido no `.bmad-core/data/pr-style-guide.md`.
    * Evite respostas evasivas. Seja transparente e objetivo.

5.  **Revisão do FAQ:**
    * **Reflexão:** O conjunto de Perguntas e Respostas cobre as dúvidas mais óbvias? As respostas são fáceis de entender? Elas ajudam um jornalista a escrever uma matéria mais completa?

---

## Saída Esperada

-   Um documento em Markdown com uma seção de FAQ, formatado de maneira clara para fácil leitura. Exemplo:

    ```markdown
    **Perguntas Frequentes (FAQ)**

    **1. Por que a [Nome da Empresa] está lançando este produto agora?**
    Acreditamos que o mercado atingiu um ponto de maturidade onde a necessidade por soluções logísticas inteligentes não é mais um diferencial, mas uma necessidade. O lançamento agora posiciona nossos clientes à frente da concorrência, permitindo que otimizem suas operações antes dos picos de demanda do final do ano.

    **2. Como a nova plataforma se diferencia da solução oferecida pelo Concorrente X?**
    Enquanto outras soluções focam apenas no rastreamento, nossa plataforma "LogisAI" utiliza uma camada de Inteligência Artificial preditiva que não só mostra onde a entrega está, mas antecipa gargalos e sugere rotas alternativas em tempo real, gerando uma economia de custos e tempo significativamente maior.

    ... (e assim por diante)
    ```