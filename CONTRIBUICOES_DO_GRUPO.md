# Contribuições do grupo para “Desenhe o som”

Este arquivo registra **propostas de integrantes do Grupo 6**, do seminário “Tecnologias da Informação (TICs) no ensino de Física” da disciplina *Elementos e Estratégia para o Ensino de Física e Ciências*. É uma **síntese atribuída**, não uma transcrição integral do WhatsApp nem uma descrição de recursos já concluídos.

**Fontes deste registro:** conversa do grupo compartilhada por Jhuann em 20/11/2026 e o PDF de duas páginas **“Ensino de física”**, enviado por Aymee no grupo. [Cópia do PDF enviado](proposta-desenho-sonoro-enviada-por-aymee.pdf). A cópia mantém o conteúdo original; o nome do arquivo foi alterado apenas para facilitar sua identificação. As capturas da conversa não foram publicadas aqui.

## Ideias apresentadas pelas integrantes

### Aymee

- Propôs uma interface em que a pessoa desenha e uma partícula em movimento produz sons ao percorrer ou encontrar pontos da figura. Sua intenção é usar a experiência para conversar sobre ondulatória e música.
- Considerou figuras simples e o gráfico de uma função como alternativas de implementação. Ofereceu-se para escrever um texto curto que explique ondas e seus gráficos na página.
- Compartilhou o PDF “Ensino de física”, no qual desenvolve uma visão mais ampla da proposta. O documento sugere converter características do desenho em parâmetros sonoros: posição vertical em frequência da nota; posição horizontal em tempo ou posição estéreo; movimento e tamanho da partícula em duração ou volume; espessura ou cor do traço em timbre.
- No PDF, propôs uma expressão para uma contribuição sonora que depende da distância entre partícula e ponto do desenho, além de Canvas 2D ou p5.js para a parte visual e Web Audio API ou p5.sound para o som. Indicou toque e mouse como entradas, e webcam, efeitos visuais, várias camadas sonoras e gravação como possíveis expansões.
- Apoiou a discussão sobre ampliar as formas de acesso à atividade para pessoas com deficiência.

### Carol

- Sugeriu começar com desenhos simples, como **círculo** e **estrela**, reconhecendo que essas figuras podem exigir mais implementação do que o gráfico de uma função.
- Propôs explorar a passagem de uma representação visual para uma sonora como forma lúdica de investigar funções, formas e comportamentos. Sua reflexão abre a pergunta: **que escolhas de modelagem transformam uma figura em uma sequência de sons?**
- Levantou a possibilidade de o recurso criar uma via adicional de acesso para pessoas cegas. Essa é uma hipótese de projeto, ainda sem validação com estudantes ou tecnologias assistivas.

### Jhuann: encaminhamento para o seminário

Jhuann situou a experiência no tema **TICs no ensino de Física** e propôs que a página tivesse **público e finalidade didática explícitos**. O interesse do grupo é usar a interface para formular perguntas, testar previsões e discutir o que a tecnologia acrescenta à aprendizagem, e não somente demonstrar uma conversão visual em som.

## O que está na página publicada em 20/11/2026

A [página interativa](https://jhuannp.github.io/desenhe-o-som/) reúne dois modos:

1. **Forma de onda:** o estudante modifica e ouve um sinal periódico. O desenho representa a amplitude do sinal ao longo do tempo em um período.
2. **Desenho sonoro:** o estudante escolhe círculo ou estrela, ou cria um traço livre. Uma bolinha percorre o traço; a posição vertical de pontos ao longo do caminho é convertida em frequência sonora entre 220 e 880 Hz. É possível alterar o tempo total do percurso e o volume.

Essa implementação usa **Canvas 2D e Web Audio API**. Ela incorpora a proposta de figura percorrida por uma bolinha e a regra **posição vertical → nota**. A bolinha segue a linha desenhada; o programa **não** calcula a proximidade entre uma partícula independente e todos os pontos da tela. As demais correspondências e expansões descritas no PDF continuam como ideias para discussão, não como recursos entregues. O texto explicativo mais desenvolvido que Aymee se ofereceu para escrever também está pendente de integração.

## Cuidados para apresentar a atividade

- Um círculo ou uma estrela não é, em geral, o gráfico de uma única função `y(x)`. Nesse modo, a figura é tratada como **trajeto bidimensional**.
- A figura não possui um som próprio. A página realiza uma **sonificação** segundo uma regra escolhida pelo programa. Alterar a regra pode alterar o som sem mudar o desenho.
- A posição **vertical na tela** foi associada à **altura musical** por convenção. Ela não é a amplitude física da onda sonora.
- O encontro da bolinha com o traço, por si só, não demonstra **interferência**. Para discutir interferência, seria necessário combinar sinais e analisar sua superposição.
- Áudio e figuras predefinidas podem abrir alternativas de interação, mas **não comprovam acessibilidade**. A experiência precisa de avaliação com pessoas usuárias de recursos assistivos, além de descrição textual e operação por teclado.

## Perguntas para levar à turma

1. Antes de ouvir: como vocês acham que círculo e estrela soarão? Por quê?
2. Qual parte da figura o programa usa para decidir a nota? Que aspectos ele deixa de fora?
3. Se mantivermos a figura e mudarmos a regra de conversão, o som será o mesmo?
4. O que o modo de forma de onda mostra que o modo de desenho sonoro não mostra, e vice-versa?

**Estado do registro:** reúne apenas as contribuições visíveis nos materiais compartilhados em 20/11/2026. Novas decisões do grupo devem ser acrescentadas com data e autoria, sem reatribuir ideias anteriores.
