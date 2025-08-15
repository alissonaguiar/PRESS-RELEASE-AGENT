# Tarefa: define-success-metrics

## Finalidade

Sugerir KPIs (Key Performance Indicators) relevantes e mensuráveis para avaliar o sucesso e o impacto de uma campanha de Press Release, alinhando os esforços de comunicação com os objetivos de negócio.

---

## Entradas

- `announcement_profile`: O perfil do anúncio, sendo o `objective` a entrada mais importante (Ex: "gerar brand awareness", "gerar leads", "informar investidores").

---

## Processamento (Passo a Passo Agentic)

1.  **Mapeamento de Objetivo para Métricas:**
    * Analise o `objective` do anúncio e conecte-o a categorias de métricas.
        * `awareness` -> Métricas de Alcance.
        * `leads` -> Métricas de Conversão.
        * `thought leadership` -> Métricas de Engajamento e Qualidade.

2.  **Sugestão de KPIs por Categoria:**
    * Com base no mapeamento, sugira uma lista de KPIs específicos e acionáveis.
    * Organize os KPIs em categorias lógicas para facilitar o entendimento.

3.  **Contextualização das Métricas:**
    * Adicione uma breve explicação para cada métrica, dizendo o que ela mede e por que é importante.

---

## Saída Esperada

-   Uma lista categorizada de KPIs sugeridos para monitorar a campanha.

    ```markdown
    **Métricas Sugeridas para Avaliar o Sucesso do seu Anúncio:**

    Com base no seu objetivo de **[inserir o `objective`]**, recomendo acompanhar as seguintes métricas:

    **1. Métricas de Cobertura de Mídia (Resultado Direto):**
    * **Número de Publicações (Clipping):** Quantos veículos de mídia publicaram a sua notícia.
    * **Qualidade da Cobertura:** Avaliar se as publicações foram em veículos de alta relevância (Tier 1) e se incluíram as mensagens-chave.
    * **Alcance Potencial (Media Impressions):** O número estimado de pessoas alcançadas pelas publicações.

    **2. Métricas de Engajamento Digital (Impacto no Público):**
    * **Menções Sociais:** Quantas vezes o anúncio foi mencionado no LinkedIn, Twitter/X, etc.
    * **Engajamento nos Posts:** Likes, comentários e compartilhamentos nas publicações oficiais sobre o anúncio.

    **3. Métricas de Negócio (Impacto Final):**
    * **Tráfego de Referência (Referral Traffic):** Quantos visitantes chegaram ao seu site através dos links nas matérias publicadas.
    * **Leads Gerados:** Se aplicável, quantos novos contatos de negócio foram gerados a partir do interesse no anúncio.
    * **Buscas pela Marca:** Um aumento no volume de buscas pelo nome da sua empresa/produto no Google após o anúncio.
    ```