# Tarefa: draft-release

## Finalidade

Gerar um rascunho completo e bem estruturado de um Press Release (PR), traduzindo o contexto de um anúncio em uma narrativa noticiável e alinhada aos objetivos de comunicação da empresa.

---

## Entradas

- `context`: Descrição inicial do anúncio (Ex: "Lançamento do novo produto X, focado em sustentabilidade").
- `announcement_profile` (gerado pela diretiva de perfil):
    - `type`: Lançamento de produto, resultados financeiros, etc.
    - `audience`: Público-alvo (investidores, consumidores).
    - `key_message`: A mensagem central.
    - `objective`: O objetivo do PR (awareness, leads).
    - `spokesperson`: Nome e cargo do porta-voz.

---

## Processamento (Passo a Passo Agentic)

1.  **Análise e Validação do Contexto:**
    * Confirme o recebimento do `context` e do `announcement_profile`.
    * **Reflexão:** As informações no `announcement_profile` são suficientes para criar um PR eficaz? A `key_message` é clara? O `objective` está bem definido?
    * **Elicitação Proativa:** Se alguma informação crucial estiver faltando, inicie uma microinteração para obtê-la.
        * Exemplo: "Você mencionou que o porta-voz é o CEO. Qual é a principal ideia que ele(a) gostaria de transmitir na sua citação para este anúncio?"

2.  **Seleção do Template Adequado:**
    * Com base no `announcement_profile.type`, selecione o template mais apropriado.
        * Se `type` for "Lançamento de Produto", use `.bmad-core/templates/product-launch-tmpl.yaml`.
        * Para outros casos, use o padrão `.bmad-core/templates/press-release-standard-tmpl.yaml`.

3.  **Geração de Conteúdo por Seção (Invocando Sub-tarefas):**
    * **Headlines:** Invoque internamente a lógica do comando `generate-headlines` para criar 3 a 5 opções de títulos e subtítulos. Selecione a mais forte para o rascunho, mas apresente as alternativas ao final.
    * **Dateline:** Insira a cidade, estado/país e a data atual (Ex: **PORTO ALEGRE, RS – 15 de agosto de 2025 –**).
    * **Parágrafo de Abertura (Lede):** Redija o primeiro parágrafo, garantindo que ele responda de forma concisa às perguntas essenciais: Quem? O quê? Quando? Onde? e Por quê?.
    * **Corpo do Texto:** Desenvolva a `key_message` em 2 a 4 parágrafos. Adicione detalhes, contexto, dados relevantes e explique a importância do anúncio.
    * **Citação do Porta-Voz:** Use a lógica do comando `extract-quote` para redigir uma citação que reforce a `key_message` com um toque humano e estratégico.
    * **Boilerplate:** Use a lógica do comando `write-boilerplate` para inserir o texto padrão "Sobre a Empresa". Se não existir, crie um placeholder.
    * **Informações de Contato:** Insira placeholders para "Contato de Mídia", incluindo Nome, Cargo, E-mail e Telefone.
    * **Marca de Encerramento:** Adicione `###` ao final do comunicado para seguir a prática padrão.

4.  **Revisão e Refinamento:**
    * Releia o rascunho completo para garantir fluidez, clareza e consistência no tom de voz. Verifique se o texto está livre de jargões excessivos e se o `objective` do PR foi atendido.
    * Solicite feedback ao usuário: "Este rascunho captura a essência do anúncio? O tom está alinhado com a nossa marca? Há algum ponto que precise de mais ênfase?".

---

## Saída Esperada

-   Um documento Markdown (`press_release_[topico].md`) contendo o rascunho completo do Press Release, pronto para revisão e customização final.
-   O documento incluirá placeholders claros para informações que precisam ser inseridas manualmente (Ex: `[INSERIR NOME DO CONTATO DE MÍDIA]`).