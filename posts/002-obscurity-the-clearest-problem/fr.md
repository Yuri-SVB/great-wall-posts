---
id: 002
titre: "L'obscurité, le problème le plus clair dont personne ne parle"
sous_titre: "Le principe de conception que cette communauté rate le plus souvent, et les manuels qui le prouvent."
langue: fr
auteur: Yuri da Silva Villas Boas
papers: [DS]
temps_de_lecture: ~8 min
couverture: assets/cover-1200x675.webp
couverture_alt: "Deux personnes sur un canapé, l'une devant un ordinateur portable et l'autre en train de lire, toutes deux occupées, pendant qu'un éléphant énorme portant un masque de Guy Fawkes est assis dans la pièce derrière elles sans que personne le relève."
---

# L'obscurité, le problème le plus clair dont personne ne parle

<p align="center"><img src="assets/cover-1200x675.webp" alt="Deux personnes sur un canapé, l'une devant un ordinateur portable et l'autre en train de lire, toutes deux occupées, pendant qu'un éléphant énorme portant un masque de Guy Fawkes est assis dans la pièce derrière elles sans que personne le relève." width="680"></p>

Quiconque a suivi un cours de conception de protocoles a croisé le principe de
Kerckhoffs vers la deuxième semaine. C'est celui que tout le monde sait réciter.
Et cette communauté, capable de débattre six heures pour savoir si le générateur
aléatoire d'un portefeuille est digne de confiance, livre des défenses contre la
contrainte physique bâties sur la sécurité par l'obscurité, et elles échouent dès
la première page du manuel.

Rien de subtil. Les manuels le disent d'eux-mêmes, et ce texte se contente à peu
près de les citer.

## Ce que dit vraiment Kerckhoffs

Laissez le jargon de côté. Un système doit rester sûr quand l'attaquant sait
exactement comment il fonctionne. Tout sauf la clé est public : la conception, le
logiciel, la procédure, le fait que la procédure existe. On juge une conception à
ce qu'elle vaut face à quelqu'un qui a lu la même documentation que vous.

Ce n'est pas du pessimisme sur les attaquants. C'est un aveu sur la publication.
Dès qu'une défense arrive chez le grand public, sa description se trouve dans un
article d'assistance, dans la langue de l'attaquant, indexée, gratuite.

### La sécurité par l'obscurité a un numéro de catalogue

La famille de tactiques qui enfreint cette règle porte un nom et un numéro de
dossier. *Reliance on Security Through Obscurity*, cataloguée
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). Dans n'importe quel
autre domaine logiciel, cette entrée désigne un défaut qu'on corrige. Dans la
conservation de bitcoin, c'est la recommandation consensuelle.

Et ce paradigme, que la conception de protocoles appelle **obscurité**, est
intrinsèquement condescendant. Il suppose que le voleur n'a pas les moyens
intellectuels de lire les mêmes manuels, de regarder les mêmes tutoriels et de
suivre les mêmes cours que ses victimes. Si une procédure s'apprend sur internet,
un voleur l'apprend aussi, et il saura à coup sûr que la procédure existe.

Visez la supposition, pas ceux qui la portent. Les gens qui livrent ces
fonctions sont des ingénieurs soigneux qui se sont trompés sur une prémisse. Il
se trouve que c'est celle qui porte tout le reste.

## Trois paris sur ce qu'un attaquant va croire

Le conseil courant vient en trois parties : détenez discrètement, niez si on vous
demande, gardez une petite somme à remettre. Reformulez-les sans le ton
rassurant et ce sont trois paris sur l'état mental d'un adversaire. Pas trois
contrôles. Trois suppositions sur ce que quelqu'un d'autre va penser, faites par
la personne la moins en mesure de vérifier.

Un contrôle fonctionne quand l'attaquant est au courant. Toute la distinction est
là, et chaque mécanisme ci-dessous échoue de ce côté-là.

## La classe, dans les mots des fabricants eux-mêmes

Je vais citer la documentation plutôt que la caractériser, parce que la
classification fait le travail toute seule et que la caractériser invite un débat
sur les intentions dont personne n'a besoin.

### Le PIN qui efface, et la sauvegarde qu'il présuppose

La Jade de Blockstream embarque un PIN alternatif qui, selon les termes du centre
d'aide, "automatically delete[s] the encrypted wallet information from Jade if
entered". Il est présenté comme "especially useful in the event of a physical
threat, as you can provide this PIN to an attacker". Saisissez-le et l'appareil
n'affiche que "Internal Error", si bien que l'effacement se lit comme une panne
et non comme une décision.

Rendons justice : l'effacement lui-même est réel, instantané, et ne peut pas être
interrompu. Il n'y a pas de course à gagner.

Lisez maintenant l'avertissement suivant sur la même page. Ensuite "there is no
way to regain access to your funds except by restoring using your recovery
phrase", donc le détenteur doit "make sure you have a backup before proceeding".

La fonction présuppose une sauvegarde. Celui qui suit la documentation en a une ;
celui qui ne la suit pas a détruit ses propres économies sous pression. Ce que
l'effacement retire n'est donc pas le secret. Il retire le chemin *de l'appareil*
vers le secret, et laisse debout celui qui passe par le souvenir qu'a la personne
de l'endroit où se trouve la sauvegarde.

L'effacement supprime la route qui n'obligeait à faire de mal à personne, et
conserve celle qui y oblige.

### Coldcard documente la régression

Vous n'avez pas à déduire l'étape suivante. Un fabricant l'a publiée.

Coldcard propose des PIN pièges, dont un portefeuille de contrainte décrit comme
"a personal safety feature… If you must reveal a PIN under duress, give the
duress PIN instead of your Main PIN". Logique de leurre ordinaire. La
documentation du firmware examine ensuite ce qui se passe quand le leurre n'est
pas cru, et son conseil est d'escalader : "you may be asked what the actual
duress PIN is, while under duress. We suggest providing the 'brickme' PIN in that
case."

C'est un fabricant qui envisage un attaquant sachant que les leurres existent, et
qui recommande un effacement irréversible effectué avec la victime encore dans la
pièce, encore en train de respirer, encore disponible pour qu'on lui demande où
est la sauvegarde.

Deux autres aveux sur la même page méritent d'être cités parce que les fabricants
en font rarement. Le premier concède que le leurre est distinguable : "if you are
somehow facing an attacker who is willing to verify he has the real main PIN,
it's possible that careful analysis of system responses will imply he's working
with the duress PIN." Le remède proposé n'est pas une réparation. C'est une
demande : "if you discover any sequences that reveal this easily, please tell us
and we'll see if we can cover them up better."

La sécurité par l'obscurité énoncée comme programme de maintenance. Ce qui est défendu, ce n'est
pas que le leurre soit indistinguable, mais que personne n'a encore publié
comment le distinguer. Un dispositif dont la sécurité est l'état actuel de la
file de divulgation est un dispositif que vous ne pouvez pas invoquer dans la
pièce, parce que vous n'avez aucune idée de ce qu'a lu l'homme en face de vous.

Le second aveu est le démenti lui-même, proposé là où briquer l'appareil passe
mal : "alternatively, you can say you set the duress PIN once, but have since
forgotten it."

Vous ne pouvez pas prouver que vous avez oublié. C'est tout l'article compagnon
en cinq mots, et le voilà en guise de conseil publié. Le fabricant a énuméré les
branches et a trouvé un bluff sur chacune.

### Ce que chaque fabricant affirme réellement

Cela compte, et c'est là que la plupart des critiques de ce genre se trompent.
Les trois entreprises ne font pas les mêmes affirmations, et un fabricant qui
livre un mécanisme sans affirmer qu'il déjoue la contrainte n'a pas commis
l'erreur dont parle ce texte.

Blockstream vend l'effacement pour la menace physique, et n'affirme rien de tel
pour ses portefeuilles à passphrase. Le cadrage « contrainte » des leurres par
passphrase est une invention de la communauté, pas du fabricant. Coldcard vend
les deux moitiés. Trezor est l'image inversée de Blockstream : ses portefeuilles
à passphrase sont vendus sur la déniabilité, tandis que son wipe code, que le
fabricant lui-même appelle un PIN « self-destruct » et qui efface la graine de
récupération, est documenté sans la moindre mention de contrainte, de coercition
ou de menace physique.

Trezor est aussi celui à qui l'on a demandé, en janvier 2022, de rendre
l'effacement *dissimulable* : un message défini par l'utilisateur à la saisie,
pour qu'un effacement passe pour une panne matérielle. La demande a été close en
**not planned**. L'appareil annonce toujours l'effacement franchement.

Ce refus est le document le plus intéressant de toute la classe. Il montre que le
déguisement en "Internal Error" n'est pas intrinsèque à l'effacement. C'est un
choix de présentation : un fabricant l'a construit, un autre s'est vu le demander
directement et a décliné.

### Une ignorance, ou deux

Il y a une façon propre de les classer, et ce n'est pas par la probabilité que
l'attaquant soit ignorant. C'est par le nombre de choses distinctes qu'il doit
ignorer.

Un leurre en demande une. Il ne doit pas savoir que les leurres existent.
Accordez-lui cela et le leurre fonctionne vraiment : il repart avec un solde
plausible et une histoire qui tient.

Une autodestruction en demande deux, et elles sont indépendantes. Il ne doit pas
savoir que la fonction existe, pour que la panne se lise comme une panne. Et il
ne doit pas raisonner jusqu'à la sauvegarde, que le manuel a dit au détenteur de
conserver. La seconde ne découle pas de la première. « Cet appareil est cassé »
n'a jamais impliqué « cette personne n'a pas de bitcoin ». Cela implique que
l'instrument est cassé, et la question naturelle suivante est où vous rangez la
sauvegarde, posée à quelqu'un qui est toujours debout là.

Donc face à un attaquant informé l'autodestruction échoue pour la raison
kerckhoffsienne ordinaire, et face à un ignorant elle échoue quand même, parce
que la croyance qu'elle fabrique ne met pas fin à la rencontre. C'est le seul
dispositif obscur qui n'a aucune branche où il l'emporte.

<p align="center"><img src="assets/m1-one-ignorance-or-two.png" alt="Un leurre exige que l'attaquant ignore une chose. Une autodestruction exige qu'il en ignore deux, indépendamment, et n'a aucune branche où elle l'emporte." width="680"></p>

Il existe une version plus discrète du même échec. La FAQ de Sparrow documente
une option permettant de stocker les données du portefeuille sur un support
amovible, en notant qu'elle "allows you to store all Sparrow data on removable
media making for more plausible deniability". La page de bonnes pratiques de
Sparrow, elle, garde les mots de la graine sauvegardés à part, "ideally in a
different location". L'attaquant contraint donc la sauvegarde de la graine, la
charge dans son propre portefeuille, et ne touche jamais au support caché. Un
leurre se tient au moins entre lui et les pièces. Celui-ci ne s'en approche pas,
et ce qu'il ajoute, c'est l'assurance nécessaire pour mentir.

## Quatre-vingt-huit personnes, douze affaires

Cette classe suppose un adversaire dont le dossier dit qu'il n'existe pas.

Le parquet français a mis en cause 88 personnes dans une douzaine d'affaires
d'enlèvement et d'extorsion liées aux cryptomonnaies, ce qui est un décompte à un
instant donné d'une série de poursuites en cours et non un total clos. Le
décompte de CertiK pour le premier semestre 2026 fait passer les invasions de
domicile de 1 à 20 sur 52 incidents en glissement annuel, ce qui est
l'échantillon semestriel d'une entreprise et non le registre public, donc lisez
la direction et pas la décimale.

Où que se stabilisent les chiffres exacts, ils décrivent des équipes organisées
avec reconnaissance et sélection des victimes à partir de bases de données
fuitées. Pas des opportunistes incapables de lire une page d'assistance dans la
langue où elle a été écrite.

## L'effet boomerang

L'obscurité n'est pas seulement inefficace. Vendue à grande échelle, elle se
retourne contre elle-même, et ceux qu'elle blesse le plus n'ont rien acheté.

Le leurre n'est pas seulement une pratique tolérée. C'est un produit et un
programme. Un cabinet hispanophone de conseil en autoconservation liste parmi ses
offres payantes "*Passphrase (tu bóveda señuelo)* — Billetera señuelo + billetera
real. Protección ante coacción/coerción" : un portefeuille leurre commercialisé,
en toutes lettres, comme protection contre la contrainte. Des guides publiés
entraînent la prestation. L'un demande au détenteur de garder un petit solde sur
la graine nue, en tant que ce que vous remettriez sous contrainte physique, en
ajoutant que « pour que cela fonctionne, le solde leurre doit être *crédible* :
assez pour ressembler à un vrai portefeuille, pas assez pour vous anéantir s'il
est perdu ».

Lisez cela comme un objectif pédagogique et le problème saute aux yeux. Un leurre
n'a besoin d'être crédible que devant un attaquant susceptible de ne pas y
croire, et le conseil se tait sur ce qui arrive quand il n'y croit pas, ce qui
est toute la question. La sécurité par l'obscurité est vendue ici comme si
c'était un contrôle, tarifée et enseignée.

### Le déni est un bien commun, et il est en train d'être épuisé

Un entraînement médiatisé augmente la probabilité a priori qu'un démenti fluide
ait été répété. Dès lors que l'attaquant sait que la crédibilité s'enseigne et se
vend, la fluidité cesse d'être une preuve de vérité et devient une preuve de
coaching. Le remède dégrade ce qu'il vend.

Et il le dégrade pour tout le monde. Celui qui ne s'est jamais entraîné, qui dit
la vérité toute nue, nie désormais face à un attaquant qui escompte les démentis
fluides en général. Celui qui ne détient aucun bitcoin aussi. Le développement
complet est dans *The Denial Spiral*, et c'est la raison pour laquelle cette
série traite l'obscurité comme un problème de santé publique plutôt que comme un
problème personnel.

Se cacher suppose un endroit où se cacher. Ce dans quoi disparaît un détenteur
discret, c'est l'immense foule des gens qui visiblement ne détiennent pas de
bitcoin, et cela ne marche que tant que la foule est majoritairement authentique.
Entraînez assez de monde à se présenter comme ordinaire et l'ordinaire cesse de
porter de l'information, parce que l'attaquant ne trie plus les détenteurs des
non-détenteurs. Si tout le monde est une aiguille, il n'y a plus de foin.

<p align="center"><img src="assets/m2-no-hay.webp" alt="Un tas d'aiguilles à coudre sur fond blanc, et rien d'autre que des aiguilles dans le tas." width="612"></p>

<p align="center"><em>Structurel, non mesuré. Personne n'a compté combien de
détenteurs pratiquent la discrétion, et par le mécanisme 1 personne ne le peut :
l'obscurité ne s'annonce pas. L'affirmation porte sur ce qui arrive à la foule à
mesure que l'entraînement se répand, pas sur l'état de la foule aujourd'hui.</em></p>

## Une conception publique rend un démenti ordinaire plus crédible

Une dernière inversion, et c'est la partie qui me surprend vraiment.

Une défense obscure demande à l'attaquant de croire une affirmation, contre son
intérêt à ne pas y croire et sans moyen pour l'un ou l'autre de trancher. Une
conception spécifiée publiquement change ce que coûte cette affirmation. Un
attaquant qui admet que des mécanismes efficaces circulent admet que mentir n'est
pas le seul outil dont dispose la victime, et un détenteur qui a de vraies
alternatives a moins de raisons de recourir au mensonge.

Ainsi une conception propre au sens de Kerckhoffs améliore la position de
précisément ces démentis obscurs qu'elle a été bâtie pour rendre inutiles. La
sécurité par l'obscurité reste infondée comme défense principale. Elle n'est pas
indifférente à la conception qu'elle accompagne.

---

*La classification, la documentation des fabricants et l'argument du bien commun
sont développés dans*
[***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*, accès libre,
sans inscription. Son compagnon,*
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*, porte sur ce
qui se passe une fois l'attaquant déjà dans la pièce : une saisie qui laisse un
chemin faisable mais inachevé transforme un vol en course, et met un prix sur
votre élimination.*

*Chaque citation de fabricant ci-dessus provient de documentation publique, liée
dans l'article. Si j'ai mal lu une fonction, ou si une page a changé,
dites-le-moi et je corrigerai en public.*

---

**Si ça valait votre temps.** Passez-le à quelqu'un qui livre un PIN de
contrainte. Une ⭐ sur [Great Wall](https://github.com/Yuri-SVB/Great-Wallet), sur
[la recherche](https://github.com/Yuri-SVB/great-wall-docs) ou sur
[ces textes](https://github.com/Yuri-SVB/great-wall-posts) ne coûte rien et rend
le travail trouvable. Et si vous voulez le financer,
[support](https://github.com/Yuri-SVB/support) accepte ⚡ Lightning et on-chain,
sans inscription, sans paliers et sans contrepartie.
