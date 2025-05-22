# Análise de Fala e Linguagem Natural

Neste laboratório, exploraremos e praticaremos o uso das ferramentas **Azure Speech Studio** e **Language Studio**, com foco na análise de fala e linguagem natural. O objetivo é aprofundar nosso entendimento e desenvolver habilidades práticas na implementação de soluções baseadas em inteligência artificial voltadas para voz e linguagem. Durante as atividades, teremos a oportunidade de conhecer e aplicar as capacidades avançadas dessas tecnologias da Microsoft Azure, ampliando nossa compreensão sobre suas possibilidades e aplicações no mundo real. 

Como entregável, será elaborado um repositório organizado contendo anotações, insights e registros das práticas realizadas, servindo como material de apoio para estudos contínuos e futuras implementações.

## Objetivos de Aprendizagem

- Aplicar os conceitos aprendidos em um ambiente prático.
- Documentar processos técnicos de forma clara e estruturada.
- Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica.

### Procedimentos

Inicialmente, acessei o **Speech Studio (Estúdio de Fala)** com a minha conta no Azure:

[https://speech.microsoft.com/portal](https://speech.microsoft.com/portal)

<img src="images/conectei_me.png" alt="conectei-me" width="500"/>

Criei o novo recurso com o nome `iafalatexto`:

<img src="images/criar_novo_recurso2.png" alt="criar_novo_recurso2" width="500"/>

Recurso criado com sucesso:

<img src="images/criado_sucesso.png" alt="criado_sucesso" width="500"/>

Em seguida, selecionei a opção **Conversão de fala em texto em tempo real** e submeti o seguinte arquivo de áudio:

[Ouvir o áudio](audio/Audio_Valeria_Baptista.mp3)

Segue o resultado apresentado:

<img src="images/resultado_fala_texto1.png" alt="resultado_fala_texto1" width="500"/>

O texto gerado foi o seguinte:

> "Nesse ponto, a gente também pode inserir perguntas e respostas, né? Conseguimos personalizar e, claro, conseguir ter também um bate-papo integrado dentro dessa plataforma. E isso é bem interessante, porque quando a gente faz o acesso, né, No No estúdio de linguagem, né, lenga de estúdio, a gente consegue fazer uma série de extração de informações, então você pode inserindo. Você pode ver modelos também do beach hub ou você pode inserir ali alguns textos para ter essa análise dele. Isso é bem bacana e ao final dessa aula a gente também vai fazer um laboratório para explorar um pouco mais sobre as funcionalidades dessa aplicação assim."

O resultado foi bom, com apenas duas falhas: 
- **"Language Studio"** transcrito como **"lenga de estúdio"**
- **"GitHub"** como **"beach hub"**

Fiz mais uma tentativa e a transcrição falhou nos mesmos dois pontos, só que dessa vez **"GitHub"** saiu como **"Pit hub"**.

<img src="images/resultado_fala_texto2.png" alt="resultado_fala_texto2" width="500"/>

Acredito que essas falhas se devem ao setup da ferramenta para a linguagem original do arquivo. Por ser Português (BR), creio que palavras faladas em inglês (ou outro idioma) a IA não reconhece com tanta precisão.

**Não era sugestão do laboratório**, mas decidi testar outro recurso oferecido pelo Speech Studio: a avaliação da minha pronúncia em inglês. O resultado foi muito bom:

<img src="images/avaliação_pronuncia.png" alt="avaliação_pronuncia" width="500"/>

O que me chamou a atenção foi a **pontuação de prosódia**. Preciso melhorar a minha prosódia — colocar mais ritmo e melodia na fala 😄.

### Language Studio

A próxima atividade foi com o uso dos recursos do **Language Studio**:

[https://language.cognitive.azure.com/](https://language.cognitive.azure.com/)

O objetivo foi analisar sentimentos de comentários sobre serviços.

No portal Azure, usando outro diretório, entrei no **Language service**:

<img src="images/criar_language_service.png" alt="criar_language_service" width="500"/>

<img src="images/criar_language_service.png" alt="criar_language_service" width="500"/>

<img src="images/criar_language_service2.png" alt="criar_language_service2" width="500"/>

E criei o recurso `idiomasensing`:

<img src="images/select.png" alt="select" width="500"/>

<img src="images/deployment_complete.png" alt="deployment_complete" width="500"/>

Uma vez criado o recurso no Portal Azure, no Portal **Language Studio** utilizei a funcionalidade **Analyze sentiment and mine opinions**:

<img src="images/classify_text.png" alt="classify_text" width="500"/>

Escolhi três comentários fictícios para análise:
- Dois em inglês (um positivo e outro negativo)
- Um em português (meio positivo, meio negativo)

Resultados:

Texto 1 , Inglês, comentário positivo:

<img src="images/text1_to_tryout.png" alt="text1_to_tryout" width="500"/>

<img src="images/text1_result1.png" alt="text1_result1" width="500"/>
<img src="images/text1_result2.png" alt="text1_result2" width="500"/>
<img src="images/text1_result3.png" alt="text1_result3" width="500"/>

Texto 2, Inglês, comentário negativo:

<img src="images/text2_to_tryout.png" alt="text2_to_tryout" width="500"/>

<img src="images/text2_result1.png" alt="text2_result1" width="500"/>
<img src="images/text2_result2.png" alt="text2_result2" width="500"/>
<img src="images/text2_result3.png" alt="text2_result3" width="500"/>

Texto 3, Português(BR), comentário meio positivo e meio negativo:

<img src="images/text3_to_tryout.png" alt="text3_to_tryout" width="500"/>

<img src="images/text3_result1.png" alt="text3_result1" width="500"/>
<img src="images/text3_result2.png" alt="text3_result2" width="500"/>
<img src="images/text3_result3.png" alt="text3_result3" width="500"/>
<img src="images/text3_result4.png" alt="text3_result4" width="500"/>

## Conclusão

O laboratório serviu como primeiro contato com ferramentas e recursos de IA para tratamento e análise de fala e linguagem natural. Os resultados foram muito bons, especialmente na **avaliação de sentimentos e opiniões de usuários de serviços diversos**. 

Quando se necessita avaliar milhares de comentários, a ferramenta se mostra indispensável e de grande valor para **Analistas de Mídias Sociais** e profissionais de Customer Experience.
