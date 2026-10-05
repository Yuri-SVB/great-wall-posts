---
id: 009
título: "Esconder seu bitcoin ainda protege você?"
subtítulo: "O Brasil tem a pior estatística do mundo para o tipo de ataque em que esconder não adianta, e o mercado continua vendendo esconderijo."
veículo: bitcoinblock.com.br
língua: pt-BR
autor: Yuri da Silva Villas Boas
data_publicação: 2026-09-22
papers: [DS, DR]
tempo_de_leitura: ~7 min
capa: assets/capa-1200x675.webp
capa_alt: "Homem tenta tapar o sol com a peneira, metáfora de esconder bitcoin como defesa contra sequestro."
---

# Esconder seu bitcoin ainda protege você?

<p align="center"><img src="assets/capa-1200x675.webp" alt="Homem tenta tapar o sol com a peneira, metáfora de esconder bitcoin como defesa contra sequestro." width="680"></p>

**Esconder bitcoin é o conselho padrão para quem teme ser sequestrado por causa
dele, e vem em três partes: não conte a ninguém, negue se perguntarem, e tenha um
*decoy* para entregar.**

**As três são apostas sobre o que o criminoso vai *acreditar*. E nenhuma delas
nunca foi avaliada como aquilo que é: esconder bitcoin é um mecanismo de
segurança cuja força inteira depende da ignorância do adversário.**

Este texto argumenta que esconder bitcoin não é só ineficaz. É **autodestrutivo em
escala**, e a conta cai em quem nunca seguiu o conselho.

---

## Esconder bitcoin tem nome, número e ficha corrida

Antes de tudo, o vocabulário.

*Decoy*, ou carteira-isca. O vulgo "dinheiro do ladrão", que nós, brasileiros,
conhecemos muito bem: um montante menor, separado de propósito para ser entregue
em caso de roubo.

Em engenharia de segurança, a família inteira dessas táticas tem nome e catálogo.
Chama-se *Reliance on Security Through Obscurity*, registrada como
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). Em qualquer outro
domínio isso é considerado defeito de projeto. Em custódia de bitcoin, é o
consenso.

### O paradigma é condescendente

Esse paradigma, que em design de protocolo se chama **obscuridade**, é
intrinsecamente condescendente. É supor que o ladrão não é mentalmente capaz de
ler os mesmos manuais, assistir aos mesmos tutoriais e fazer os mesmos cursos que
suas vítimas.

Se você é capaz de aprender um procedimento na internet, um ladrão também é. E
certamente saberá que o procedimento existe. No fundo, esconder bitcoin é um
plano que depende de o adversário não ter feito a lição de casa.

---

## O Brasil está no pior quadrante do registro

Jameson Lopp mantém há anos um [registro público de ataques físicos a detentores
de bitcoin](https://github.com/jlopp/physical-bitcoin-attacks). Os "ataques da
chave de grifo", o `$5 wrench attack`. Codifiquei os 351 incidentes do registro por
modalidade. O resultado por país não é uniforme: varia em uma ordem de grandeza.

| Jurisdição | Incidentes | Sequestro | Assalto à mão armada | Razão S:A |
|---|---:|---:|---:|---:|
| **Brasil** *(n pequeno)* | 12 | 75,0% | 8,3% | **9,0** |
| França | 61 | 57,4% | 8,2% | 7,0 |
| *Todos os incidentes* | 351 | 35,0% | 22,8% | 1,5 |
| Estados Unidos | 59 | 20,3% | 33,9% | 0,6 |
| Rússia *(n pequeno)* | 10 | 30,0% | 50,0% | 0,6 |

### Nove sequestros para cada assalto

Leia a coluna da direita. Nos Estados Unidos, o ataque típico é um assalto: arma
apontada, transferência imediata, minutos em cena.

No Brasil, a proporção se inverte: **para cada assalto registrado, nove
sequestros**. O ataque brasileiro não é um evento de minutos. É um evento de horas
ou dias, com a vítima sob controle do criminoso o tempo todo.

### A ressalva vem junto, e ela é séria

O registro é uma amostra de imprensa, `n=12` para o Brasil não sustenta nada
sozinho, e a codificação é por palavra-chave em manchete, não por duração medida.
Trate a linha do Brasil como direcional.

A comparação que realmente carrega peso é França contra Estados Unidos: dois
subconjuntos do mesmo tamanho (61 e 59), com composições invertidas. A composição
varia mesmo com as condições locais, e as condições locais brasileiras são
conhecidas de qualquer um que more aqui.

Isso importa porque **toda a promessa de esconder bitcoin depende de o ataque ser
curto**. Um decoy funciona se o criminoso pega os R$ 8 mil e vai embora. Ele não
tem resposta para a pergunta seguinte, feita no terceiro dia, no cativeiro.

---

## O que acontece quando todo mundo é treinado a negar

Aqui está o mecanismo, e ele é econômico antes de ser criptográfico.

### A credibilidade de uma negativa é um recurso comum

Ela é produzida pelo conjunto de todos os detentores e consumida por cada um que
nega. Enquanto negar é raro, negar carrega informação: o criminoso atualiza a
crença dele e a chance de soltar você sobe.

Quando negar vira o roteiro esperado, quando todo canal, todo curso, todo grupo
de Telegram ensina a mesma frase, **uma negativa deixa de carregar informação**.

O interrogatório que começa com "eu não tenho nada" não dá ao criminoso nenhuma
atualização favorável a você. E a continuação racional dele, nesse ponto, não é
soltar. É insistir.

A resposta individualmente racional a esse ambiente é esconder bitcoin melhor e
ensaiar mais. O que **esgota o recurso ainda mais, para todo mundo**.

Chamei isso de **Espiral da Negação**, e o custo dela é uma externalidade
clássica: cai sobre quem precisa ser acreditado. Inclusive sobre quem usa um
arranjo que não depende de mentir. Inclusive sobre quem, honestamente, **não tem
bitcoin nenhum**, e o registro tem casos assim.

### O mercado vende o esgotamento como produto

Diversas consultorias, cursos e tutoriais de autocustódia listam, entre serviços
pagos, a montagem de decoys com treinamento de credibilidade.

Ou seja: paga-se para ficar fluente em uma negativa que, exatamente por ser
ensinada e vendida, o criminoso já desconta. O remédio degrada aquilo que ele
vende, e não só para o cliente.

Existe um mercado inteiro montado em torno de esconder bitcoin com método, e o
método é o que o criminoso estuda.

---

## O problema mais grave: você não pode provar que esqueceu

Há uma segunda falha, e ela é pior, porque é sobre o desfecho e não sobre a
duração.

Parta de um fato simples e incontornável: **ninguém consegue provar que não sabe
de alguma coisa.** Saber é demonstrável; *não* saber, não. Você não tem como
provar que esqueceu a senha, nem que não existe backup em lugar nenhum.

### A Corrida Mortal

Agora considere qualquer esquema que, depois de tomar seu dispositivo, deixe o
criminoso com um caminho **viável porém não concluído** até o dinheiro: uma trava
de tempo, um resgate por delegado, um cofre com atraso, uma chave que ainda
precisa ser quebrada.

Você é solto. E você não consegue provar que não guardou uma cópia utilizável.

O que existe a partir daí é uma **corrida** entre você e ele pelo mesmo saldo. E
uma corrida com um competidor ao alcance da mão cria uma coisa que nenhum
whitepaper de carteira menciona: **um incentivo material para te eliminar.** Não
por crueldade. Por aritmética: tirar o outro corredor da pista é a jogada mais
barata disponível.

Chamei isso de **Corrida Mortal**. No registro, ao menos 4,6% dos incidentes (16 de
351) trazem vítima morta, e esse número é um **piso**, não uma estimativa:
homicídio costuma ser noticiado como homicídio, não como "ataque a detentor de
bitcoin". O desfecho que o argumento prevê está documentado na prática.

E nada disso depende de você ter escondido bem. Esconder bitcoin não mexe em
nenhuma das duas pontas: nem na impossibilidade da prova, nem na aritmética do
corredor a mais.

### Por que o decoy é uma máquina de zona cinzenta

O critério de projeto que sai disso é seco: **um esquema de custódia resistente a
coerção só pode admitir dois desfechos: o ataque claramente funciona, ou o ataque
claramente fracassa. Nunca uma corrida.**

A zona cinzenta é exatamente onde mora o incentivo ao assassinato. Chamei de
**Princípio da Ausência de Zona Cinzenta**.

Note o que isso faz com o decoy. Ele é, por construção, uma máquina de zona
cinzenta: o criminoso sai de lá com a suspeita de que existe mais, e sem nenhum
jeito de encerrar a suspeita. É o pior lugar possível para se estar.

---

## Um caso brasileiro que fecha o argumento

Porto Velho, outubro de 2019. Uma quadrilha sequestra
[Arcilio Nogueira de Souza](https://archive.is/jyzcJ), amarra a vítima em uma
árvore e a agride por horas. Os criminosos **não levaram nada**. O celular não
dava acesso aos fundos.

Esse caso é o argumento inteiro em um parágrafo. A inacessibilidade dos fundos
*não encerrou o ataque*. Ela **prolongou** o ataque.

O esquema "funcionou" no sentido em que a indústria mede, porque o dinheiro não saiu,
e a pessoa passou horas amarrada em uma árvore apanhando, porque do lado de fora da
cabeça dela não havia nada que encerrasse a dúvida do criminoso.

Esconder bitcoin resolveu o problema errado ali: protegeu o saldo e deixou a
pessoa exposta.

É por isso que separo os dois mecanismos. A Corrida Mortal precifica o
**desfecho**. A Espiral da Negação precifica a **duração**. Um arranjo pode ser
inocente de um e culpado do outro, e a maioria dos arranjos vendidos hoje é
culpada dos dois.

---

## O que sobra, se esconder bitcoin não é defesa

Se esconder bitcoin não é mecanismo, a pergunta prática é o que resta. Sobram
três rotas honestas, e é bom saber em qual você está.

### 1. Física

Espalhar geograficamente, cofres, multisig com custódia distante. Funciona, e
reduz a segurança do bitcoin a "quão bom é o cofre". Bitcoin virando **ouro com
passos extras**, com custo que escala com a defesa. Para a imensa maioria, é
inacessível.

### 2. Delegada

Alguém fora do alcance do criminoso guarda a peça que falta: corretora,
co-custódia, resgate por terceiro. Limpa o critério, mas troca a premissa: a
custódia deixa de ser individual. *Not your keys.* E a rota **fecha** se o
delegado mora perto de você.

### 3. Tácita

O segredo nunca esteve no dispositivo, e não é ditável nem sob tortura, porque é
reconhecimento perceptual, não uma frase. Apreender o aparelho não entrega nada
viável: **fracasso claro**, sem corredor sobrando, com a custódia continuando
individual.

A terceira rota é onde trabalho, e o projeto se chama **Great Wall**. Aqui vale o
aviso que qualquer texto honesto sobre isso precisa ter: **a implementação é um
protótipo. Não coloque suas economias atrás dela ainda.**

Quando isso mudar, estará escrito, com data, em
[`DELIVERED.md`](https://github.com/Yuri-SVB/support/blob/main/DELIVERED.md), que é
um arquivo versionado em git justamente para que "o trabalho está andando" seja
uma afirmação auditável e não uma promessa.

### O efeito colateral contraintuitivo

Há um efeito colateral bonito nessa rota: **um projeto público e não-obscuro
melhora a situação de quem nega.**

Um criminoso que acredita que existe mecanismo eficaz em circulação está
acreditando que mentir não é a única ferramenta disponível para a vítima, e uma
vítima com alternativa real tem menos motivo para mentir.

Esconder bitcoin continua ruim como defesa primária. Mas não é indiferente qual
arranjo essa prática acompanha.

---

## O que eu vendo, e o que eu não vendo

**Não vendo software.** Great Wall, BTC-D20, BIP-450 e os papers são MIT ou
Apache-2.0, e isso não muda: sem versão "pro", sem funcionalidade destravada por
pagamento, sem fila preferencial para quem doou.

Está escrito no [repositório de apoio](https://github.com/Yuri-SVB/support), e está
escrito lá porque promessa em artigo não vale nada e promessa em git tem data.

### Vendo consultoria de autocustódia

É um serviço, e o serviço é este: eu olho o arranjo que você já tem, seja hardware
wallet, passphrase, multisig, isca ou plano de herança, e respondo quatro perguntas
em relatório fechado:

1. A sua segurança se apoia em algum **truque secreto**? Ela depende de o
   criminoso não saber o que você faz, e como você faz?
2. Apreendidos os seus dispositivos e os seus segredos, o criminoso conseguiria
   gastar **na hora**, ou só **depois de algum tempo**? "Depois" quer dizer que
   você continua sendo um corredor.
3. A sua custódia é **estritamente individual**? Mais alguém pode fazer alguma
   coisa que te impeça de chegar às suas próprias moedas?
4. Ela depende de **objetos específicos em lugares específicos**? E esses
   lugares são seus?

Não é venda de produto: na maioria das auditorias, a recomendação é mexer no que
já existe, e em algumas o veredito é que está razoável. O que não vou fazer é
montar decoy com treinamento de negativa, pelo argumento inteiro acima.

Contato: **yuri@t3infosecurity.com**.

### E se você não quer comprar nada

Os papers são gratuitos e não estão atrás de nenhum cadastro —
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) (a corrida e o
critério) e [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) (a
espiral, a classificação dos produtos obscuros no mercado e o método de
codificação do registro).

Dados novos de incidentes vão para o
[registro do Lopp](https://github.com/jlopp/physical-bitcoin-attacks), e não para
um banco de dados meu, porque essa informação é patrimônio público e pertence a
todo mundo, inclusive ao próximo alvo.

Se este texto foi útil, [o apoio fica aqui](https://github.com/Yuri-SVB/support) —
Lightning e on-chain, sem contrapartida nenhuma e sem cadastro.

---

*Yuri da Silva Villas Boas é criptógrafo aplicado, autor da BIP-450 (Formosa) e do
protocolo Great Wall. As duas afirmações centrais deste artigo estão desenvolvidas
formalmente nos papers citados, atualmente em avaliação acadêmica.*
