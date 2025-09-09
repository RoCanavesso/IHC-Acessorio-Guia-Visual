# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](http://lattes.cnpq.br/6747210702910392) e Prof. Dr. [Plino Thomaz Aquino Junior](http://lattes.cnpq.br/6186413528999908).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Guia Visual: SIstema de Detecção de Objetos para Deficientes Visuais** sob orientação do Professor **Isaac Jesus da Silva** e desenvolvido pelos seguintes alunos:

- Rômulo Carneiro de Oliveira Canavesso
- Lucas Antunes Sampaio

## Resumo

O presente trabalho propõe o desenvolvimento de um website voltado à divulgação e comercialização de um protótipo assistivo criado para pessoas com deficiência visual. O produto em questão consiste em um acessório inteligente de óculos baseado em visão computacional, capaz de detectar elementos do ambiente urbano como pessoas, veículos e placas de sinalização e transmitir essas informações ao usuário por meio de feedback sonoro em tempo real. O site terá como objetivo apresentar as funcionalidades do dispositivo, demonstrar seu funcionamento por meio de descrições interativas e recursos multimídia, além de fornecer uma interface intuitiva para potenciais interessados. Dessa forma, busca-se aplicar princípios de Interação Humano-Computador (IHC) no design e na usabilidade da plataforma, de modo a garantir clareza, acessibilidade e engajamento na apresentação da tecnologia desenvolvida no Trabalho de Conclusão de Curso.

## Introdução

 <!--
 
- Apresente o propósito do produto ou serviço e quais são os principais benefícios que ele oferece aos usuários.
- Identifique os problemas ou necessidades que o produto ou serviço resolve ou satisfaz.
- Liste as características e funcionalidades do seu produto ou serviço de forma detalhada.
- Liste as tecnologias e ferramentas computacionais que pretendem usar neste projeto (TCC).
- Apresente o contexto de uso dessa aplicação. (“Usuários, tarefas, equipamentos (hardware, software e materiais) e o ambiente físico e social no qual um produto é usado.”)

-->

<!--

ESSA É A PARTE DO PEDRO, TOMAR COMO REFERÊNCIA!!!

A criação de datasets de imagens rotuladas é uma etapa essencial em projetos de visão computacional, especialmente no contexto de reconhecimento facial e detecção de emoções. No entanto, esse processo é, em geral, demorado e trabalhoso, exigindo classificação manual de uma grande quantidade de imagens antes que seja possível iniciar o treinamento automático de modelos de aprendizado de máquina. Este projeto busca explorar alternativas que tornem esse processo mais ágil, confiável e acessível. Ao minimizar o custo produtivo da coleta e rotulagem inicial, é possível direcionar mais atenção à curadoria e à qualidade das classificações, aspecto relevante quando se trata de emoções, que são frequentemente ambíguas e subjetivas à interpretação humana.

As expressões faciais são um dos principais meios de comunicação não verbal, permitindo a manifestação e a interpretação de sentimentos mesmo na ausência da fala. Este trabalho propõe o desenvolvimento de uma ferramenta que automatize a criação de datasets de expressões faciais humanas, associadas a diferentes emoções, com foco específico em sessões reais de jogos digitais. Diferente de abordagens existentes, que dependem de jogos específicos que instruem o jogador a imitar emoções pré-definidas, a ferramenta aqui proposta visa capturar expressões espontâneas, registradas naturalmente por uma facecam enquanto o jogador interage com qualquer jogo eletrônico. Ao relacionar essas expressões ao contexto do que está sendo exibido na tela, busca-se construir conjuntos de dados mais representativos e aplicáveis a cenários reais.

- Webcam: Será utilizada uma câmera voltada para computadores, que possua resolução de no mínimo 720p, para captura das expressões faciais do usuário. A webcam foi escolhida em relação a outros tipos de câmeras pelo seu preço, pela facilidade de utilização e pela portabilidade. Levamos em conta na escolha, também, pois já possuímos esse material em nossas residências.
- Computador: Utilizaremos um computador ou notebook que possuam no mínimo as seguintes especificações: processador i5-8400 (ou equivalente/melhor) e 16 GB de memória RAM. Usaremos essas máquinas para realizar a programação, design e desenvolvimento do projeto, assim como seus testes e correções. Também o utilizaremos como um artifício para teste e prototipação em jogos, para identificar e definir as expressões faciais do usuário. Utilizaremos o computador para testes e não videogames, pois a interface da aplicação estará no próprio aparelho, facilitando a captura.
- Dataset: Datasets contendo imagens de expressões faciais serão utilizados para a realização da comparação e identificação dessas expressões. A intenção é utilizar datasets já disponíveis, para otimizar e agilizar o processo de desenvolvimento do nosso projeto. Alguns datasets recomendados incluem: Kaggle - Face Expression Recognition Dataset e DFEW (Dynamic Facial Expression in-the-Wild).
- IA: Utilizaremos uma IA que consiga ser alimentada de modo a analisar o contexto presente na tela e reconhecer corretamente a relação entre a expressão do indivíduo e o contexto que se apresenta. Algumas IAs que podem ser utilizadas são: FER - Facial Expression Recognition e MediaPipe.

-->

<!-- 
ESSE ABAIXO É O NOSSO PROJETO! 
Precisa ser finalizado os 3 ultimos tópicos da introdução
Eu fiz baseado no nosso produto de tcc, mas eu nao sei se ele quer que descreva na introdução o prototipo do tcc ou o site que iremos fazer, ou os dois
-->
O acessório assistivo tem como propósito ampliar a autonomia e a segurança de pessoas com deficiência visual durante a locomoção em ambientes urbanos. Por meio de visão computacional, reconhecimento de textos e síntese de voz, o dispositivo possibilita que o usuário receba informações em tempo real sobre elementos relevantes ao seu redor, facilitando a orientação e promovendo maior inclusão social.

Os principais benefícios oferecidos aos usuários são:

1. **Autonomia**: o usuário pode se deslocar com mais independência, reduzindo a necessidade de auxílio constante de terceiros.

2. **Segurança**: a detecção de pessoas, veículos e placas de sinalização ajuda a evitar situações de risco no trânsito e em espaços públicos.

3. **Acessibilidade**: o feedback sonoro transforma informações visuais em mensagens auditivas claras, permitindo melhor compreensão do ambiente.

4. **Praticidade**: o formato modular, leve e portátil, permite que o acessório seja acoplado a qualquer óculos, garantindo ergonomia e conforto no uso diário.

5. **Inclusão**: o dispositivo contribui para a integração social, oferecendo às pessoas com deficiência visual maior liberdade para realizar atividades cotidianas em ambientes externos.

O acessório assistivo desenvolvido neste trabalho busca resolver um conjunto de problemas enfrentados por pessoas com deficiência visual em seu cotidiano. A locomoção autônoma em ambientes urbanos apresenta desafios significativos, uma vez que a presença de veículos, obstáculos e sinalizações pouco acessíveis aumenta o risco de acidentes e limita a segurança desses indivíduos. Além disso, informações importantes, como placas de orientação e faixas de pedestres, não são facilmente percebidas, gerando dependência constante de terceiros para a realização de tarefas simples. As tecnologias assistivas tradicionais, como bengalas e cães-guia, oferecem suporte apenas na identificação de obstáculos físicos imediatos, mas não fornecem informações contextuais sobre o ambiente. Nesse sentido, o dispositivo proposto atende às necessidades de maior autonomia, segurança e acesso à informação, contribuindo para a inclusão e a independência do usuário em espaços públicos.

## Publico Alvo

<!-- 
- Determine qual o grupo específico de pessoas ou organizações para as quais este produto ou serviço é direcionado.
- Descreva as caracteristicas demográficas, comportamentais, psicográficas ou geográficas deste público alvo que o torna mais propenso a se interessar pelo que está sendo oferecido neste projeto ou serviço.

-->
O público-alvo deste projeto são pessoas e empresas cujo trabalho impactam os seus clientes emocionalmente, como empresas de jogos, produtores de filmes e principalmente desenvolvedores que possuam projetos de DeepLearning que requer treinamento de emoções faciais.Tanto grandes estúdios de jogos quanto produtores de filmes como foco principal o desenvolvimento de entretenimento e buscam formas de aumentar o engajamento. Elas se beneficiam do projeto por promover uma maior aproximação entre o produto e consumidor, permitindo customizações mais precisas e experiências mais envolventes. Em termos de características, esse público é composto por organizações que valorizam inovação, adaptação às tendências do mercado e feedback direto do usuário, sendo mais propensas a investir em ferramentas que aumentem a retenção e a satisfação do seu público.
Enquanto a desenvolvedores de deeplearning, é comum uma etapa para desenvolvimento de uma base de dados própria porém essa atividade é extensa e trabalhosa. Este projeto como um objetivo secundário, facilitar o desenvolvimento de novas bases de dados visando encurtar o tempo necessário para a criação de um dataset original.

## Análise de concorrência
<!--
1. Identifique os principais concorrentes ou softwares mais utilizados pelo seu público-alvo.
2. Colete informações sobre os concorrentes selecionados.
3. Analise as características e funcionalidades dos concorrentes.
4. Avalie a experiência do usuário (UX).
5. Examine os preços e modelos de negócio.
6. Pesquisa de satisfação do cliente e opiniões.
7. Identifique padrões e tendências no mercado.
8. Elabore relatórios e sumarize os resultados.
9. Extraia pontos positivos e faça recomendações.
-->

1. Há vários sites que permitem a criação, download e upload de datasets, e dentre eles os mais conhecidos são o Kaggle, Hugging Face e Nevermind, onde Kaggle e Hugging Face são plataformas online onde os usuários podem, entre outras coisas, fazer download e upload de datasets. Já Nevermind é um jogo de suspence psicológico que usa a detecção de expressões faciais como artífice que torna o jogo.
2. 
   - Kaggle: Plataforma com foco em Ciência de Dados e Machine Learning, cuja função primária são suas competições, onde times ou indivíduos podem enviar seus modelos para resolver problemas específicos e ganhar prêmios, além disso ele oferece datasets, notebooks e um fórum da comunidade. Os usuários podem fazer download ou upload de datasets e notebooks;<br>
     <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/184c7fcb-7920-4c62-a615-d0173ccb2087" />
     
   - Hugging Face: Uma empresa responsável pelo desenvolvimento de ferramentas e recursos para o desenvolvimento de plicações com Machine Learning. Sua plataforma permite que os usuários colaborem em modelos de Machine Learning e datasets;<br>
     <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/305a3b5f-e3a4-4e9f-b333-70fefbb3405f" />
   
   - Nevermind: um jogo de suspence psicológico que adapta a dificuldade, visuais e som de acordo com o estresse detectado na expressão facial do jogador.<br>
     <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/2ef14b47-399c-45e6-89f7-1723d66e86a5" />

3.
   - Kaggle: Competição entre usuários utilizando modelos de Machine Learning; upload e download de datasets que podem ser públicos ou privados; upload e download de notebooks que permitem o compartilhamento de técnicas de criação de códigos e análise de dados e cursos de aprendizado de ciência de dados;
   - Hugging Face: Biblioteca Transformers que simplifica o uso de modelos transformer para geração de texto e tradução; upload e download de datasets, principalmente relacionados a modelos de Machine Learning e NLP; hub de modelos que funciona como repositório de modelos pré-treinados para tarefas relacionadas a NLP, visão computacional e áudio;
   - Nevermind: Uso de expressões faciais do jogador, captadas a partir da webcam, para alterar a jogabilidade do jogo, mudando a dificuldade, visuais e sons; O jogo se torna mais difícil conforme o estresse emocional do jogador aumenta, onde medo e ansiedade tem um foco maior.
4. A Kaggle possui uma interface minimalista e ao mesmo tempo cheia de informações, apesar de tanto texto a navegação é intuitiva.A Kaggle não foca apenas em datasets, é um ecossistema de cientistas que publicam seus estudos, com modelos e datasets utilizados e por consequência, acada se tornando um site comum para download de datasets, tendo, inclusive, uma aba dedicada apenas a datasets.
5. A kaggle baseia-se no plano freemium, onde todas as principais ferramentas são disponibilizadas de forma gratuita e a monetização vem de empresas que se interessam em criar suas próprias competições na plataforma, além da plataforma fazer parcerias com empresas como google cloud e receber uma porcentagem do prêmio das competições citadas anteriormente. Resumidamente, usuários individuais não precisam pagar um plano para ter acesso total às funcionalidades do site, mas empresas devem pagar pelo suporte da kaggle para hospedar competições pagas e para utilizar de alguma ferramenta da kaggle para projetos empresariais.
6. Na plataforma da Kaggle não existe explicitamente uma área de avaliação, mas a coleta é realizada de forma rápida distribuindo questionário de avaliação para a comunidade da kaggle fora da plataforma, opiniões de usuários em redes sociais. Também, após uma competição hosedada na kaggle, existe um formulário curto para receber o feedback daquela função. De forma um pouco mais discreta, existe a opção de reportar bugs ou falhas no sistema, que serve pode servir como crítica construtiva.
7. O mercado de Inteligência artificial vem crescendo rapidamente e de maneira desenfreada, juntamente com a IA, os datasets tornam-se fatores principais nesse meio. Desta maneira, a busca por treinamento, machine learning, só tende a aumentar e ganhar cada vez mais o mercado no mundo. Com isso, a procura por datasets / modelos treinados permite que áreas relacionadas consigam dominar.
8. O Kaggle possui um acervo enorme de datasets e informações, cerca de dezenas de milhares (de acordo com o site https://www.innovatiana.com/en/post/kaggle-for-datasets?utm_source=chatgpt.com), isso se dá pela grande quantidade de acessos e por ser open source. Este modelo vem crescendo constantemente no mercado, com mais e mais pessoas utilizando as máquinas para aprendizagem e inteligências artificiais. Com isso, a possibilidade de crescimento de Kaggle é muito grande, além disso, é a porta de entrada para muitos ourtos artifícios de acervos e disponibilização de datasets.
9. Pontos positivos:
<ul>
 <li>A plataforma Kaggle oferece muitos datasets de diversos tipos, de forma open-source;</li>
 <li>Tais datasets são disponibilizados com extensões fáceis de serem utilizadas, como CSV, Json;</li>
 <li>É um site ativo, com manutenção e adição de informações recentes,</li>
</ul>

### Personas
<!--
- Descreva as personas que irão interagir com a aplicação ou produto. Deixe claro suas principais caracteristicas e contextos sociais, econômicos e culturais.
- Quais informações sobre o usuário o serviço ou poduto deve guardar?
-->
#### Persona primária
1. Thiago Alberto Mendes, de 35 anos, é formado em Design de Jogos e atualmente trabalha como Game Director em uma empresa pequena de nome Best Games Studio. Já criou títulos como ATG VI, Armored Lore, Bright Souls. Todos esses jogos possuem características únicas, mas nenhum conseguiu colocar a empresa em posição de destaque. Sua ideia para aumentar o renome da empresa é fazer um título único e inovador.
   Thiago gostaria de adicionar em seu jogo uma mecânica única, que consiga aproximar o jogo e o jogador, de uma forma natural e que adicione elementos de jogabilidade.<br>
   <img width="256" height="256" alt="image" src="https://github.com/user-attachments/assets/840e1f88-3f76-439c-9127-e4c811bcb35c" />

2. Valter Alter, de 58 anos, tem um blog e um canal no YouTube de desenvolvimento de jogos chamado ClickGamesBR, com cerca de 1.3 milhões de inscritos. O foco de seu canal é criar, mostrar ao seu público e publicar os jogos na web. Ultimamente, seus seguidores pediram para que fizesse um jogo que interaja com o usuário a partir de suas emoções. Valter tem uma ideia de história, mas necessita que seus seguidores enviem vídeos com webcam e gameplay de diversos jogos, e dessa maneira ele poderia utilizar uma ferramenta que facilite a criação de datasets, a fim de criar o que seus seguidores desejam.<br>
    <img width="256" height="256" alt="image" src="https://github.com/user-attachments/assets/51503288-f126-448a-8377-81d675db1de1" />


3. Gabriel Cavalcante, de 43 anos, trabalha como analista de dados na empresa Mind Plus, onde semanalmente necessita criar datasets para outras empresas, cujo foco principal das mesmas é o desenvolvimento de jogos. Essas empresas necessitam de datasets personalizados que consigam envolver o jogo e o jogador. Gabriel precisa de uma ferramenta que facilite a captação da emoção de pessoas enquanto jogam, dessa maneira consegue saber que tipos de jogos causariam, mais conforto, raiva e medo, a fim de auxiliar na criação de uma experiência customizada.<br>
   <img width="256" height="256" alt="image" src="https://github.com/user-attachments/assets/8004ef7f-e31e-4866-a6d5-e321e374af5e" />

#### Persona secundária
1. Lora Barros, de 21 anos, estudante de ciências da computação tem como principal hobby jogar videogame. Costuma jogar jogos únicos com mecânicas diferentes e impactantes. Como está de férias, busca jogar um novo jogo, algo que possa ser controlado e desenvolvido a partir de identificações de rosto, emoções. Para ela, esse seria o ápice da tecnologia nos jogos eletrônicos.
2. Alberto Bezerra, de 24 anos, estudante de ciências da computação está participando de uma iniciação científica que envolve o desenvolvimento de aplicações com Deep Learning, mas o projeto acabou se estagnando pois o dataset que ele utiliza está desbalanceado. Como está no terceiro semestre da faculdade, ele não compreende completamente o conceito de data augmentation, então ele busca por métodos de criação de datasets usando o próprio rosto para suprir os dados que estão em falta no dataset original.

### Mapa de empatia

![Mapa de empatia](empatia.png)

<!--
- Determine o mapa de empatia[^1] de pelo menos uma persona primária e uma sercundária.
  - O que o usuário vê: aqui estamos falando do ambiente visual em que o usuário se encontra. Ou seja, o que ele efetivamente enxerga, as pessoas e objetos que estão ao seu redor. Isso ajuda a entender o contexto em que o usuário está inserido e as influências visuais que está recebendo.
  - O que o usuário ouve: neste quadrante, buscamos entender o que o usuário está ouvindo, os sons que o cercam e como eles influenciam suas ações.
  - O que o usuário diz e faz: aqui consideramos ações e comportamentos que o usuário apresenta durante sua interação com serviço ou poduto.
  - O que o usuário pensa e sente: neste quadrante, buscamos entender os pensamentos, sentimentos, emoções e percepções que o usuário tem em relação ao serviço ou poduto. Quais expectativas o usuário cria sobre o serviço ou poduto?
  Que tipo de serviço ou poduto mais agrada essa persona?
  - Dores: quando falamos sobre dores do usuário, estamos fazendo referência a quaisquer obstáculos, necessidades ou frustrações que o usuário possa experimentar ao tentar realizar uma tarefa ou alcançar um objetivo. Isso inclui, por exemplo, problemas de usabilidade, dificuldades de acesso ou outros desafios que podem afetar a experiência do usuário.
  - Ganhos: nesse caso estamos falando de quaisquer benefícios ou recompensas que o usuário possa experimentar ao utilizar o serviço ou poduto. Isso pode incluir economia de tempo ou facilidade de uso, por exemplo. Que desejos do usuário o serviço ou poduto satisfaz?
-->

#### Persona primária: Gabriel Calvacante, 43 anos
- O que o usuário vê: Família bem estruturada; Amigos de classe média-alta, Chefe que demanda desempenho por parte dos funcionários.
- O que o usuário ouve: Precisa passar mais tempo com a família e menos no trabalho; Assiste a canais do YouTube sobre a área de dados.
- O que o usuário diz e faz: Gosta de ler livros que abordam psicologia, desde suspense até estudos científicos; Frquenta lugares de luxo moderado, de forma que a família esteja confortável sem precisar gastar mais do que deve.
- O que o usuário pensa e sente: Preciso estudar para crescer na minha área; Acredito que jogos customizados podem vender mais do que jogos comuns; Compreendo que quanto mais dados a empresa tiver, mais fácil será o trabalho dos funcionários.
- Dores: Sente que passa menos tempo com a família por conta do tempo gasto dentro de seu trabalho; Sente que não atende as demandas de seu chefe, e se conseguisse um facilitador poderia alavancar seus resultados.
- Ganhos: Redução de tempo de trabalho, tanto por parte da pesquisa de um dataset coerente, quanto por parte da criação de um novo; Facilidade ao encontrar novos dados.

#### Persona primária: Valter Alter, 58 anos
- O que o usuário vê: Seus seguidores do Youtube apoiando suas ideias, família bem unida, cenário de game development mais desenvolvido.
- O que o usuário ouve: As ferramentas para realizar seu trabalho estão avançando rapidamente, família apoia muito seu trabalho.
- O que o usuário diz e faz: Gosta de jogar com seus filhos, gosta de produzir jogos e distribuir a seus seguidores. Diz que ama o que faz.
- O que o usuário pensa e sente: Sente que precisa inovar em seu conteúdo e que precisa de ferramentas novas para isso.
- Dores: Sente que ainda não fez um jogo de sucesso e que gostasse. Gostaria de atrair mais pessoas para seu nicho de games.
- Ganhos: Redução do tempo de trabalho e uma produção mais rápida de conteúdo.

#### Persona primária: Thiago Alberto Mendes, 35 anos
- O que o usuário vê: Sua contribuição em desenvolvimento de jogos interessantes, 
- O que o usuário ouve: Que fez bons jogos, que precisa renovar o estado dos games.
- O que o usuário diz e faz: Diz que quer fazer um jogo que seja inovador e muito grande, que precisa criar uma família.
- O que o usuário pensa e sente: Se sente sozinho e estagnado profissionalmente.
- Dores: Não ter feito um jogo muito conhecido, não ter uma família.
- Ganhos: Muita experiência no desenvolvimento de jogos e manejamento de equipes.

#### Persona secundária: Lora Barros, 21 anos
- O que o usuário vê: Amigos bem fiéis, família que apoia suas decisões. Bem disciplinada e sempre tira boas notas.
- O que o usuário ouve: Ouve que deve arrumar logo um emprego, sobre anúncio de novos jogos e sobre evoluções tecnológicas.
- O que o usuário diz e faz: Gosta de jogar videogame e estuda bastante, principalmente programação e tecnologias. Não gosta muito de sair, prefere passar o tempo em casa, seja nos estudos ou nos jogos. Gosta de ler livros técnicos.
- O que o usuário pensa e sente: Queria um jogo revolucionário, com que possa jogar e se divertir com os amigos. Sente que precisa logo arranjar um estágio, pois todos os seus amigos estão começando em um.
- Dores: Precisa logo de um emprego e quer começar a estudar o desenvolvimento de jogos e datasets.
- Ganhos: Ser bem sucedida, ter um foco profissional na área de games e ter vários amigos.
  
## Contexto de uso

### Descreva o ambiente em que o serviço ou produto deve ser utilizado:
* Gabriel Cavalcante:
Como Gabriel precisa capturar expressões faciais com precisão para gerar datasets confiáveis, o ambiente ideal de uso do produto deve ser controlado. Ele normalmente utiliza salas bem iluminadas e silenciosas em sua empresa, com webcams de pelo menos 720p e fundos neutros, garantindo que os dados não sejam comprometidos por interferências visuais. Como profissional da área, Gabriel também se certifica de que os participantes não utilizem acessórios que obstruam o rosto, como bonés, máscaras ou óculos escuros, para manter a qalidade do reconhecimento facial.
### Qual/quais o(s) contexto(s) sociais, econômicos e culturais existentes neste ambiente?
* Gabriel Cavalcante:
Gabriel atua em um contexto profissional, dentro de uma empresa de tecnologia com foco em dados e jogos digitais. Ele tem acesso a recursos computacionais avançados e trabalha com colaboradores familiarizados com tecnologia. Culturalmente, ele está inserido em um ambiente onde inovação, usabilidade e personalização são valorizados, pois os datasets gerados serão usados para melhorar a experiência de jogadores de diferentes perfis. Economicamente, sua empresa investe em ferramentas que otimizem o tempo e aumentem a qualidade dos dados, o que torna fundamental que o produto seja eficiente e compatível com sistemas mais robustos.
### Quais informações sobre o ambiente, o serviço ou poduto deve guardar antes de iniciar a interação?
* Gabriel Cavalcante:
Antes de iniciar a coleta de dados, Gabriel precisa configurar o ambiente e o sistema de forma adequada. Isso inclui garantir que os participantes estejam posicionados corretamente, com boa iluminação e sem obstruções no rosto. O sistema deve registrar informações básicas sobre o cenário de uso (como iluminação, tipo de câmera, resolução e características do ambiente), bem como armazenar fotos iniciais dos usuários para o treinamento do modelo de reconhecimento facial. Esses dados são fundamentais para que o processo ocorra sem erros e para garantir consistência nos datasets gerados.
### O que normalmente deve estar acontecendo com o ambiente quando o usuário interagir com o serviço ou poduto?
* Gabriel Cavalcante:
Durante a coleta das emoções, Gabriel garante que o ambiente permaneça estável: a iluminação constante, pouco ruído e o mínimo de movimento externo. Isso evita interferências no reconhecimento facial e garante que as emoções captadas estejam realmente relacionadas às interações do jogador com o jogo. O foco é criar uma experiência imersiva para o participante, enquanto Gabriel observa, coleta e analisa os dados gerados em tempo real ou após a sessão.

## Jornada do usuário
<!--
- Criar uma narrativa para o o seu serviço ou poduto com o usuário.
- Determine o que o usuário realiza desde a primeira até o última interação com o serviço ou poduto.
  - Descreva o que acontece ou pode acontecer passo a passo
  - Como a tarefa começa? Como a tarefa se desenvolve? Como a tarefa termina?
-->

Jorge Mateus trabalha na área de dados de uma empresa de desenvolvimento de jogos e decidiu utilizar seu próprio rosto para criar um dataset que será usado em seu trabalho.
Ele acessa o site do produto, realiza o cadastro, e em seguida cria um nome e uma descrição para o seu dataset. Depois, liga a webcam e define a quantidade de frames que deseja capturar. Durante esse processo, os frames da webcam são salvos automaticamente em uma pasta separada.
Assim que a quantidade de frames definida é atingida, Jorge inicia o treinamento do dataset clicando em um botão. Em seguida, ele aciona outro botão para começar a captura de emoções e, ao mesmo tempo, inicia sua jogatina. Durante esse período, as imagens capturadas para análise emocional são armazenadas diretamente no dataset criado.
<!--
## Análise de concorrência

- Pesquise serviços ou podutos existentes atualmente que possam realizar o objetivo deste projeto.
- Selecione pelo menos 3 serviços ou podutos diferentes.
- Em relação aos concorrentes, respondam as seguintes perguntas?
  - Existe plataforma similar que atende o mesmo mercado e funcionalidades? Se sim: Quais os pontos positivos? Quais os pontos negativos?
  - Existe plataforma diferente quanto ao serviço, mas que atenda esse mercado? Se sim: Quais os pontos positivos? Quais os pontos negativos?
 -->

## Qualidade de Uso em IHC
* A usabilidade é um dos pilares fundamentais do projeto e deve ser muito bem projetada, uma vez que qualquer um que possuir a licença poderá utilizar a plataforma.
Desta maneira, ela será intuitiva, com ícones, imagens e explicações das funcionalidades, deve ser, também, fácil de ser utilizada e deve ter um grau de aprendizagem rápido e permanente no usuário, para que não precise se utilizar de tutoriais a cada uso.
Juntamente a isso, será feito um fluxo lógico de navegação, direcionando o usuário para a próxima etapa do processo de forma fluida e focada.
Por ser um aplicativo local, a segurança será o menor dos problemas, uma vez que as imagens tiradas e os dados gerados estarão presentes no computador do usuário. <br>
* A experiência do usuário será baseada em suas emoções e expressões faciais, desta maneira, para atribuir sensações de prazer, diversão e profissionalismo, o aplicativo deverá possuir animações fluidas. interfaces modernas, feedback ao usuário e design inteligente.
Tais fatores contribuirão para a satisfação e credibilidade do usuário com o projeto. <br>
* Para acessibilidade, teremos menus simples e explicações compreensíveis para o entendimento de todo público alvo, algo a ser implementado seria uma resposta auditiva ao clicar botões, para uma maior abrangência de público.
O design inteligente e o fluxo lógico para o desenvolvimento da atividade torna o aplicativo fácil de ser utilizado e intuitivo na hora do uso. <br>
* O sistema terá boa comunicabilidade, uma vez que cada passo apresentará explicações de como usar e o que está sendo feito, com as imagens, com o usuário, com o sistgema. Serão utilizados icones, imagens, para facilitar a comunicação e interação com o usuário, a partir da aplicação.

## Ambiente e contexto

### Thiago Alberto Mendes:
#### Perguntas:

### Valter Alter  
#### Perguntas de refinamento: <br>
1 - Quem pode/deve cadastrar os dados de gameplay e expressões faciais no sistema? <br>
2 - Quando são cadastradas as sessões de jogo para geração de datasets? <br>
3 - Quem fornece os dados de gameplay e das expressões? <br>
4 - Quais dados de gameplay e faciais devem ser cadastrados? <br>
5 - Quantas sessões de captura são realizadas em cada período? <br>
6 - Quem pode contribuir com gravações de gameplay e expressões? <br>
7 - Que dados são necessários para cadastrar um seguidor como participante externo? <br>
8 - Como são obtidos os vídeos enviados por seguidores? <br>
9 - De quem depende a conclusão do cadastro de um dataset? <br>
10 - De que informações Valter e seus seguidores precisam para confirmar que o dataset foi gerado corretamente? <br>
11 - Como um participante confirma que seu material foi aceito? <br>
12 - Em que pontos a interação de Valter com a aplicação pode ser mais eficiente? <br>
13 - Como Valter entra em contato com seus seguidores para organizar o envio dos dados? <br>
14 - Quem precisa ser notificado quando um dataset é concluído? <br>

#### Atores:
Valter Alter, 58 anos, criador de conteúdo para jogos digitais no canal ClickGamesBR (1,3 milhão de inscritos no YouTube). Seus seguidores frequentemente pedem novidades, incluindo jogos que respondam às emoções dos jogadores.

#### Narrativa:
Valter Alter, 58 anos, é criador do canal **ClickGamesBR**. Ele utiliza seu **PC gamer e webcam HD em seu estúdio** [Q1]. **Os atores principais são Valter e seus seguidores**, que podem enviar gravações de gameplay [Q2]. **Seu objetivo é gerar datasets de emoções para criar jogos interativos** e, como meta secundária, inovar no canal [Q3].

Primeiro, **testa a ferramenta em suas próprias lives** e depois planeja campanhas para receber vídeos dos seguidores [Q4]. Durante o uso, conecta a webcam e deixa a aplicação registrar automaticamente suas expressões [Q5]. A iluminação e qualidade da câmera podem interferir nos resultados [Q6]. Valter avalia os datasets verificando se as expressões correspondem às situações de jogo [Q7].

Ele escolhe a ferramenta por economizar tempo em relação à rotulagem manual [Q8]. Já tem experiência com gravações, mas não com análise automática de emoções [Q9]. **Pretende usar a aplicação regularmente em transmissões e gravações** [Q10]. Entre as barreiras estão iluminação inadequada e custos de equipamento [Q11]. Ele conta com softwares de edição e plataformas de streaming como apoio [Q12]. O retorno é a criação rápida de datasets rotulados [Q13]. A longo prazo, espera consolidar sua imagem como criador inovador [Q14].

### Gabriel Cavalcante:
#### Perguntas de refinamento:
1. Quem pode/deve cadastrar os dados de sessões de jogo e emoções no sistema?<br>
2. Quando são cadastradas as sessões de teste para geração dos datasets?<br>
3. Quem fornece os dados necessários (jogadores, equipe de coleta, clientes)?<br>
4. Quais informações de gameplay e expressões devem ser cadastradas?<br>
5. Quantas sessões de coleta geralmente são realizadas por projeto?<br>
6. Quem pode participar como jogador/usuário nas sessões de captura?<br>
7. Que dados são necessários para cadastrar um jogador externo no sistema?<br>
8. Como são obtidos os dados dos jogadores (capturas automáticas, formulários, vídeos)?<br>
9. De quem depende a conclusão da criação de um dataset (Gabriel, equipe, ferramenta)?<br>
10. De que informações Gabriel e a equipe precisam para validar os datasets criados?<br>
11. Como um cliente confirma que o dataset atende suas necessidades?<br>
12. Em que pontos a interação de Gabriel com a ferramenta pode ser mais eficiente?<br>
13. Como Gabriel entra em contato com jogadores ou clientes envolvidos no processo?<br>
14. Quem precisa ser notificado quando um dataset é concluído (Gabriel, equipe, empresa cliente)?<br>

#### Atores:
Gabriel Cavalcante, 43 anos, trabalha na empresa MindPlus. Semanalmente precisa criar datasets para outras empresas, cujo foco é o desenvolvimento de jogos.

### Narrativa:
Gabriel Cavalcante, 43 anos, **trabalha na MindPlus**, em um **escritório com computadores potentes e webcams** [Q1]. **O ator principal é Gabriel**; **secundários são jogadores** que participam dos testes e os clientes que recebem os datasets [Q2]. **Seu objetivo é produzir datasets personalizados de emoções**, reduzindo tempo de coleta manual [Q3].

Ele organiza sessões, ajusta ambiente e executa a ferramenta para capturar expressões durante o gameplay [Q4–Q5]. Fatores como ruído ou iluminação podem interferir [Q6]. Gabriel avalia os resultados comparando emoções detectadas com eventos do jogo [Q7].

O que o leva a usar a aplicação é a **necessidade de gerar datasets sob demanda de forma mais rápida** [Q8]. Ele tem experiência com dados, mas o reconhecimento facial automatizado é novidade [Q9]. O uso é frequente, semanal ou diário [Q10]. As barreiras envolvem limitações técnicas e prazos apertados [Q11]. Como apoio, usa bibliotecas de IA e softwares estatísticos [Q12]. O retorno é a entrega de datasets prontos e consistentes [Q13]. A longo prazo, espera fortalecer sua carreira e consolidar a MindPlus no mercado [Q14].
<br>


## Coleta de dados (A FAZER)

## Modelo de tarefas (A FAZER)

## Design (A FAZER)

- Pense nas características de Affordances do seu serviço ou poduto. 
    - Que tipo de acessibilidades devem ser consideradas dentro do seu projeto?
- Discuta o papel das expectativas do usuário no projeto deste serviço ou poduto. Qual a importância e pontos a serem considerados se você quiser vender esse serviço ou poduto?

### Prototipação em baixo nível (papel) (A FAZER)
#### Avaliação heurística

### Prtotipação em médio nível (Figma) (A FAZER)
#### Avaliação heurística

### Prtotipação em alto nível (React) (A FAZER)
#### Avaliação heurística

[^1]: Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>

<!-- TODOs:
- Add exemplos
 -->
