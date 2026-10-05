---
id: 006
título: "A corrida mortal"
subtítulo: "Uma apreensão parcial não te deixa meio roubado. Deixa você como o concorrente entre o atacante e o dinheiro. E ainda o acordo estranho que vocês dois podem fechar no lugar disso, que troca a morte por um sequestro."
língua: pt-BR
autor: Yuri da Silva Villas Boas
papers: [DR]
tempo_de_leitura: ~9 min
capa: assets/cover-1200x675.webp
capa_alt: "Uma balança de pratos em luz baixa. Um crânio humano num prato e uma ampulheta no outro, pesados um contra o outro."
---

# A corrida mortal

<p align="center"><img src="assets/cover-1200x675.webp" alt="Uma balança de pratos em luz baixa. Um crânio humano num prato e uma ampulheta no outro, pesados um contra o outro." width="680"></p>

Todo plano de autocustódia tem um ponto em que deixa de ser sobre software. Tem
alguém dentro da sua casa. Estão com a sua hardware wallet, com o seu celular e
com você, e o que vier a seguir não vai ser decidido pela sua fonte de
entropia. O que você quer do seu arranjo nesse momento é resistência à coação, e
quase ninguém que vende isso conferiu o que seria preciso para ter.

Quase todo projeto tem uma resposta para esse momento, e a resposta costuma ser
alguma versão de *eles não levam tudo*. Uma passphrase que eles não têm. Uma
chave em outra cidade. Um resgate com timelock. Uma semente dividida em três. A
parte tranquilizadora é a mesma em todas: terminado o encontro, o atacante ainda
está longe do dinheiro.

É justamente essa tranquilidade que é o problema, e vale destrinchar por quê,
porque o argumento tem quatro passos e cada um é sem graça sozinho.

## A coisa que você não consegue fazer

Comece por algo que soa como tecnicalidade.

Você consegue provar que sabe um segredo. Assina uma mensagem, entrega uma
pré-imagem, gasta do endereço. Provar que você *não* sabe, ou que não existe
nenhuma cópia em lugar nenhum ao seu alcance, não é uma versão mais difícil da
mesma tarefa. Não existe protocolo para isso, porque não há o que exibir.
**Você não consegue provar que esqueceu.**

Repare no tanto minúsculo que bastaria esconder para isso valer. Um cartão SD.
Uma senha que você decorou de uma conta de e-mail onde tem um arquivo cifrado.
Quatro palavras escritas na margem de um livro na estante. Nada disso é exótico,
e nada disso pode ser descartado por alguém parado na sua sala.

Então o atacante que terminou com você fica com uma pergunta que não consegue
fechar: existe outra cópia? E ele tem que responder do único jeito racional, que
é supor que sim.

## No que isso transforma um assalto

Junte as duas metades, e lembre do tipo de ativo que é esse. Bitcoin é ao
portador e é rival: o primeiro gasto válido leva tudo, e não há recurso, não há
estorno, não há seguradora para ligar.

Se ele sai com um caminho até as suas moedas que ainda não terminou, e te
solta, vocês dois estão apontados para o mesmo dinheiro com o mesmo relógio
correndo. Ele está trabalhando em cima do que apreendeu. Você está, até onde ele
sabe, andando até um segundo backup que ele nunca achou. Só um de vocês chega
primeiro.

Nesse ponto você não é uma vítima em nenhum sentido que interesse a ele. Você é
o outro corredor.

### Quanto mais gentil o fallback, pior fica

Um projeto que falha de forma dura entrega ao atacante ou tudo ou nada. Um
projeto que degrada *com elegância* foi feito para dar a ele um caminho lento,
parcial e eventual, o que é outro jeito de dizer que ele mantém as chances dele
bem abaixo da certeza enquanto deixa o saldo inteiro na mesa. Essa combinação é
exatamente a que maximiza o que ele ganha removendo a concorrência.

Degradação elegante é uma virtude em quase todo sistema que você vai construir
na vida. Neste aqui é o modo de falha, e os produtos que mais calorosamente
anunciam isso estão sentados na pior parte da faixa.

## A aritmética, que infelizmente é simples

Com você vivo e solto, o esperado dele é a chance de ganhar a corrida vezes o
valor do estoque. Se ele te mata, a chance dele vai para perto de um. A
diferença entre esses dois números é o que ele ganha. Ele age quando isso passa do que um
homicídio custa a ele.

É essa a conta inteira. Nenhuma criptografia aparece em lugar nenhum dela, e é
por isso que "a criptografia é forte" não é resposta. O perigo é fabricado pelo
*formato* do caminho de recuperação, não pela dureza dele. Resistência à coação
mora na camada de incentivos, e a maioria dos modelos de ameaça não tem uma
coluna para isso.

E isso não é um experimento mental sem dados de desfecho. Dezesseis dos 351
incidentes do registro público de Jameson Lopp registram uma vítima morta. São
4,6%, e é um piso e não uma estimativa, porque um assassinato tende a ser
noticiado como assassinato e não como ataque a bitcoiner, então os que nunca são
ligados a uma carteira nunca entram na conta.

## 'Leve-me com você' — o acordo sherazadiano

O que vem a seguir é uma hipótese sobre o que a estrutura de incentivos pode
levar os agentes a fazer. Até hoje não tenho evidência empírica confirmando
nenhuma instância particular dessa cadeia de eventos, ainda que, pelos mesmos
mecanismos de supressão de informação tratados em
[**The Denial Spiral**](https://zenodo.org/doi/10.5281/zenodo.22778480) e percorridos em
[**Anosognosia**](https://yuri-svb.github.io/posts/007-anosognosia/),
o silêncio seja sobredeterminado.

Em qualquer ponto de um wrench attack contra um arranjo vulnerável à corrida
mortal, o agressor, a vítima ou os dois podem perceber os incentivos para o
movimento terminal. Nessa situação a vítima pode de fato **se oferecer** para
ficar sob a custódia do agressor, num **acordo sherazadiano** torto. Em *As Mil
e Uma Noites*, a protagonista se oferece para o que acaba sendo um cativeiro a
fim de impedir a morte de terceiros, e depois prolonga esse cativeiro noite
após noite, mil e uma vezes, para adiar a própria, oferecendo desfechos de
suspense em troca da vida.

<p align="center"><img src="assets/m3-scheherazade.webp" alt="A pintura de Ferdinand Keller, de 1880. Sherazade está recostada num aposento à luz de lamparina, uma das mãos erguida no meio de uma frase, enquanto o sultão barbudo se inclina para fora da sombra para ouvir." width="680"></p>

<p align="center"><em>Ferdinand Keller, “Scheherazade und Sultan Schariar” (1880), domínio
público. Ela está no meio da história e ele está ouvindo, e é esse o mecanismo
inteiro: o que compra a manhã seguinte é a história não ter acabado. No livro
ela é perdoada na milésima segunda manhã.</em></p>

Numa corrida mortal, trocar o movimento terminal por um sequestro baixa a
responsabilidade penal do agressor mantendo praticamente a mesma vantagem na
corrida, e poupa a vida da vítima. Vítima e agressor podem, assim, concluir que
o acordo é mutuamente vantajoso, e cooperar com o sequestro.

## Sucesso claro ou fracasso claro — nunca uma corrida

<p align="center"><img src="assets/m1-the-gray-band.png" alt="Uma linha do fracasso claro ao sucesso claro, com a faixa do meio marcada como a corrida. A faixa diz: o atacante tem um caminho, você está vivo, e te remover é o que aumenta as chances dele. Decisório, não criptográfico." width="680"></p>

Daí sai o teste, e ele é direto o bastante para aplicar sem base em matemática.

Resistência à coação significa deixar só dois tipos de final. Ou o ataque
fracassa claramente, isto é, o que ele levou não chega a lugar nenhum e você não
tem mais nada transmissível para entregar. Ou vence claramente, isto é, ele pega
as moedas durante o encontro e não há corrida depois porque não sobrou nada pelo
que correr.

Tudo entre os dois é a faixa perigosa. Não "menos seguro". Estruturalmente
diferente, porque é a única região em que te matar compensa.

O segundo final te custa o dinheiro, e as pessoas não gostam de ouvir que isso
conta como aprovação. Conta, porque a régua aqui é a sua sobrevivência primeiro
e as suas moedas depois. Um esquema que entrega o saldo de forma limpa não mata
ninguém. Um esquema que o deixa no meio do caminho é pior que essa perda limpa,
o que é uma frase para se sentar em cima, dado que quase todo fallback do
mercado foi feito para deixá-lo no meio do caminho.

## As duas rotas para resistência à coação

<p align="center"><img src="assets/m2-two-exits.png" alt="Dois jeitos de passar no critério: tirar a corrida, de modo que nenhum caminho viável exista depois da apreensão e a custódia siga individual; ou tirar o alcance, de modo que quem vence seja um delegado remoto, o que torna a custódia compartilhada. Afirmação estrutural sobre o que passa no critério, não uma medição." width="680"></p>

O incentivo só morde contra um corredor que ele consegue alcançar de fato. Então
são duas rotas e não há uma terceira, e todo produto no campo pega uma das duas
ou nenhuma.

**Tirar a corrida.** Arranjar as coisas de modo que, depois da apreensão, não
exista caminho viável nenhum. O segredo fica atrás de algo que não pode ser
entregue sob pressão nenhuma e não pode ser reconstruído a partir do que ele
levou. A custódia continua só sua.

A outra é tirar o alcance dele. Fazer com que quem vai vencer a corrida seja
alguém que ele não consegue pegar: um delegado remoto que guarda a capacidade de
resgate e não está na sala. A corrida continua existindo, mas o corredor que ele
precisaria eliminar está a mil quilômetros, e te matar não rende nada a ele.

### A rota do delegado funciona, e não é autocustódia

Essa segunda rota é real, e isso deve ser dito com todas as letras e sem má
vontade. Ela passa no critério.

Passa assumindo que o seu delegado vai te recusar. É esse o mecanismo: a mesma
recusa que derrota um pedido seu sob coação, com uma arma na sua cabeça, também
derrota um pedido seu genuíno no pior dia da sua vida, e não existe versão em
que ela distinga os dois, porque distinguir é justamente o que não dá para
fazer. Você reintroduziu a contraparte confiável que o exercício inteiro queria
remover. *Not your keys, not your coins* aqui não é slogan, é só uma descrição
correta do que você contratou.

Vale saber qual das duas você escolheu. Tem bastante gente na rota do delegado
achando que está na outra.

### Onde os arranjos geográficos caem

Espalhar partes por várias cidades parece a primeira rota e se comporta como a
segunda, mal. Assim que o wrench attack para, quem chegar primeiro a sites
suficientes leva o dinheiro, e isso agora é uma corrida a pé sobre terreno
físico. Pode funcionar: se os sites forem difíceis o bastante de alcançar, a
chance dele cai a ponto de a corrida não valer a pena.

Mas veja o que isso concede. A sua segurança virou uma pergunta sobre quão boas
são as suas defesas físicas contra um atacante físico. Isso é ouro com passos
extras, e se você vai acabar guardando objetos em cofres, os objetos podiam pelo
menos ter sido ouro.

## O residual, dito com honestidade

Uma janela sobrevive, e fingir que não faria deste texto o mesmo tipo de
documento que ele está criticando.

Na construção tácita existe um período de mais ou menos um a dois minutos no fim
da derivação em que o estado está vivo. Um atacante que apreende dentro dessa
janela ganha uma raspagem do último passo, não um começo do zero. Se aquele
minuto raspado vale um homicídio depende de outras condições que em geral não
valem, mas é uma janela real e o lugar dela é à vista.

É essa a cara de uma afirmação de resistência à coação quando ela é honesta: um
número, uma duração e as condições em que aquilo importa. Compare com "oferece
negação plausível", que não limita nada e ninguém consegue conferir.

## Quatro perguntas, e elas são suas

O que presta aqui não é o argumento. É que resistência à coação desaba num teste
que você roda no seu próprio arranjo esta tarde.

1. **Alguma parte disso depende de o atacante não saber alguma coisa?** Não de
   não ter uma chave. De não ter *conhecimento* de um recurso, de um hábito, de
   um esconderijo.
2. **Depois que eles têm os seus aparelhos e tudo que você diria sob pressão,
   ainda sobra um caminho até as moedas?** Um lento conta. Um lento é o problema
   inteiro.
3. **A sua custódia é individual de verdade?** Ou existe uma pessoa de cuja
   recusa a sua segurança depende, e você decidiu isso de propósito?
4. **Existe algum estado do seu arranjo em que o ataque acaba claramente?** Em
   que ele tem, ou em que não sobrou nada para ele pegar, e de um jeito ou de
   outro não há motivo para voltar.

São essas as quatro perguntas pelas quais eu cobro. Elas valem pouco como
segredo e valem bastante como hábito, então estão aqui. Se o seu arranjo responde
a quarta com "bom, no fim das contas ele conseguiria", você achou a faixa.

---

*A cadeia acima está enunciada direito, com o lema, o critério e a construção que
passa nele, em* [***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*,
acesso aberto, sem cadastro. O companheiro dele,*
[***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*, precifica quanto
tempo o encontro dura, e não como ele termina: por que negação, iscas e PINs de
coação são um recurso comum que o uso de todo mundo vai drenando.*

*Dados de incidentes do* [*registro de Jameson Lopp*](https://github.com/jlopp/physical-bitcoin-attacks)*,
uma amostra de imprensa: perde o que não é noticiado e pesa demais o que virou
manchete. Casos novos que eu encontro vão para lá, e não para uma base minha.*

---

**Se isso valeu seu tempo.** Mande para quem te convenceu do seu arranjo atual.
Uma ⭐ no [Great Wall](https://github.com/Yuri-SVB/Great-Wallet), na
[pesquisa](https://github.com/Yuri-SVB/great-wall-docs) ou
[nestes textos](https://github.com/Yuri-SVB/great-wall-posts) não custa nada e faz
o trabalho ser encontrado. E se você quiser financiá-lo, o
[apoio](https://github.com/Yuri-SVB/support) aceita ⚡ Lightning e on-chain, sem
cadastro, sem níveis e sem contrapartida nenhuma.
