# Tarefa: draft-pitch-email

## Finalidade

Criar um rascunho de e-mail de "pitch" conciso e personalizado para um jornalista, com o objetivo de apresentar um Press Release de forma atrativa e aumentar as chances de cobertura da mídia.

---

## Entradas

- `press_release_text`: O conteúdo do PR para extrair a notícia.
- `full_pr_link`: O URL para o comunicado completo.
- `journalist_name`: O nome do jornalista (Ex: "Ana Costa").
- `outlet_name`: O nome do veículo de mídia (Ex: "Jornal de Negócios Tech").
- `outlet_type`: O tipo de veículo (para adaptar o ângulo).

---

## Dados Internos a Consultar

- `.bmad-core/data/media-outlet-types.md`: Para entender os interesses do veículo e personalizar o ângulo.
- `.bmad-core/data/company-profile.md`: Para usar o nome da empresa e dos porta-vozes corretamente.

---

## Processamento (Passo a Passo Agentic)

1.  **Personalização do Ângulo:**
    * Analise o `outlet_type` usando o `media-outlet-types.md`. Qual é o gancho mais forte para *este* jornalista? (Ex: para um jornal de negócios, o gancho é o ROI; para um blog de tecnologia, é a inovação).

2.  **Criação de um Assunto de E-mail Atrativo:**
    * Crie um assunto curto e informativo. Ex: "Sugestão de pauta: [Nome da Empresa] lança IA que impacta o setor de logística".

3.  **Redação do Corpo do E-mail (Estrutura de 3 Parágrafos):**
    * **Parágrafo 1 (O Gancho):** Comece de forma pessoal: "Olá, [Nome do Jornalista],". Vá direto ao ponto e apresente o gancho que você definiu. "Acompanho sua cobertura sobre inovação no [Nome do Veículo] e acredito que o novo lançamento da [Nome da Empresa] será de grande interesse para seus leitores."
    * **Parágrafo 2 (O Resumo):** Resuma a notícia principal em 2-3 frases e inclua o link para o comunicado completo.
    * **Parágrafo 3 (O CTA):** Ofereça o próximo passo. "O nosso [Cargo do Porta-Voz], [Nome do Porta-Voz], está disponível para uma entrevista exclusiva para falar sobre o impacto desta tecnologia. Você teria interesse?"

4.  **Finalização Profissional:**
    * Termine com uma assinatura profissional.

---

## Saída Esperada

-   O texto completo do e-mail de pitch, pronto para ser enviado.

    ```markdown
    **Assunto:** Sugestão de pauta: [Nome da Empresa] lança IA que reduz custos logísticos em 25%

    **Corpo:**

    Olá, Ana Costa,

    Acompanho sua excelente cobertura sobre o setor de tecnologia no Jornal de Negócios Tech e acredito que o mais recente anúncio da [Nome da Empresa] tem um forte alinhamento com os interesses do seu público.

    Estamos lançando hoje a "LogisAI", a primeira plataforma de logística do mercado que utiliza IA preditiva para garantir uma redução de até 25% nos custos operacionais da cadeia de suprimentos. A notícia completa pode ser lida aqui: [Inserir `full_pr_link`]

    O nosso CEO, [Nome do CEO], está disponível para uma entrevista exclusiva para detalhar o impacto desta tecnologia no mercado brasileiro. Você teria interesse em conversar com ele?

    Agradeço a atenção.

    Atenciosamente,
    [Seu Nome/Nome do Assessor]
    ```