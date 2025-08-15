# Coleção de Tarefas Criativas

---
## Tarefa: draft-release

### Finalidade
Gerar um rascunho completo e bem estruturado de um Press Release (PR), traduzindo o contexto de um anúncio em uma narrativa noticiável e alinhada aos objetivos de comunicação da empresa.

### Entradas
- `context`: Descrição inicial do anúncio.
- `announcement_profile`: O perfil do anúncio.

### Processamento
1.  **Análise e Validação do Contexto:** Confirme o recebimento e verifique se as informações são suficientes. Se não, inicie uma elicitação proativa.
2.  **Seleção do Template Adequado:** Com base no `announcement_profile.type`, selecione o template apropriado.
3.  **Geração de Conteúdo por Seção:** Invoque as lógicas das tarefas `generate-headlines`, `extract-quote` e `write-boilerplate` para preencher as seções. Construa o corpo do texto e a dateline.
4.  **Revisão e Refinamento:** Releia o rascunho completo para garantir fluidez, clareza e consistência. Solicite feedback ao usuário.

### Saída Esperada
- Um documento Markdown (`press_release_[topico].md`) com o rascunho completo do PR.

---
## Tarefa: generate-headlines

### Finalidade
Gerar uma variedade de headlines e subheadlines de alto impacto, explorando diferentes ângulos de comunicação.

### Entradas
- `topic`: O tema central do anúncio.
- `announcement_profile`: O perfil do anúncio (público, objetivo).
- `quantity` (opcional): Número de headlines a gerar.

### Processamento
1.  **Análise do Tópico e Perfil:** Decomponha o tópico e analise o público e objetivo.
2.  **Brainstorming de Ângulos Estratégicos:** Gere abordagens diferentes (Benefício Direto, Inovação, Problema Resolvido, Impacto no Mercado).
3.  **Redação dos Headlines:** Crie títulos para cada ângulo, usando verbos de ação do `agent_knowledge_base.md`.
4.  **Criação dos Subheadlines:** Crie subtítulos que complementem cada headline.
5.  **Revisão e Curadoria:** Avalie e ordene a lista de headlines gerados.

### Saída Esperada
- Uma lista numerada em Markdown com pares de headline/subheadline.

---
## Tarefa: extract-quote

### Finalidade
Gerar uma citação estratégica, autêntica e de impacto para um porta-voz.

### Entradas
- `spokesperson_name`, `spokesperson_title`
- `key_message`
- `announcement_profile`

### Processamento
1.  **Análise do Contexto e do Porta-Voz:** Analise o cargo, o público e o objetivo para definir o tom da citação.
2.  **Definição do Objetivo Estratégico da Citação:** Escolha um objetivo (Dar Visão, Explicar o "Porquê", Criar Empatia, Destacar Benefício).
3.  **Brainstorming de Ângulos:** Gere ângulos para a citação (Visionário, Focado no Cliente, Focado no Impacto).
4.  **Redação do Rascunho:** Redija 1-2 opções de forma conversacional e concisa.
5.  **Refinamento e Polimento:** Leia e verifique se a citação soa autêntica e adiciona valor.

### Saída Esperada
- Um bloco de texto em Markdown formatado como uma citação.

---
## Tarefa: write-boilerplate

### Finalidade
Gerar o texto padrão "Sobre a Empresa" (boilerplate), conciso e informativo.

### Entradas
- `company_name`, `core_business_summary`, `key_differentiator` (opcional), `company_website`

### Processamento
1.  **Validação das Informações:** Verifique as entradas e solicite detalhes se necessário.
2.  **Estruturação do Parágrafo:** Siga a estrutura: Frase 1 (Identidade), Frase 2 (Diferencial), Frase 3 (CTA).
3.  **Redação e Refinamento:** Combine os elementos em um parágrafo coeso e revise a concisão e o tom.

### Saída Esperada
- Um bloco de texto em Markdown com o título "Sobre a [Nome da Empresa]" e o parágrafo gerado.

---
## Tarefa: create-faq

### Finalidade
Antecipar e formular respostas para as perguntas mais prováveis da imprensa sobre o Press Release.

### Entradas
- `press_release_text`: O conteúdo completo do PR.
- `announcement_profile`: O perfil do anúncio.
- `quantity` (opcional): Número de Q&As a gerar.

### Processamento
1.  **Análise Crítica do Comunicado:** Leia o PR com um olhar de jornalista para identificar pontos de dúvida.
2.  **Brainstorming de Perguntas:** Simule diferentes personas (Jornalista Esclarecedor, Cético, Analista de Negócios) para formular perguntas.
3.  **Seleção e Formulação das Perguntas:** Escolha as perguntas mais relevantes.
4.  **Redação das Respostas:** Elabore respostas concisas, diretas e consistentes com o PR.
5.  **Revisão do FAQ:** Verifique se as Q&As cobrem as dúvidas principais e são fáceis de entender.

### Saída Esperada
- Um documento em Markdown com uma seção de FAQ.