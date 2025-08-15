# Tarefa: create-linkedin-post

## Finalidade

Transformar o conteúdo de um Press Release formal em um post para o LinkedIn que seja conciso, profissional e engajador. O objetivo é capturar a atenção do público na plataforma, gerar discussão e direcionar tráfego para a notícia completa.

---

## Entradas

- `press_release_text`: O conteúdo completo do Press Release que servirá como fonte.
- `announcement_profile`: O perfil do anúncio, especialmente a `key_message` e a `audience`.
- `full_pr_link`: O URL onde o comunicado de imprensa completo está hospedado.
- `spokesperson_name` (opcional): Nome do porta-voz principal para ser mencionado.
- `company_linkedin_handle` (opcional): O @handle da empresa no LinkedIn para ser marcado.

---

## Dados Internos a Consultar

- O `press_release_text` para extrair os pontos-chave.
- `.bmad-core/data/pr-style-guide.md`: Para manter a consistência do tom de voz da marca.
- (Sugerido) `.bmad-core/data/linkedin-best-practices.md`: Um guia com as melhores práticas da plataforma (uso de hashtags, formatação, CTAs).

---

## Processamento (Passo a Passo Agentic)

1.  **Extração da Essência da Notícia:**
    * Analise o `press_release_text` e identifique os 3 elementos mais importantes:
        1.  **A Notícia Principal:** Qual é o fato central em uma única frase?
        2.  **O Principal Benefício:** Qual é o impacto mais significativo para a `audience`?
        3.  **O Dado ou Citação de Impacto:** Qual é a estatística mais forte ou a frase mais memorável da citação?

2.  **Criação do "Hook" (A Primeira Frase):**
    * A primeira linha é crucial para prender a atenção. Redija uma abertura forte e direta.
    * **Técnicas:** Comece com uma pergunta, uma estatística surpreendente ou uma declaração ousada sobre o futuro do setor.
    * Exemplo: "E se a sua logística pudesse prever o futuro? Hoje, estamos dando o primeiro passo nessa direção."

3.  **Estruturação do Corpo do Post:**
    * Mantenha o texto aerado, usando parágrafos curtos (1-2 linhas) e espaços em branco.
    * Resuma a notícia principal em 2 a 3 frases.
    * Use bullet points (com emojis profissionais como 💡, 🚀, ✅) para destacar 2 ou 3 benefícios ou características principais.
    * Incorpore a menção ao porta-voz e à empresa, se os handles foram fornecidos (Ex: "Com a liderança de `[Nome do Porta-Voz]`...").
    * Inclua um Call-to-Action (CTA) claro no final do texto. O que o leitor deve fazer? (Ex: "Leia o comunicado completo", "Deixe sua opinião nos comentários", "Visite nosso site para saber mais").

4.  **Seleção de Hashtags Estratégicas:**
    * Gere de 3 a 5 hashtags relevantes.
    * O ideal é uma combinação de:
        * **Hashtags de Setor:** (Ex: `#Logistica`, `#Varejo`, `#InteligenciaArtificial`)
        * **Hashtags de Conceito:** (Ex: `#Inovacao`, `#Tecnologia`, `#FuturoDoTrabalho`)
        * **Hashtag da Marca:** (Ex: `#[NomeDaEmpresa]`)

5.  **Revisão Final (Otimização para LinkedIn):**
    * **Reflexão:** O post é escaneável? A mensagem principal é clara nos primeiros segundos? Ele convida à interação? O tom é adequado para uma rede profissional? O link para o PR completo está incluído?

---

## Saída Esperada

-   Um bloco de texto em Markdown, pronto para ser copiado e colado no LinkedIn, contendo todos os elementos do post. Exemplo:

    ```markdown
    Temos o prazer de anunciar uma grande novidade! 🚀

    A [Nome da Empresa] acaba de lançar a "LogisAI", nossa nova plataforma de IA que está redefinindo a eficiência na cadeia de suprimentos.

    Com esta nova solução, nossos clientes podem esperar:
    ✅ Redução de custos operacionais em até 25%.
    ✅ Otimização de rotas em tempo real com análise preditiva.
    ✅ Aumento