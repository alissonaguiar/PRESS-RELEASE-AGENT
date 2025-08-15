# Tarefa: extract-quote

## Finalidade

Gerar uma citação (quote) estratégica, autêntica e de impacto para um porta-voz, que reforce a mensagem principal do Press Release, adicione uma perspectiva humana e capture a essência da visão da empresa sobre o anúncio.

---

## Entradas

- `spokesperson_name`: O nome completo do porta-voz (Ex: "Juliana Santos").
- `spokesperson_title`: O cargo do porta-voz (Ex: "Diretora de Inovação").
- `key_message`: A mensagem central que o Press Release quer comunicar.
- `announcement_profile`: O perfil do anúncio, especialmente o `audience` (público-alvo) e o `objective` (objetivo).

---

## Dados Internos a Consultar

- `.bmad-core/data/pr-style-guide.md`: Para garantir que a linguagem da citação esteja alinhada ao tom de voz geral da marca.

---

## Processamento (Passo a Passo Agentic)

1.  **Análise do Contexto e do Porta-Voz:**
    * Analise o cargo (`spokesperson_title`). Um CEO falará mais sobre visão e mercado. Um Diretor de Produto falará mais sobre a solução para o cliente.
    * Identifique a `audience`. Uma citação para investidores deve focar em crescimento e mercado. Uma para consumidores deve focar em benefícios e experiência.
    * Entenda o `objective`. Se o objetivo é gerar confiança, a citação deve ser mais visionária. Se é gerar vendas, deve ser focada em benefícios.

2.  **Definição do Objetivo Estratégico da Citação:**
    * **Reflexão:** Qual o papel desta citação? O que ela precisa adicionar que o resto do texto não faz? Escolha um objetivo principal:
        * **Dar Visão de Futuro:** Pintar um quadro de como o anúncio impactará o futuro.
        * **Explicar o "Porquê":** Conectar o anúncio à missão e aos valores da empresa.
        * **Criar Empatia:** Focar na perspectiva do cliente e no problema que está sendo resolvido.
        * **Destacar um Benefício-Chave:** Reforçar o benefício mais importante de forma memorável.

3.  **Brainstorming de Ângulos para a Citação:**
    * Com base no objetivo estratégico, gere internamente 2-3 ângulos possíveis:
        * **O Visionário:** "Este lançamento não é apenas sobre um produto, é sobre redefinir o futuro da indústria..."
        * **O Focado no Cliente:** "Ouvimos nossos clientes e a principal dificuldade era X. Este anúncio é a nossa resposta direta a esse desafio..."
        * **O Focado no Impacto:** "O impacto real disso será sentido na forma como nossos usuários conseguirão alcançar Y com muito mais facilidade..."

4.  **Redação do Rascunho da Citação:**
    * Escolha o ângulo mais forte e redija 1 ou 2 opções de citação.
    * **Regra de Ouro:** Escreva de forma conversacional. A citação deve soar como algo que uma pessoa realmente diria. Evite linguagem excessivamente formal ou jargões.
    * Incorpore a `key_message` de forma natural, não como uma repetição.
    * Mantenha a citação concisa, idealmente com 2 a 3 frases curtas e diretas.

5.  **Refinamento e Polimento:**
    * Leia a citação em voz alta (metaforicamente). Ela flui bem? É fácil de entender e citar?
    * Verifique se ela adiciona personalidade e autoridade ao comunicado.
    * Atribua a citação corretamente ao nome e cargo do porta-voz.

---

## Saída Esperada

-   Um bloco de texto em Markdown, formatado como uma citação, pronto para ser inserido no template do Press Release. Exemplo:

    ```markdown
    > "Este não é apenas mais um software no mercado. É a materialização da nossa visão de um futuro onde a logística é inteligente, preditiva e totalmente transparente. Estamos capacitando nossos clientes a transformar um de seus maiores desafios operacionais em uma vantagem competitiva."
    >
    > **– Juliana Santos, Diretora de Inovação**
    ```