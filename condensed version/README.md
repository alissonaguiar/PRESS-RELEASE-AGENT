README.md


Exemplo 1: Fluxo de Trabalho Completo - Lançamento de Produto
Este cenário mostra o agente em sua capacidade máxima, guiando o usuário desde a concepção até a criação de múltiplos conteúdos.

Objetivo: Anunciar um novo produto chamado "LogisAI".

Passos da Interação:

Usuário: Olá! Preciso criar um press release para o lançamento do nosso novo produto, o "LogisAI".

Agente (ativando a diretiva de perfil): Claro! Para criar o melhor comunicado, preciso de alguns detalhes. Qual é o principal objetivo deste PR? (Ex: gerar vendas, awareness). Quem é o público-alvo e qual a mensagem mais importante que eles devem lembrar sobre o "LogisAI"?

Usuário: O objetivo é gerar awareness no setor de varejo. O público são gestores de logística e e-commerce. A mensagem principal é que o LogisAI reduz custos operacionais em até 25% usando IA preditiva.

Agente: Entendido. E quem será o porta-voz para a citação?

Usuário: Nossa CEO, Juliana Santos.

Usuário: Com essas informações, por favor, use o comando draft-release.

Agente (processando a tarefa draft-release):
(O agente consulta o template, usa a lógica de generate-headlines e extract-quote, e monta o rascunho completo.)
Aqui está o rascunho do seu Press Release:

PARA DIVULGAÇÃO IMEDIATA

[Nome da Empresa] Lança "LogisAI", Plataforma de IA que Promete Reduzir Custos Logísticos em 25%

PORTO ALEGRE, RS – 15 de agosto de 2025 – A [Nome da Empresa], líder em soluções para o varejo, anunciou hoje o lançamento da "LogisAI", uma nova plataforma de software que utiliza inteligência artificial preditiva para otimizar a cadeia de suprimentos...

"A LogisAI não é apenas uma ferramenta de eficiência; é um parceiro estratégico que capacita nossos clientes a transformar dados em decisões mais inteligentes e lucrativas", afirma Juliana Santos, CEO da [Nome da Empresa].

... (resto do comunicado) ...

Usuário: Excelente. Agora, a partir deste texto, crie um post para o LinkedIn.

Agente (processando a tarefa create-linkedin-post):
Aqui está uma sugestão de post para o LinkedIn para anunciar o "LogisAI":

Temos o prazer de anunciar uma grande novidade! 🚀

A [Nome da Empresa] acaba de lançar a "LogisAI", nossa nova plataforma de IA que está redefinindo a eficiência na cadeia de suprimentos para o varejo...

✅ Redução de custos operacionais em até 25%.
✅ Otimização de rotas em tempo real com análise preditiva.

Leia o comunicado completo aqui: [Link para o PR]

#Inovacao #InteligenciaArtificial #Logistica #Varejo #[NomeDaEmpresa]

O que este exemplo demonstra: A capacidade do agente de conduzir um projeto do início ao fim, desde a coleta de requisitos (profiling) até a criação do material principal (draft-release) e a sua amplificação para mídias sociais (create-linkedin-post).

Exemplo 2: Adaptação Estratégica - Maximizando a Cobertura
Este cenário mostra a inteligência do agente em adaptar a mesma notícia para diferentes públicos.

Objetivo: Pegar o PR do "LogisAI" e criar materiais específicos para um jornalista de tecnologia.

Passos da Interação:

Usuário: Tenho o press release final do "LogisAI". Preciso de uma versão adaptada para o "Jornal de Negócios Tech", que é um veículo focado em inovação. Use o comando tailor-for-outlet.

Agente (processando a tarefa tailor-for-outlet):
(O agente consulta sua base de conhecimento media-outlet-types.md, entende que este público valoriza detalhes técnicos e inovação, e reescreve o PR.)
Entendido. Aqui está a versão adaptada para um público de tecnologia, com foco no "como funciona":

Nota de Adaptação: O foco foi ajustado para a inovação tecnológica. O headline destaca o algoritmo preditivo e o corpo do texto detalha mais a arquitetura da solução.

[Nome da Empresa] Revela Algoritmo de IA Preditiva por Trás da Nova Plataforma LogisAI

PORTO ALEGRE, RS – 15 de agosto de 2025 – A [Nome da Empresa] detalhou hoje a tecnologia por trás da "LogisAI", sua nova plataforma que utiliza um algoritmo de machine learning para analisar mais de 50 variáveis em tempo real...

Usuário: Perfeito. Agora, com base nesta versão, prepare um e-mail de pitch para a jornalista Ana Costa do "Jornal de Negócios Tech".

Agente (processando a tarefa draft-pitch-email):
Aqui está um rascunho de e-mail de pitch personalizado:

Assunto: Sugestão de pauta: O algoritmo de IA da [Nome da Empresa] que está mudando a logística

Olá, Ana Costa,

Acompanho sua cobertura sobre inteligência artificial no Jornal de Negócios Tech e acredito que nosso último lançamento será de grande interesse...

O que este exemplo demonstra: A habilidade do agente de atuar como um verdadeiro assessor de imprensa, entendendo as nuances de diferentes mídias (tailor-for-outlet) e criando a comunicação (draft-pitch-email) para engajar jornalistas de forma eficaz.

Exemplo 3: Tarefa Rápida e Iterativa - Refinando a Mensagem
Este cenário mostra como o agente pode ser usado para tarefas menores e como ele aprende com o feedback.

Objetivo: Criar apenas uma citação e melhorá-la com a ajuda do usuário.

Passos da Interação:

Usuário: Preciso de uma citação para nossa Diretora de Produto, Maria Lima, sobre a nova funcionalidade de "relatórios em tempo real". A mensagem principal é que isso dá mais poder de decisão aos nossos clientes.

Agente (processando a tarefa extract-quote):
Claro. Aqui está uma sugestão de citação:

"A nova funcionalidade de relatórios em tempo real foi projetada para dar aos nossos clientes os dados de que precisam para tomar decisões mais rápidas e informadas."

Usuário: Está bom, mas um pouco genérico. Quero que seja mais impactante. Use o comando refine-output com o feedback: "deixe o tom mais focado em 'transformação' e menos em 'funcionalidade'".

Agente (processando a tarefa refine-output):
Entendido. Refinando com foco em transformação:

"Não estamos apenas entregando relatórios; estamos entregando poder. Com dados em tempo real nas mãos, nossos clientes deixam de reagir ao passado e passam a moldar o futuro de seus negócios. É uma transformação na cultura de decisão."

O que este exemplo demonstra: A agilidade do agente para tarefas pontuais (extract-quote) e, mais importante, sua capacidade de aprender e se adaptar ao feedback do usuário em tempo real (refine-output), funcionando como um parceiro de brainstorming.