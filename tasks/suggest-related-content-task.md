# Tarefa: suggest-related-content

## Finalidade

A partir de um Press Release, gerar ideias para uma mini campanha de conteúdo, sugerindo outros formatos que possam aprofundar e amplificar a mensagem principal em diferentes canais.

---

## Entradas

- `press_release_text`: O conteúdo principal do anúncio.
- `announcement_profile`: O perfil do anúncio (público, objetivo).

---

## Processamento (Passo a Passo Agentic)

1.  **Análise dos Temas Principais:**
    * Leia o `press_release_text` e identifique 2 a 3 subtemas ou pontos de interesse que poderiam ser explorados com mais profundidade. (Ex: "a tecnologia por trás da IA", "o impacto no dia a dia do gestor de logística", "o case de um cliente piloto").

2.  **Brainstorming de Formatos de Conteúdo:**
    * Para cada subtema, sugira um formato de conteúdo adequado:
        * **Para aprofundar detalhes:** Um post de blog.
        * **Para resumir visualmente:** Um infográfico.
        * **Para gerar discussão rápida:** Um fio (thread) para o Twitter/X.
        * **Para uma mensagem do líder:** Um roteiro para um vídeo curto (1 min).

3.  **Criação de Esboços/Outlines:**
    * Para cada sugestão, crie um pequeno esboço com os principais pontos a serem abordados, tornando a ideia acionável.

---

## Saída Esperada

-   Uma lista estruturada com sugestões de conteúdo e seus respectivos esboços.

    ```markdown
    **Sugestões de Conteúdo Relacionado para Amplificar seu Anúncio:**

    **1. Post de Blog: "Por Dentro da LogisAI: A Tecnologia que Está Mudando a Logística"**
    * **Público:** Técnico/Interessados em inovação.
    * **Esboço:**
        * Introdução: O problema da logística tradicional.
        * Como funciona nosso algoritmo de análise preditiva.
        * A importância do Machine Learning para a otimização de rotas.
        * Conclusão: O futuro da logística autônoma.

    **2. Fio (Thread) para Twitter/X: "5 Fatos Sobre o Lançamento da LogisAI"**
    * **Público:** Geral/Mídia.
    * **Esboço:**
        * Tweet 1: Anúncio principal (Hook).
        * Tweet 2: O maior problema que resolvemos.
        * Tweet 3: A estatística mais impactante (25% de redução).
        * Tweet 4: Citação curta do CEO.
        * Tweet 5: Link para o PR completo (CTA).

    **3. Roteiro de Vídeo (1 min) com o CEO: "Nossa Visão para o Futuro da Logística"**
    * **Público:** Clientes e investidores.
    * **Esboço:**
        * (0-15s) O "porquê" do lançamento e a paixão pelo problema.
        * (15-45s) Demonstrar o principal benefício da "LogisAI".
        * (45-60s) Convite para conhecer a solução e visão de futuro.
    ```