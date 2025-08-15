# Tarefa: write-boilerplate

## Finalidade

Gerar o texto padrão "Sobre a Empresa" (boilerplate), um parágrafo conciso e informativo que descreve a organização, sua missão e seu posicionamento de mercado. Este texto deve ser padronizado e reutilizável em todos os comunicados de imprensa.

---

## Entradas

- `company_name`: O nome oficial e completo da empresa (Ex: "Soluções Vértice S.A.").
- `core_business_summary`: Um resumo em uma frase do que a empresa faz (Ex: "desenvolve soluções de software baseadas em nuvem para o setor financeiro").
- `key_differentiator` (opcional): O principal diferencial ou valor da empresa (Ex: "focada em segurança de dados e conformidade com a LGPD").
- `company_website`: O URL do site oficial (Ex: "www.solucoesvertice.com.br").

---

## Dados Internos a Consultar

- `.bmad-core/data/pr-style-guide.md`: Para garantir que o tom e a terminologia do boilerplate estejam alinhados com a identidade da marca.

---

## Processamento (Passo a Passo Agentic)

1.  **Validação das Informações:**
    * Verifique se as entradas essenciais (`company_name`, `core_business_summary`, `company_website`) foram fornecidas.
    * **Elicitação Proativa:** Se o `core_business_summary` for vago, solicite mais detalhes. Ex: "Para que o boilerplate seja preciso, você poderia me dar um exemplo do principal produto ou serviço que a [company_name] oferece?".

2.  **Estruturação do Parágrafo:**
    * O agente deve seguir uma estrutura lógica para montar o parágrafo:
        * **Frase 1 (Identidade):** Comece com `[Nome da Empresa]` e conecte com o `core_business_summary`.
        * **Frase 2 (Diferencial/Missão):** Se o `key_differentiator` for fornecido, incorpore-o para adicionar profundidade e posicionamento. Caso contrário, elabore sobre a missão ou o público-alvo.
        * **Frase 3 (Call-to-Action):** Termine com um convite para saber mais, direcionando para o `company_website`.

3.  **Redação e Refinamento:**
    * Combine os elementos estruturados em um parágrafo fluido e coeso.
    * Consulte o `pr-style-guide.md` para usar a terminologia correta e o tom de voz aprovado.
    * **Reflexão:** O texto é uma representação precisa e positiva da empresa? É conciso (idealmente entre 50 e 100 palavras)? Está livre de hipérboles ou jargões excessivos?

---

## Saída Esperada

-   Um bloco de texto em Markdown, formatado com o título "Sobre a [Nome da Empresa]" e o parágrafo gerado, pronto para ser usado. Exemplo:

    ```markdown
    **Sobre a Soluções Vértice S.A.**

    A Soluções Vértice S.A. desenvolve soluções de software de ponta, baseadas em nuvem, para o setor financeiro. Com um foco rigoroso em segurança de dados e conformidade com a LGPD, a empresa ajuda seus clientes a navegar na complexidade regulatória enquanto otimizam suas operações. Para mais informações, visite [www.solucoesvertice.com](https://www.solucoesvertice.com).br.
    ```