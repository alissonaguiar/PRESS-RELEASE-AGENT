# Coleção de Tarefas Estratégicas

---
## Tarefa: tailor-for-outlet

### Finalidade
Adaptar um Press Release geral para um tipo de veículo de mídia específico, ajustando o ângulo, tom e linguagem.

### Entradas
- `press_release_text`, `outlet_type`, `announcement_profile`

### Processamento
1.  **Análise do Veículo de Mídia:** Consulte o `agent_knowledge_base.md` para entender o perfil do veículo (público, interesses).
2.  **Definição do Novo Ângulo Noticioso:** Determine qual aspecto do anúncio é mais interessante para aquele público.
3.  **Reescrita Estratégica do Conteúdo:** Reestruture o PR, reescrevendo o título, o primeiro parágrafo e reordenando o corpo do texto para refletir o novo ângulo.
4.  **Ajuste de Tom e Linguagem:** Adapte o vocabulário e o tom para o esperado pelo veículo.

### Saída Esperada
- O texto do PR reescrito e uma "Nota de Adaptação" explicando as mudanças.

---
## Tarefa: suggest-distribution-channels

### Finalidade
Recomendar uma lista estratégica de canais e tipos de veículos para a distribuição de um Press Release.

### Entradas
- `topic`, `announcement_profile`

### Processamento
1.  **Análise do Perfil de Distribuição:** Analise o tópico e o público-alvo.
2.  **Mapeamento de Público para Veículos:** Use o `agent_knowledge_base.md` para encontrar os perfis de mídia correspondentes.
3.  **Geração de Categorias de Canais:** Crie uma lista de categorias de canais recomendados.
4.  **Sugestão de Exemplos Ilustrativos:** Forneça 2-3 exemplos de veículos para cada categoria.
5.  **Recomendação de Táticas Adicionais:** Sugira outros métodos (newswires, mídias sociais, comunidades de nicho).
6.  **Estruturação da Saída:** Organize as sugestões em uma lista clara e priorizada.

### Saída Esperada
- Uma lista em Markdown com os canais de distribuição sugeridos.

---
## Tarefa: draft-pitch-email

### Finalidade
Criar um rascunho de e-mail de "pitch" conciso e personalizado para um jornalista.

### Entradas
- `press_release_text`, `full_pr_link`, `journalist_name`, `outlet_name`, `outlet_type`

### Processamento
1.  **Personalização do Ângulo:** Analise o perfil do veículo para definir o gancho mais forte.
2.  **Criação de um Assunto de E-mail Atrativo:** Crie um assunto curto e informativo.
3.  **Redação do Corpo do E-mail:** Siga a estrutura de 3 parágrafos (Gancho, Resumo + Link, CTA com oferta de entrevista).
4.  **Finalização Profissional:** Use uma assinatura profissional.

### Saída Esperada
- O texto completo do e-mail de pitch.

---
## Tarefa: suggest-related-content

### Finalidade
A partir de um Press Release, gerar ideias para uma mini campanha de conteúdo para amplificar a mensagem.

### Entradas
- `press_release_text`, `announcement_profile`

### Processamento
1.  **Análise dos Temas Principais:** Identifique 2-3 subtemas no PR que podem ser aprofundados.
2.  **Brainstorming de Formatos:** Sugira formatos adequados para cada subtema (blog post, infográfico, thread, vídeo).
3.  **Criação de Esboços/Outlines:** Crie um pequeno esboço para cada sugestão, tornando-a acionável.

### Saída Esperada
- Uma lista estruturada com sugestões de conteúdo e seus esboços.

---
## Tarefa: define-success-metrics

### Finalidade
Sugerir KPIs para avaliar o sucesso e o impacto de uma campanha de Press Release.

### Entradas
- `announcement_profile` (especialmente o `objective`)

### Processamento
1.  **Mapeamento de Objetivo para Métricas:** Conecte o objetivo a categorias de métricas (Alcance, Conversão, Engajamento).
2.  **Sugestão de KPIs por Categoria:** Sugira uma lista de KPIs específicos e acionáveis.
3.  **Contextualização das Métricas:** Adicione uma breve explicação para cada métrica.

### Saída Esperada
- Uma lista categorizada de KPIs sugeridos para monitorar a campanha.