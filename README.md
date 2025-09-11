# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](http://lattes.cnpq.br/6747210702910392) e Prof. Dr. [Plino Thomaz Aquino Junior](http://lattes.cnpq.br/6186413528999908).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Guia Visual: SIstema de Detecção de Objetos para Deficientes Visuais** sob orientação do Professor **Isaac Jesus da Silva** e desenvolvido pelos seguintes alunos:

- Rômulo Carneiro de Oliveira Canavesso - RA: 24.122.093-8
- Lucas Antunes Sampaio - RA: 24.122.056-5

## Resumo

Este trabalho apresenta o desenvolvimento de um protótipo assistivo para deficientes visuais, concebido como um acessório acoplável a qualquer óculos, com o objetivo de ampliar a autonomia e a segurança na locomoção. O sistema utiliza visão computacional e aprendizado de máquina, empregando o modelo YOLOv8 para detecção de pessoas e veículos, aliado ao Tesseract OCR para reconhecimento de textos em placas e sinalizações. A implementação será realizada em uma Raspberry Pi 5, integrada a câmeras, fone de ouvido e estrutura confeccionada em impressão 3D, assegurando portabilidade e ergonomia. As informações captadas são processadas em tempo real e transmitidas ao usuário por meio de feedback sonoro, de forma clara e objetiva.

## Introdução

 <!--
 
- Apresente o propósito do produto ou serviço e quais são os principais benefícios que ele oferece aos usuários.
- Identifique os problemas ou necessidades que o produto ou serviço resolve ou satisfaz.
- Liste as características e funcionalidades do seu produto ou serviço de forma detalhada.
- Liste as tecnologias e ferramentas computacionais que pretendem usar neste projeto (TCC).
- Apresente o contexto de uso dessa aplicação. (“Usuários, tarefas, equipamentos (hardware, software e materiais) e o ambiente físico e social no qual um produto é usado.”)

-->

#### Propósito e Benefícios
O projeto tem como propósito desenvolver um **sistema assistivo para pessoas com deficiência visual**, em formato de **acessório acoplável a qualquer óculos**.  
Os principais benefícios oferecidos aos usuários são:  
- **Maior autonomia** na locomoção em ambientes urbanos.  
- **Segurança** ao identificar elementos críticos do cenário, como pessoas, veículos e placas.  
- **Acesso à informação** por meio de leitura de textos em placas e sinalizações.  
- **Praticidade e ergonomia**, já que o protótipo é portátil e de fácil uso.  

#### Problemas e Necessidades Atendidas
O produto busca resolver desafios enfrentados por pessoas com deficiência visual, tais como:  
- Dificuldade de se locomover com independência em ruas e vias públicas.  
- Riscos associados a obstáculos como veículos, sinalizações e faixas de pedestres.  
- Necessidade de compreender informações textuais presentes em placas e orientações.  
- Falta de soluções acessíveis, portáteis e de baixo custo voltadas para mobilidade urbana.  

#### Características e Funcionalidades
O sistema oferece as seguintes funcionalidades principais:  
- **Detecção em tempo real** de pessoas e veículos utilizando visão computacional.  
- **Reconhecimento de textos** em placas e sinalizações por meio de OCR.  
- **Feedback sonoro imediato**, transmitido ao usuário via fone de ouvido.  
- **Interface simples de ativação**, projetada como botão físico acoplado ao óculos.  
- **Portabilidade**, garantindo ergonomia e conforto ao usuário durante a utilização.  

#### Tecnologias e Ferramentas Utilizadas
O projeto faz uso das seguintes tecnologias e ferramentas computacionais:  
- **YOLOv8 (Ultralytics)** → Detecção de pessoas e veículos.  
- **Tesseract OCR** → Leitura e reconhecimento de textos em placas.  
- **gTTS (Google Text-to-Speech)** → Geração de feedback sonoro.  
- **OpenCV** → Processamento de imagens e suporte à visão computacional.  
- **Datasets públicos (COCO, Open Traffic Lights, entre outros)** para treinamento e testes.  
- **Plataforma Raspberry Pi 5** → Execução embarcada do sistema.  
- **Estrutura em impressão 3D** para fixação dos componentes ao óculos.
- **Webcam** para a captura das imagens em tempo real.
- **Botão** para interação com o protótipo.

#### Contexto de Uso
- **Usuários:** Pessoas com deficiência visual que necessitam de auxílio em ambientes urbanos.  
- **Tarefas:** Locomoção segura, identificação de obstáculos, compreensão de placas e sinalizações.  
- **Equipamentos (hardware):** Raspberry Pi 5, duas webcams, fone de ouvido, botão físico, suporte em óculos confeccionado em 3D.  
- **Equipamentos (software):** YOLOv8, Tesseract OCR, OpenCV, gTTS, bibliotecas auxiliares em Python.  
- **Ambiente físico e social:** Utilização em espaços urbanos (ruas, avenidas, calçadas e áreas públicas), promovendo **inclusão social** e **acessibilidade**.  

## Publico Alvo

<!-- 
- Determine qual o grupo específico de pessoas ou organizações para as quais este produto ou serviço é direcionado.
- Descreva as caracteristicas demográficas, comportamentais, psicográficas ou geográficas deste público alvo que o torna mais propenso a se interessar pelo que está sendo oferecido neste projeto ou serviço.

-->

O público-alvo deste trabalho são pessoas com deficiência visual, que enfrentam desafios relacionados à mobilidade e à autonomia em ambientes urbanos. Esse grupo inclui indivíduos com baixa visão e aqueles com cegueira total, que necessitam de suporte tecnológico para identificar obstáculos, compreender sinalizações e se locomover com maior segurança. Além dos usuários finais, o sistema também pode ser de interesse para instituições de apoio à inclusão social, organizações voltadas à acessibilidade, e pesquisadores da área de tecnologias assistivas, que buscam soluções portáteis, acessíveis e de fácil utilização no cotidiano.

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

#### 1. Principais concorrentes

- **OrCam MyEye**: módulo compacto acoplado aos óculos; IA para leitura de textos e reconhecimento de rostos/objetos; áudio descritivo em tempo real; não mede distância.

- **Envision Glasses**: baseado em Google Glass 2; câmera com OCR; reconhecimento de pessoas/objetos; foco em leitura e orientação; integra apps móveis e nuvem.

- **biped.ai**: dispositivo tipo colar (vestível no pescoço); visão estéreo 3D; detecção de obstáculos e cálculo de distância; feedback sonoro; áudio não disponível em português.

#### 2. Informações dos concorrentes
- **OrCam MyEye**:
  - **Forma**: módulo que se acopla aos óculos.
  - **Funções**: leitura de textos impressos; reconhecimento de rostos/objetos; áudio em tempo real.
  - **Limitação**: não mede distâncias; referência consolidada em acessibilidade.

- **Envision Glasses**:
  - **Forma**: óculos inteligentes (Google Glass 2).
  - **Funções**: OCR embutido; reconhecimento de pessoas/objetos; leitura/tradução; integração com apps/nuvem.
  - **Posicionamento**: ideal para leitura e orientação contextual.

- **biped.ai**:
  - **Forma**: vestível no pescoço (colar).
  - **Funções**: visão estéreo 3D; detecção de buracos, postes, carros; distância em tempo real; feedback por fones.
  - **Limitação**: sem áudio em português (impacto direto na adoção no Brasil).

#### 3. Características e funcionalidades dos concorrentes

| Critério                  | OrCam MyEye               | Envision Glasses                 | biped.ai                       |
| ------------------------- | ------------------------- | -------------------------------- | ------------------------------ |
| **Formato**               | Módulo acoplado ao óculos | Óculos inteligentes (Glass 2)    | Colar/arnês no pescoço         |
| **Leitura (OCR)**         | Forte (texto impresso)    | Forte (OCR + tradução)           | Secundária                     |
| **Reconhecimento**        | Rostos/objetos            | Pessoas/objetos/cenas            | Obstáculos em movimento        |
| **Navegação / Distância** | —                         | Limitada (orientação contextual) | **Forte** (3D + distância)     |
| **Feedback**              | Áudio descritivo          | Áudio descritivo                 | Áudio (espacial/orientativo)   |
| **Integrações**           | —                         | **Apps + Nuvem**                 | —                              |
| **Idiomas**               | Amplo                     | Amplo                            | **Sem PT-BR**                  |

#### 4. Avaliação de experiência do usuário (UX)
- **OrCam MyEye**:
  - **Prós**: muito discreto; preserva o óculos do usuário; fluxo rápido para leitura e identificação pontual.
  - **Contras**: sem noção de profundidade/distância; experiência focada em leitura/identificação, não em navegação.

- **Envision Glasses**:
  - **Prós**: experiência “tudo-em-um” de leitura e descrição; integra com apps/nuvem; boa curva de aprendizado para tarefas diárias.
  - **Contras**: dependência de hardware dedicado; pode ser menos discreto; experiência de navegação não é o foco.

- **biped.ai**:
  - **Prós**: UX centrada em mobilidade ativa e prevenção de colisões; áudio orientativo com distância em tempo real.
  - **Contras**: formato colar pode incomodar alguns usuários; ausência de PT-BR diminui acessibilidade local.
  
## 5) Preços e Modelos de Negócio
- **OrCam MyEye:** dispositivo premium, custo elevado; modelo de aquisição única do hardware.  
- **Envision Glasses:** disponível em diferentes edições (Read, Home, Pro), com pacotes de recursos distintos; adota também modelo de **atualizações pagas** para novos recursos.  
- **biped.ai:** dispositivo dedicado em formato de colar; política de preços menos transparente, com tendência a planos de software e atualizações contínuas.  

## 6) Satisfação e Opiniões dos Usuários
- **OrCam MyEye:** feedback positivo em leitura de textos e reconhecimento de rostos; críticas ao preço elevado e à ausência de recursos de navegação espacial.  
- **Envision Glasses:** opiniões majoritariamente positivas quanto à leitura/tradução de textos e integração com aplicativos móveis; limitações apontadas no custo e na autonomia da bateria.  
- **biped.ai:** considerado promissor para navegação urbana; usuários elogiam a detecção de obstáculos, mas destacam a ausência de suporte em **português** como limitação relevante.  

## 7) Padrões e Tendências do Mercado
- **Integração IA + vestíveis**: foco em unificar leitura, reconhecimento e navegação em um só produto.  
- **Feedback sonoro contextual**: mensagens rápidas e direcionais (ex.: avisos de obstáculos).  
- **Processamento on-device**: redução da dependência de nuvem, garantindo privacidade e baixa latência.  
- **Customização local**: idiomas e sinalizações específicas por país (no Brasil, PT-BR e elementos do trânsito local são diferenciais).  
- **Modelos de atualização contínua**: tendência crescente de cobrar por upgrades de software além do hardware inicial.  

## 8) Relatório e Sumário dos Resultados
- O mercado atual se divide entre **leitura/descrição** (OrCam, Envision) e **navegação ativa** (biped.ai).  
- Há uma lacuna para um dispositivo de **baixo custo**, **acoplável a qualquer óculos**, com suporte em **português**.  
- O protótipo desenvolvido neste TCC se posiciona para preencher essa lacuna ao oferecer:  
  - **OCR em PT-BR**,  
  - **Detecção urbana de pessoas e veículos**,  
  - **Alertas sonoros em tempo real**,  
  - **Custo reduzido** por meio de webcams e estrutura em impressão 3D.  

## 9) Pontos Positivos e Recomendações
**Inspirações dos concorrentes:**  
- **OrCam MyEye:** formato acoplável discreto.  
- **Envision Glasses:** fluxo de OCR fluido e integração com aplicativos.  
- **biped.ai:** alertas direcionais e cálculo de distância em tempo real.  

**Recomendações para evolução do protótipo:**  
1. **Aprimorar navegação básica** com uso de visão estéreo (duas webcams).  
2. **Garantir baixo custo** explorando componentes acessíveis e impressão 3D.  
3. **Mensagens sonoras em português**, claras, curtas e com baixa latência.  
4. **Modos de operação**: (a) Leitura/OCR, (b) Detecção urbana, (c) Navegação básica.  
5. **Privacidade by design**: processamento local como padrão.  
6. **Testes práticos com usuários reais** para validar UX e reduzir falsos alertas.  
7. **Planejamento de roadmap** para expandir classes detectadas (faixas de pedestre, placas brasileiras, semáforos).

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
