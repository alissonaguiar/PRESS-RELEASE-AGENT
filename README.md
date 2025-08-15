# PRESS-RELEASE-AGENT

O PRESS-RELEASE-AGENT é um projeto para automatizar e organizar a criação, revisão e distribuição de press releases, facilitando o trabalho de comunicação e marketing.

## Funcionalidades

- Modelos e checklists para press releases
- Tarefas para geração de conteúdo (posts, e-mails, FAQs, etc)
- Base de conhecimento e instruções para melhores práticas
- Sugestão de canais de distribuição e métricas de sucesso

## Estrutura do Projeto

```
condensed version/         # Documentação condensada e templates
data/                     # Dados de apoio (empresa, mídia, verbos, etc)
tasks/                    # Tarefas para automação de conteúdo
templates/                # Templates de press release
checklists/               # Checklists de revisão
```

## Como usar

1. Clone o repositório:
   ```sh
   git clone https://github.com/alissonaguiar/PRESS-RELEASE-AGENT.git
   ```
2. Navegue pelas pastas para acessar templates, tarefas e checklists.
3. Siga as instruções dos arquivos `README.md` e `Instructions.md` para cada etapa do processo.

## Contribuição

Contribuições são bem-vindas!  
Abra uma issue ou envie um pull request com sugestões, correções ou novas funcionalidades.

## Licença

Este projeto está sob a licença MIT.

## Como usar como GEM (Gemini) ou GPT (ChatGPT)


> **Atenção:** Somente os arquivos da pasta `condensed version/` devem ser utilizados para configurar GEMs do Gemini ou GPTs personalizados do ChatGPT. Os arquivos das demais pastas possuem o mesmo conteúdo, mas estão organizados separadamente apenas para facilitar a visualização das tarefas e templates.

### Gemini (GEM)

1. Importe os arquivos da pasta `condensed version/` para o painel de criação de GEMs do Gemini.
2. Utilize o arquivo `condensed version/Instructions.md` como instrução principal da GEM, garantindo que o agente siga as orientações e o fluxo sugerido.
3. Siga as orientações do Gemini para mapear cada tarefa e template conforme desejado.
4. Teste a GEM com prompts de exemplo para garantir que as respostas estejam alinhadas ao objetivo do projeto.

### ChatGPT (GPT personalizado)

1. Acesse a área de criação de GPTs personalizados em https://chat.openai.com/gpts.
2. Faça upload apenas dos arquivos da pasta `condensed version/`.
3. Utilize o arquivo `condensed version/Instructions.md` como instrução principal do GPT, inserindo seu conteúdo no campo de instruções do modelo.
4. Personalize o comportamento do GPT conforme necessário, utilizando os exemplos e instruções do projeto.
5. Teste o GPT com prompts reais para validar o funcionamento.
