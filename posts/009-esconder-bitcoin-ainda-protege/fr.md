---
id: 009
titre: "Cacher vos bitcoins vous protège-t-il encore ?"
sous_titre: "Le Brésil détient la pire statistique au monde pour le type d'attaque où se cacher ne sert à rien, et le marché continue de vendre des cachettes."
langue: fr
auteur: Yuri da Silva Villas Boas
papers: [DS, DR]
temps_de_lecture: ~7 min
traduction_de: pt-BR.md
couverture: assets/capa-1200x675.webp
couverture_alt: "Un homme lève un tamis pour cacher le soleil, et la lumière traverse la toile. C'est l'expression brésilienne pour vouloir cacher ce que tout le monde voit déjà."
---

# Cacher vos bitcoins vous protège-t-il encore ?

<p align="center"><img src="assets/capa-1200x675.webp" alt="Un homme lève un tamis pour cacher le soleil, et la lumière traverse la toile. C'est l'expression brésilienne pour vouloir cacher ce que tout le monde voit déjà." width="680"></p>

**Le conseil standard, pour qui redoute d'être enlevé à cause de ses bitcoins,
tient en trois parties : n'en parlez à personne, niez si on vous pose la
question, et gardez un *decoy* à céder.**

**Les trois sont des paris sur ce que le criminel va *croire*. Et aucune n'a
jamais été évaluée pour ce qu'elle est : un mécanisme de sécurité dont toute la
force repose sur l'ignorance de l'adversaire.**

Ce texte soutient que cacher ses bitcoins n'est pas seulement inefficace. C'est
**autodestructeur à l'échelle**, et la facture retombe sur des gens qui n'ont
jamais suivi le conseil.

---

## Cacher ses bitcoins a un nom, un numéro et un casier

D'abord le vocabulaire.

Un *decoy*, ou portefeuille-leurre. Au Brésil on appelle ça « l'argent du
voleur », et on connaît bien : une somme plus petite, mise de côté exprès pour
être cédée lors d'un braquage.

En ingénierie de la sécurité, toute cette famille de tactiques est cataloguée.
Ça s'appelle *Reliance on Security Through Obscurity*, enregistré sous
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). Dans n'importe quel
autre domaine, c'est un défaut de conception. Dans la garde de bitcoins, c'est le
consensus.

### Le paradigme est condescendant

Ce paradigme, qu'on appelle **obscurité** en conception de protocoles, est
intrinsèquement condescendant. Il suppose que le voleur n'est pas mentalement
capable de lire les mêmes manuels, de regarder les mêmes tutoriels et de suivre
les mêmes formations que ses victimes.

Si vous pouvez apprendre une procédure sur internet, un voleur aussi. Et il
saura certainement que la procédure existe.

---

## Le Brésil occupe le pire quadrant du registre

Jameson Lopp tient depuis des années un [registre public des attaques physiques
contre les détenteurs de bitcoins](https://github.com/jlopp/physical-bitcoin-attacks),
les « attaques à la clé à molette ». J'ai codé les 351 incidents du
registre par modalité. La répartition par pays n'a rien d'uniforme : elle varie
d'un ordre de grandeur.

| Juridiction | Incidents | Enlèvement | Vol à main armée | Rapport E:V |
|---|---:|---:|---:|---:|
| **Brésil** *(petit n)* | 12 | 75,0 % | 8,3 % | **9,0** |
| France | 61 | 57,4 % | 8,2 % | 7,0 |
| *Tous les incidents* | 351 | 35,0 % | 22,8 % | 1,5 |
| États-Unis | 59 | 20,3 % | 33,9 % | 0,6 |
| Russie *(petit n)* | 10 | 30,0 % | 50,0 % | 0,6 |

### Neuf enlèvements pour un braquage

Lisez la colonne de droite. Aux États-Unis, l'attaque typique est un braquage :
arme sortie, virement immédiat, quelques minutes sur place.

Au Brésil, la proportion s'inverse. **Pour chaque vol à main armée enregistré,
neuf enlèvements.** L'attaque brésilienne n'est pas un événement de quelques
minutes. C'est un événement de plusieurs heures ou de plusieurs jours, la victime
restant sous le contrôle du criminel tout du long.

### La réserve vient avec, et elle est sérieuse

Le registre est un échantillon de presse, le `n=12` du Brésil ne soutient rien
tout seul, et le codage se fait par mot-clé de titre, pas par durée mesurée.
Traitez la ligne Brésil comme indicative.

La comparaison qui porte vraiment, c'est la France contre les États-Unis : deux
sous-ensembles de même taille (61 et 59) aux compositions inversées. La
composition varie bien avec les conditions locales, et les conditions locales
brésiliennes sont connues de quiconque vit ici.

Tout cela compte parce que **toute la promesse de cacher ses bitcoins dépend de la brièveté
de l'attaque**. Un decoy fonctionne si le criminel prend les 8 000 reais et s'en
va. Il n'a aucune réponse à la question suivante, posée le troisième jour, en
captivité.

---

## Ce qui arrive quand tout le monde est formé à nier

Voici le mécanisme, et il est économique avant d'être cryptographique.

### La crédibilité d'une dénégation est une ressource commune

Elle est produite par l'ensemble des détenteurs et consommée par chacun de ceux
qui nient. Tant que nier reste rare, nier porte de l'information : le criminel
met à jour sa croyance et vos chances d'être relâché montent.

Dès que nier devient le script attendu, dès que chaque chaîne, chaque formation,
chaque groupe Telegram enseigne la même phrase, **une dénégation cesse de porter
de l'information**.

Un interrogatoire qui s'ouvre sur « je n'ai rien » ne donne au criminel aucune
mise à jour en votre faveur. Et sa suite rationnelle, à ce moment-là, n'est pas
de vous relâcher. C'est d'insister.

La réponse individuellement rationnelle à cet environnement, c'est de mieux se
cacher et de répéter davantage. Ce qui **épuise la ressource encore plus, pour
tout le monde**.

J'ai appelé ça la **Spirale du Déni**, et son coût est une externalité
classique : il retombe sur qui a besoin d'être cru. Y compris sur qui utilise un
dispositif qui ne dépend pas du mensonge. Y compris sur qui, honnêtement, **ne
détient aucun bitcoin**, et le registre contient de tels cas.

### Le marché vend l'épuisement comme un produit

Diverses sociétés de conseil, formations et tutoriels d'autoconservation
proposent, parmi leurs services payants, le montage de decoys avec entraînement
à la crédibilité.

Donc : on paie pour devenir fluide dans une dénégation que le criminel escompte
déjà, précisément parce qu'elle est enseignée et vendue. Le remède dégrade ce
qu'il vend, et pas seulement pour le client.

---

## Le problème plus grave : vous ne pouvez pas prouver que vous avez oublié

Il y a une seconde faille, et elle est pire, parce qu'elle porte sur l'issue
plutôt que sur la durée.

Partez d'un fait simple et incontournable : **personne ne peut prouver qu'il ne
sait pas quelque chose.** Savoir est démontrable ; ne *pas* savoir, non. Vous
n'avez aucun moyen de prouver que vous avez oublié la passphrase, ni qu'aucune
sauvegarde n'existe nulle part.

### La Course Mortelle

Considérez maintenant n'importe quel dispositif qui, une fois votre appareil
saisi, laisse au criminel un chemin **viable mais inachevé** jusqu'à l'argent :
un verrou temporel, une récupération détenue par un tiers, un coffre à délai,
une clé qu'il reste à casser.

On vous relâche. Et vous ne pouvez pas prouver que vous n'avez gardé aucune copie
utilisable.

Ce qui existe à partir de là, c'est une **course** entre vous et lui pour le même
solde. Et une course contre un concurrent à portée de main crée quelque chose
qu'aucun livre blanc de portefeuille ne mentionne : **une incitation matérielle à
vous éliminer.** Pas par cruauté. Par arithmétique. Sortir l'autre coureur de la
piste est le coup le moins cher disponible.

J'ai appelé ça la **Course Mortelle**. Dans le registre, au moins 4,6 % des
incidents (16 sur 351) font état d'une victime tuée, et ce chiffre est un
**plancher**, pas une estimation : un homicide est rapporté comme un homicide,
pas comme « attaque contre un détenteur de bitcoins ». L'issue que l'argument
prédit est documentée dans les faits.

### Pourquoi le decoy est une machine à zone grise

Le critère de conception qui en découle est sec : **un dispositif de garde
résistant à la coercition ne peut admettre que deux issues. L'attaque réussit
clairement, ou l'attaque échoue clairement. Jamais une course.**

La zone grise est exactement là où vit l'incitation au meurtre. J'ai appelé ça le
**Principe d'Absence de Zone Grise**.

Voyez ce que ça fait au decoy. Il est, par construction, une machine à zone
grise : le criminel repart en soupçonnant qu'il y a davantage, sans aucun moyen
de régler ce soupçon. C'est le pire endroit possible où se trouver.

---

## Un cas brésilien qui referme l'argument

Porto Velho, octobre 2019. Un gang enlève
[Arcilio Nogueira de Souza](https://archive.is/jyzcJ), attache la victime à un
arbre et la frappe pendant des heures. Les criminels **n'ont rien emporté** : le
téléphone ne donnait pas accès aux fonds.

Ce cas, c'est l'argument entier en un paragraphe. L'inaccessibilité des fonds
*n'a pas mis fin à l'attaque*. Elle l'a **prolongée**.

Le dispositif a « fonctionné » au sens où l'industrie le mesure, l'argent n'est
pas parti, et la personne a passé des heures attachée à un arbre à se faire
battre, parce qu'en dehors de sa tête il n'y avait rien qui puisse régler le
doute du criminel.

C'est pour ça que je sépare les deux mécanismes. La Course Mortelle tarifie
l'**issue**. La Spirale du Déni tarifie la **durée**. Un dispositif peut être
innocent de l'un et coupable de l'autre, et l'essentiel de ce qui se vend
aujourd'hui est coupable des deux.

---

## Ce qui reste, si cacher ses bitcoins n'est pas une défense

Il reste trois routes honnêtes, et il vaut mieux savoir sur laquelle on est.

### 1. Physique

Dispersion géographique, coffres, multisig avec garde lointaine. Ça marche, et ça
réduit la sécurité du bitcoin à « le coffre est-il bon ». Le bitcoin devient de
l'**or avec des étapes en plus**, à un coût qui croît avec la défense. Pour
l'immense majorité, c'est hors de portée.

### 2. Déléguée

Quelqu'un hors d'atteinte du criminel détient la pièce manquante : une
plateforme d'échange, une cogarde, une récupération par un tiers. Ça satisfait le
critère, mais ça change la prémisse : la garde cesse d'être individuelle. *Not
your keys.* Et la route se **ferme** si le délégataire habite près de chez vous.

### 3. Tacite

Le secret n'a jamais été sur l'appareil, et ne peut pas être dicté même sous la
torture, parce que c'est une reconnaissance perceptuelle et non une phrase.
Saisir le matériel ne donne rien de viable. **Échec clair**, aucun coureur en
trop, garde toujours individuelle.

La troisième route est celle sur laquelle je travaille, et le projet s'appelle
**Great Wall**. Voici l'avertissement que tout texte honnête à ce sujet doit
porter : **l'implémentation est un prototype. N'y mettez pas encore vos
économies.**

Quand ça changera, ce sera écrit, avec une date, dans
[`DELIVERED.md`](https://github.com/Yuri-SVB/support/blob/main/DELIVERED.md), un
fichier tenu dans git précisément pour que « le travail avance » soit une
affirmation auditable et non une promesse.

### L'effet secondaire contre-intuitif

Cette route a un bel effet secondaire : **un projet public et non obscur améliore
la position de ceux qui nient.**

Un criminel qui croit qu'un mécanisme efficace circule est en train de croire que
mentir n'est pas le seul outil dont dispose la victime. Et une victime qui a une
vraie alternative a moins de raisons de mentir.

Cacher ses bitcoins reste mauvais comme défense principale. Mais le dispositif que cette
pratique accompagne n'est pas indifférent.

---

## Ce que je vends, et ce que je ne vends pas

**Je ne vends pas de logiciel.** Great Wall, BTC-D20, BIP-450 et les articles
sont sous MIT ou Apache-2.0, et ça ne change pas : pas de version « pro », pas de
fonctionnalité débloquée par paiement, pas de file prioritaire pour les
donateurs.

C'est écrit dans le [dépôt de soutien](https://github.com/Yuri-SVB/support), et
c'est écrit là parce qu'une promesse dans un article ne vaut rien et qu'une
promesse dans git a une date.

### En revanche je vends du conseil en autoconservation

C'est un service, et le voici : je regarde le dispositif que vous avez déjà,
portefeuille matériel, passphrase, multisig, decoy, plan de succession, ce qu'il
y a, et je réponds à quatre questions dans un rapport fermé :

1. Votre sécurité repose-t-elle sur un **tour de passe-passe** ? Dépend-elle de
   ce que l'attaquant ignore ce que vous faites, et comment vous le faites ?
2. Une fois vos appareils et vos secrets saisis, l'attaquant pourrait-il dépenser
   **tout de suite**, ou seulement **au bout d'un certain temps** ? « Au bout
   d'un certain temps » veut dire que vous êtes encore un coureur.
3. Votre garde est-elle **strictement individuelle** ? Quelqu'un d'autre peut-il
   faire quelque chose qui vous empêche d'atteindre vos propres pièces ?
4. Dépend-elle d'**objets précis dans des lieux précis** ? Et ces lieux sont-ils
   à vous ?

Ce n'est pas de la vente de produit : dans la plupart des audits, la
recommandation est de retoucher ce qui existe déjà, et dans certains le verdict
est que c'est raisonnable. Ce que je ne ferai pas, c'est monter un decoy avec
entraînement à la dénégation, pour tout l'argument ci-dessus.

Contact : **yuri@t3infosecurity.com**.

### Et si vous ne voulez rien acheter

Les articles sont gratuits et derrière aucune inscription :
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) (la course et le
critère) et [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) (la
spirale, la classification des produits obscurs sur le marché, et la méthode de
codage du registre).

Les données d'incidents nouvelles vont au [registre de
Lopp](https://github.com/jlopp/physical-bitcoin-attacks) plutôt que dans une base
à moi, parce que cette information est un bien public et appartient à tout le
monde, y compris à la prochaine cible.

Si ceci vous a été utile, [le soutien se trouve
ici](https://github.com/Yuri-SVB/support). Lightning et on-chain, sans
contrepartie et sans inscription.

---

*Yuri da Silva Villas Boas est cryptographe appliqué, auteur de la BIP-450
(Formosa) et du protocole Great Wall. Les deux affirmations centrales de cet
article sont développées formellement dans les articles cités, actuellement en
évaluation académique.*
