# Tarefa: suggest-distribution-channels

## Finalidade

Recomendar uma lista estratégica de canais e tipos de veículos de mídia para a distribuição de um Press Release, com base no seu tópico e público-alvo, a fim de maximizar o alcance relevante e as chances de publicação.

---

## Entradas

- `topic`: O tema central do Press Release (Ex: "Lançamento de plataforma de e-commerce sustentável").
- `announcement_profile`: O perfil do anúncio, especialmente:
    - `audience`: O público que se deseja alcançar (Ex: "Varejistas de moda", "Consumidores ecologicamente conscientes").
    - `objective`: O objetivo do PR (Ex: "Gerar awareness", "Atrair parceiros de varejo").

---

## Dados Internos a Consultar

- `.bmad-core/data/media-outlet-types.md`: Para mapear o público-alvo aos perfis de mídia mais adequados.

---

## Processamento (Passo a Passo Agentic)

1.  **Análise do Perfil de Distribuição:**
    * Analise o `topic` e o `announcement_profile`. Quem precisa saber desta notícia? Qual ecossistema de mídia cobre este assunto?

2.  **Mapeamento de Público para Veículos de Mídia:**
    * Use a `audience` informada para encontrar os perfis correspondentes no arquivo `media-outlet-types.md`.
    * **Raciocínio:** Se a `audience` é "Varejistas de moda", o agente deve selecionar os perfis "Revista de Varejo / Portal Setorial" e talvez "Jornal de Negócios". Se a `audience` também inclui "Consumidores ecologicamente conscientes", ele deve adicionar o perfil "Revista de Lifestyle / Blog de Tendências".

3.  **Geração de Categorias de Canais:**
    * Com base nos perfis de mídia selecionados, crie uma lista de *categorias* de canais recomendados.

4.  **Sugestão de Exemplos Ilustrativos:**
    * Para cada categoria, forneça 2 ou 3 exemplos de veículos de mídia conhecidos para tornar a recomendação mais concreta. Deixe claro que são exemplos para ilustrar o perfil.

5.  **Recomendação de Táticas Adicionais:**
    * Pense além da mídia tradicional e sugira outros métodos de distribuição:
        * **Serviços de Distribuição (Newswires):** Sugira plataformas pagas que distribuem comunicados em massa para redações (Ex: PR Newswire).
        * **Mídias Sociais:** Recomende as plataformas mais adequadas (Ex: LinkedIn para anúncios B2B, Twitter/X para notícias urgentes, Instagram/TikTok para apelo visual).
        * **Comunidades de Nicho:** Sugira a divulgação em fóruns especializados, grupos de LinkedIn ou subreddits relevantes onde o público-alvo se encontra.

6.  **Estruturação da Saída:**
    * Organize as recomendações em uma lista clara e priorizada, começando pelos canais mais diretos e relevantes.

---

## Saída Esperada

-   Um documento em Markdown com uma lista estruturada de canais de distribuição sugeridos. Exemplo:

    ```markdown
    **Recomendações de Canais de Distribuição para o seu Anúncio**

    Com base no tópico de "e-commerce sustentável" e no seu público-alvo, sugiro focar a distribuição nos seguintes tipos de canais:

    **1. Mídia Setorial de Varejo e Moda (Prioridade Alta):**
    * **Foco:** Atingir diretamente os decisores do setor.
    * **Exemplos:** Mercado & Consumo, E-commerce Brasil, portais de notícias da indústria da moda.

    **2. Mídia de Sustentabilidade e Lifestyle (Prioridade Média):**
    * **Foco:** Engajar o consumidor final e formadores de opinião sobre o tema.
    * **Exemplos:** Blogs de consumo consciente, seções de sustentabilidade em grandes portais, revistas de lifestyle.

    **3. Mídia de Negócios e Tecnologia:**
    * **Foco:** Destacar o ângulo de inovação e o potencial de negócio da plataforma.
    * **Exemplos:** Pequenas Empresas & Grandes Negócios, seções de tecnologia em jornais de negócios.

    **Táticas Adicionais:**

    * **LinkedIn:** Publicar um artigo detalhado no perfil da empresa e dos executivos, marcando influenciadores do setor de varejo.
    * **Grupos de Comunidade:** Compartilhar a notícia em grupos de LinkedIn para "Profissionais de E-commerce" e "Líderes de Varejo".
    ```