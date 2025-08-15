# Tarefa: create-facebook-post

## Finalidade

Adaptar um Press Release para um post de Facebook, criando uma mensagem que incentive a conversação, o compartilhamento e cliques no link, aproveitando o foco da plataforma em comunidade e distribuição de conteúdo.

---

## Entradas

- `press_release_text`: O conteúdo completo do Press Release.
- `announcement_profile`: O perfil do anúncio, especialmente a `key_message` e a `audience`.
- `full_pr_link`: O URL onde o comunicado de imprensa completo está hospedado.
- `company_facebook_page_handle` (opcional): O @handle da página da empresa no Facebook.

---

## Dados Internos a Consultar

- O `press_release_text` para extrair a notícia e seus detalhes.
- (Sugerido) `.bmad-core/data/facebook-best-practices.md`: Um guia com as melhores práticas da plataforma (uso de imagens, escrita para compartilhamento, etc.).

---

## Processamento (Passo a Passo Agentic)

1.  **Análise e Sugestão de Visual:**
    * Analise o PR e sugira um visual forte para acompanhar o texto. No Facebook, imagens claras, infográficos e vídeos curtos funcionam muito bem para aumentar o alcance.
    * A sugestão deve ser uma imagem que resuma o anúncio ou um vídeo curto e explicativo.

2.  **Redação do Texto do Post:**
    * **Hook Conversacional:** Comece com uma pergunta ou uma frase que se conecte com um problema ou desejo do público. (Ex: "Cansado de atrasos e custos inesperados na sua logística? Temos uma novidade que pode ajudar.").
    * **Corpo Explicativo:** Escreva um texto um pouco mais detalhado que o do Instagram, mas ainda conciso e de fácil leitura. Use parágrafos curtos e emojis para manter o tom amigável. Explique o que é o anúncio e, mais importante, por que o público deveria se importar.
    * **Inclusão do Link:** O Facebook é excelente para direcionar tráfego. Inclua o `full_pr_link` de forma clara após o texto principal.
    * **CTA (Call-to-Action):** Incentive a ação. Peça para as pessoas lerem, comentarem e compartilharem. (Ex: "Leia a notícia completa, deixe sua opinião nos comentários e compartilhe com quem possa se interessar!").

3.  **Seleção de Hashtags:**
    * O uso de hashtags no Facebook é mais para categorização. Selecione de 2 a 4 hashtags principais e relevantes. (Ex: `#Logistica #InteligenciaArtificial #[NomeDaEmpresa]`).

4.  **Revisão Final:**
    * **Reflexão:** O post é informativo? O tom é apropriado para o Facebook? O link está visível e o CTA incentiva o clique e o compartilhamento?

---

## Saída Esperada

-   Um bloco de texto em Markdown com a sugestão de visual e o texto completo para o post do Facebook.

    ```markdown
    **Sugestão de Post para Facebook**

    ---

    **1. Sugestão de Visual:**
    Uma imagem de alta qualidade no formato de infográfico, com o logo da "LogisAI" e 3 ícones que representam seus principais benefícios: um caminhão com um relógio (velocidade), um cofre (economia) e um cérebro com circuitos (IA Preditiva).

    ---

    **2. Texto do Post:**

    Cansado de atrasos e custos inesperados na sua operação logística? 🤔

    Temos uma grande novidade! Apresentamos a "LogisAI", nossa nova plataforma que usa o poder da Inteligência Artificial para tornar a sua cadeia de suprimentos mais inteligente e preditiva.

    Isso significa menos incerteza e mais eficiência para o seu negócio, com otimização de rotas em tempo real e redução de custos operacionais.

    Queremos saber sua opinião! O que você acha do uso de IA para revolucionar a logística?

    Leia o comunicado completo para saber todos os detalhes e compartilhe esta novidade!
    👇
    [Inserir o `full_pr_link`]

    #Logistica #InteligenciaArtificial #Inovacao #[NomeDaEmpresa]
    ```