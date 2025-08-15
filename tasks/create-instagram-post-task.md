# Tarefa: create-instagram-post

## Finalidade

Adaptar um Press Release para o formato do Instagram, criando uma sugestão de conteúdo visual e uma legenda (caption) que seja engajadora, concisa e otimizada com hashtags para maximizar o alcance e a interação.

---

## Entradas

- `press_release_text`: O conteúdo completo do Press Release.
- `announcement_profile`: O perfil do anúncio, especialmente a `key_message` e a `audience`.
- `full_pr_link`: O URL do comunicado de imprensa para ser usado no "link na bio".
- `company_instagram_handle` (opcional): O @handle da empresa no Instagram.

---

## Dados Internos a Consultar

- O `press_release_text` para extrair a essência visual e textual da notícia.
- (Sugerido) `.bmad-core/data/instagram-best-practices.md`: Um guia com as melhores práticas da plataforma (storytelling visual, estratégia de hashtags, CTAs).

---

## Processamento (Passo a Passo Agentic)

1.  **Definição do Conceito Visual (Visual-First):**
    * **Reflexão:** O Instagram é uma plataforma visual. Qual é a imagem ou vídeo mais poderoso que pode contar essa história?
    * **Brainstorming de Visuais:**
        * **Lançamento de Produto:** Uma foto de alta qualidade do produto em uso, um vídeo teaser ou um carrossel mostrando os principais recursos.
        * **Anúncio de Parceria:** Uma imagem com os logos das duas empresas ou uma foto dos líderes se cumprimentando.
        * **Resultados Financeiros:** Um infográfico simples e limpo com o principal destaque (Ex: "Crescimento de 25%").
        * **Anúncio de Evento:** O cartaz do evento ou um vídeo curto com um convite.
    * O agente deve gerar uma descrição clara da sugestão visual.

2.  **Criação da Legenda (Caption):**
    * **Hook Cativante:** Crie uma primeira linha que gere curiosidade e complemente a imagem.
    * **Storytelling Conciso:** Resuma a notícia em 2 a 4 frases curtas, usando uma linguagem mais pessoal e direta. Emojis podem ser usados para adicionar personalidade e quebrar o texto.
    * **Citação de Impacto:** Se usar uma citação, ela deve ser muito curta e inspiradora.
    * **Call-to-Action (CTA):** Direcione o usuário para a ação desejada. Como links não são clicáveis nas legendas, o padrão é usar "Clique no link na nossa bio para saber mais!". Incentive a interação com perguntas como "O que vocês acharam da novidade? Contem pra gente nos comentários! 👇".

3.  **Desenvolvimento da Estratégia de Hashtags:**
    * Gere uma lista de 7 a 15 hashtags para maximizar a descoberta.
    * **Estrutura Sugerida:**
        * **Hashtags de Nicho:** Específicas sobre o tópico (Ex: `#InteligenciaArtificialNaLogistica`).
        * **Hashtags de Comunidade:** Usadas pelo seu público (Ex: `#StartupBrasil`, `#InovacaoTecnologica`).
        * **Hashtags Amplas:** Populares e relacionadas ao seu setor (Ex: `#Tecnologia`, `#Sustentabilidade`).
        * **Hashtag da Marca:** `#[NomeDaEmpresa]`.

4.  **Revisão Final:**
    * O texto da legenda complementa a sugestão de visual? A mensagem está clara? O CTA e as hashtags estão otimizados?

---

## Saída Esperada

-   Um bloco de texto em Markdown com duas seções claras: a sugestão de visual e o texto completo da legenda, pronto para ser usado.

    ```markdown
    **Sugestão de Post para Instagram**

    ---

    **1. Sugestão de Visual:**
    Um vídeo curto (Reels) de 15 segundos mostrando a interface da plataforma "LogisAI" em ação, com transições rápidas que destacam 3 benefícios principais (ex: "Rotas Otimizadas", "Custos Reduzidos", "Entregas no Prazo"). A música de fundo deve ser moderna e energética.

    ---

    **2. Texto da Legenda (Caption):**

    O futuro da logística chegou. 🤖✨

    Estamos muito orgulhosos de apresentar a "LogisAI", nossa nova plataforma de Inteligência Artificial que está transformando a cadeia de suprimentos!

    Chega de adivinhar. Com a LogisAI, você tem o poder de prever gargalos, otimizar rotas em tempo real e garantir entregas mais rápidas e econômicas.

    Quer revolucionar sua operação? 💡

    Clique no link na nossa bio para descobrir tudo!

    #Inovacao #Tecnologia #InteligenciaArtificial #Logistica #SupplyChain #Eficiencia #StartupBrasil #Lancamento #[NomeDaEmpresa]
    ```