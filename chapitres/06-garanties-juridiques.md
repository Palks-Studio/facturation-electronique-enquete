# Chapitre 6 — Garanties juridiques

> **Navigation :** [← Retour au sommaire](#documentation)

Les chapitres précédents ont permis d'identifier les données collectées, les infrastructures concernées et plusieurs possibilités ou mécanismes documentés d'interconnexion entre facturation, fiscalité, produits, données environnementales, identité numérique et paiement.

L'existence d'une capacité technique d'interconnexion ne signifie cependant pas que son utilisation soit juridiquement autorisée.

Ce chapitre examine donc les garanties juridiques susceptibles d'encadrer, limiter ou interdire certains traitements ou rapprochements de données identifiés au cours de l'enquête.

L'analyse recherche notamment :

- les bases juridiques permettant les traitements ;  
- les finalités pour lesquelles les données peuvent être collectées et réutilisées ;  
- le principe de limitation des finalités ;  
- le principe de minimisation des données ;  
- les conditions applicables au croisement de données provenant de systèmes différents ;  
- les règles relatives au profilage et aux décisions automatisées ;  
- les droits des personnes concernées ;  
- les obligations de transparence ;  
- les règles de conservation et d'accès ;  
- les pouvoirs et positions des autorités de contrôle, notamment la CNIL ;  
- les exigences de nécessité et de proportionnalité ;  
- les éventuelles garanties spécifiques prévues pour l'identité numérique, le DPP et les infrastructures de paiement ;  
- les possibilités et conditions d'une évolution future des finalités ou des bases juridiques.

L'objectif n'est pas de présumer qu'une violation existe.

Il est de déterminer, pour chaque capacité identifiée dans les chapitres précédents, si le droit actuel :

> **l'autorise explicitement ;**

> **l'autorise sous conditions ;**

> **la limite ;**

> **semble l'interdire ;**

> **ou ne permet pas encore de conclure.**

Une attention particulière sera portée à la différence entre une protection inscrite dans le droit actuel et une impossibilité technique.

Une règle juridique peut limiter aujourd'hui un traitement que l'architecture permettrait techniquement.

Inversement, l'existence d'une infrastructure technique ne permet pas de présumer qu'une évolution juridique autorisant de nouveaux usages interviendra ultérieurement.

Le chapitre cherchera donc à identifier à la fois les protections existantes et leurs limites, sans transformer une possibilité d'évolution du droit en intention institutionnelle établie.

---

## Sommaire

- [6.1 — Cadre juridique applicable](#61-cadre-juridique-applicable)  
- [6.2 — Finalité des traitements et réutilisation des données](#62-finalité-des-traitements-et-réutilisation-des-données)  
- [6.3 — Croisement, rapprochement et interconnexion des données](#63-croisement-rapprochement-et-interconnexion-des-données)  
- [6.4 — Profilage et décisions automatisées](#64-profilage-et-décisions-automatisées)  
- [6.5 — Nécessité, proportionnalité et minimisation](#65-nécessité-proportionnalité-et-minimisation)  
- [6.6 — Droits des personnes et contrôle par la CNIL](#66-droits-des-personnes-et-contrôle-par-la-cnil)  
- [6.7 — Garanties propres aux infrastructures étudiées](#67-garanties-propres-aux-infrastructures-étudiées)  
- [6.8 — Évolution des finalités et du cadre juridique](#68-évolution-des-finalités-et-du-cadre-juridique)  
- [6.9 — Vulnérabilités juridiques et limites de l'analyse](#69-vulnérabilités-juridiques-et-limites-de-lanalyse)  
- [6.10 — Ce que ce chapitre permet d'établir](#610-ce-que-ce-chapitre-permet-détablir)

---

## 6.1 Cadre juridique applicable

**Statut : GARANTIES JURIDIQUES ÉTABLIES / POINTS DE VIGILANCE IDENTIFIÉS**

Les chapitres précédents ont étudié principalement l'existence des données, leur circulation et les possibilités d'interconnexion entre différentes infrastructures.

Le Chapitre 6 pose une question différente :

> **le fait qu'un traitement soit techniquement réalisable et poursuive un objectif d'intérêt général suffit-il à le rendre juridiquement admissible ?**

La réponse est négative.

Plusieurs niveaux de droit encadrent les traitements étudiés.

---

### Le RGPD s'applique aux données personnelles utilisées dans le dispositif

Le règlement général sur la protection des données s'applique lorsqu'une information concerne une personne physique identifiée ou identifiable [S36].

Toutes les données contenues dans une facture ne constituent donc pas nécessairement des données personnelles.

Une facture concernant une société peut comporter principalement des informations relatives à une personne morale.

Mais les systèmes de facturation peuvent également contenir des informations permettant d'identifier directement ou indirectement des personnes physiques.

Ce point n'est plus seulement théorique concernant l'exploitation fiscale des données issues de la réforme.

La CNIL qualifie explicitement les données issues de la facturation électronique ajoutées au traitement CFVR de **données personnelles collectées** [S37].

**AVÉRÉ :**

> Au moins une partie des données provenant de la réforme de la facturation électronique entre dans le champ de la protection des données personnelles.

Le dispositif ne se situe donc pas en dehors du RGPD au seul motif qu'il concerne principalement des transactions économiques entre entreprises.

---

### La réforme dispose d'une base légale

Un premier argument doit immédiatement être écarté.

La transmission des données à l'administration n'est pas mise en œuvre sans fondement juridique.

Elle résulte notamment du Code général des impôts, de dispositions législatives et réglementaires organisant la facturation électronique et le e-reporting.

Le décret organisant le dispositif vise lui-même explicitement le RGPD et a été adopté après consultation de la CNIL [S38].

**ARGUMENT INSUFFISANT :**

> « La collecte est obligatoire et réalisée sans consentement, donc elle viole nécessairement le RGPD. »

Le RGPD ne repose pas uniquement sur le consentement.

Un traitement peut notamment être fondé sur une obligation légale ou être nécessaire à l'exécution d'une mission d'intérêt public prévue par le droit [S36].

L'absence de consentement des entreprises ou personnes concernées ne suffit donc pas, à elle seule, à rendre la réforme illégale.

---

### L'existence d'une base légale ne donne cependant pas un droit illimité d'utilisation

C'est ici qu'apparaît une première distinction juridique importante.

Le RGPD impose que les données soient :

> collectées pour des finalités déterminées, explicites et légitimes ;

et :

> non réutilisées ultérieurement d'une manière incompatible avec ces finalités [S36].

Il impose également que les données soient :

> adéquates, pertinentes et limitées à ce qui est nécessaire au regard des finalités poursuivies [S36].

Par conséquent :

```
base légale
   ≠
autorisation générale de réutilisation
```

et :

```
collecte légalement obligatoire  
   ≠
possibilité illimitée de croiser les données pour toute politique publique future
```

**GARANTIE JURIDIQUE ÉTABLIE :**

> Une réutilisation ultérieure de données personnelles doit rester compatible avec le cadre juridique applicable, notamment les finalités et principes de nécessité, de proportionnalité et de minimisation.

Cette distinction devient particulièrement importante au regard des interconnexions étudiées dans le Chapitre 5.

---

### Une découverte importante : les données de facturation alimentent effectivement un traitement algorithmique de ciblage fiscal

Le Chapitre 2 avait laissé ouverte la question des traitements automatisés réellement appliqués aux données issues de la réforme.

La documentation publiée en 2026 permet désormais d'apporter une réponse précise.

La CNIL a examiné l'intégration des données issues de la facturation électronique au traitement automatisé **CFVR — ciblage de la fraude et valorisation des requêtes** [S37].

Cette évolution a ensuite été inscrite dans le cadre réglementaire par l'arrêté du 10 juillet 2026 modifiant l'arrêté portant création de CFVR [S45].

Les données issues de la facturation électronique font donc désormais partie des catégories de données intégrées au dispositif CFVR.

La CNIL précise en outre qu'une partie des données de CFVR ainsi que les données issues de la facturation électronique doivent alimenter la plateforme sécurisée des données de la DGFiP afin d'y être exploitées, notamment en raison de leur volumétrie [S37].

Elle relève que :

> leur ajout augmente substantiellement le volume de données traitées ;

et que la volumétrie concernée est de l'ordre de :

> **2 à 3 milliards de factures électroniques par an** [S37].

Les résultats issus de l'exploitation réalisée sur cette plateforme peuvent ensuite alimenter CFVR et être rapprochés d'autres informations afin de contribuer notamment à l'identification d'anomalies et d'entreprises présentant certains risques fiscaux [S37].

**AVÉRÉ :**

> L'intégration des données issues de la facturation électronique au traitement CFVR repose désormais sur un texte réglementaire adopté [S45].

**AVÉRÉ :**

> Ces données sont destinées à être exploitées à grande échelle au sein de l'infrastructure d'analyse de données de la DGFiP pour des finalités liées au contrôle et au ciblage fiscal [S37][S45].

**GARANTIE JURIDIQUE ÉTABLIE :**

> Cette intégration ne soustrait pas les traitements réalisés aux principes applicables de finalité, minimisation, sécurité, nécessité et proportionnalité [S36][S43][S44].

---

### Les données sont croisées avec d'autres résultats d'analyse

L'avis de la CNIL apporte un second élément important.

Les données exploitées sur la plateforme doivent permettre de produire des résultats qui peuvent être croisés avec les autres informations utilisées par CFVR afin d'obtenir notamment des listes d'entreprises considérées comme présentant certains risques fiscaux [S37].

La CNIL indique également qu'à terme l'ensemble des données du traitement CFVR a vocation à alimenter la plateforme sécurisée des données.

La chaîne réellement documentée devient donc :

```
données de facturation électronique
   ↓
plateforme sécurisée des données DGFiP
   ↓
exploitation algorithmique
   ↓  
rapprochement avec d'autres données / résultats
   ↓
détection d'anomalies
   ↓
identification d'entreprises présentant certains risques
   ↓
orientation possible du contrôle fiscal
```

**AVÉRÉ :**

> Le croisement et l'analyse automatisée de données issues de la facturation électronique avec d'autres informations fiscales ne constituent plus une simple possibilité technique.

Ils font partie des usages documentés du dispositif CFVR [S37].

---

### Le traitement dépasse les seules entreprises

L'historique de CFVR décrit par la CNIL mérite également d'être relevé.

Initialement développé pour les contribuables professionnels, le dispositif a ensuite été étendu aux personnes physiques impliquées dans le fonctionnement des entreprises, puis aux particuliers [S37].

Cela ne signifie pas que chaque donnée de facturation électronique sera associée à chaque particulier.

Mais cela démontre que l'infrastructure analytique dans laquelle ces données viennent désormais s'insérer n'est pas limitée par nature aux seules personnes morales.

**POINT DE VIGILANCE :**

> L'intégration massive des données issues de la facturation électronique dans une infrastructure utilisant déjà différentes catégories de données relatives aux professionnels et aux personnes physiques renforce l'importance des règles de finalité, de minimisation, d'habilitation et de proportionnalité.

---

### Des échanges avec d'autres administrations sont également documentés

La même délibération décrit des échanges entre la DGFiP et les organismes de sécurité sociale dans le cadre de CFVR [S37].

Ces échanges disposent d'un fondement juridique spécifique et sont limités à certaines finalités.

La CNIL considère ces finalités légitimes dans le cadre juridique actuellement prévu.

**AVÉRÉ :**

> Des mécanismes juridiques permettent déjà à certaines données administratives de circuler entre organismes publics pour des finalités déterminées.

Mais la CNIL insiste précisément sur :

- la minimisation des données ;  
- la limitation aux agents habilités ;  
- le besoin d'en connaître ;  
- la durée de conservation ;  
- l'information des personnes ;  
- la proportionnalité des échanges [S37].

Cette observation est essentielle pour la suite de l'enquête.

**GARANTIE JURIDIQUE ÉTABLIE :**

> L'interconnexion entre administrations n'est pas juridiquement libre : elle doit reposer sur un fondement juridique et respecter des finalités et garanties déterminées.

---

### Première zone de vulnérabilité : l'extension progressive des finalités

La réforme repose initialement sur des objectifs notamment fiscaux : modernisation de la collecte de TVA, lutte contre la fraude, pré-remplissage et amélioration de la connaissance de l'activité économique.

L'utilisation des données pour le ciblage fiscal possède donc un lien direct avec plusieurs finalités annoncées.

**ARGUMENT INSUFFISANT À CE STADE :**

> L'utilisation actuelle des données de facturation par CFVR constituerait nécessairement un détournement de finalité.

Les sources étudiées ne permettent pas de soutenir cette conclusion.

La lutte contre la fraude et le contrôle fiscal font précisément partie du cadre dans lequel ces traitements sont organisés.

En revanche, la question deviendrait juridiquement beaucoup plus sensible si les mêmes données étaient ultérieurement réutilisées pour une finalité substantiellement différente.

Par exemple :

```
collecte pour finalité fiscale
   ↓
conservation d'une infrastructure détaillée de transactions
   ↓
réutilisation pour une autre politique publique
   ↓
rapprochement avec d'autres catégories de données
```

Une telle évolution devrait être examinée au regard de la limitation des finalités, de sa base juridique, de sa nécessité et de sa proportionnalité [S36][S43].

**VULNÉRABILITÉ POTENTIELLE :**

> La capacité technique de réutiliser les données ne constitue pas une base juridique permettant de leur attribuer librement de nouvelles finalités.

---

### Deuxième zone de vulnérabilité : la volumétrie et la proportionnalité

La CNIL constate elle-même l'augmentation substantielle du volume de données provoquée par l'intégration de la facturation électronique à CFVR [S37].

Le volume annoncé atteint plusieurs milliards de factures par an.

Or la jurisprudence relative à la protection de la vie privée et des données personnelles impose de mettre en balance :

> l'objectif d'intérêt général poursuivi

avec :

> la nature, l'étendue et la sensibilité des données traitées ainsi que la gravité de l'ingérence [S39][S44].

La question juridique pertinente n'est donc pas simplement :

> « la lutte contre la fraude est-elle un objectif légitime ? »

Elle l'est.

La question est :

> **« l'étendue précise des données collectées, leur niveau de détail, leur durée de conservation, leurs croisements et leurs modalités d'exploitation sont-ils nécessaires et proportionnés à cet objectif ? »**

C'est sur ce terrain qu'un contrôle juridique devient réellement intéressant.

---

### Troisième zone de vulnérabilité : la protection des données dès la conception et par défaut

Le principe de minimisation ne s'applique pas uniquement au choix initial des catégories de données collectées.

L'article 25 du RGPD impose également au responsable du traitement de mettre en œuvre des mesures techniques et organisationnelles permettant d'appliquer effectivement les principes de protection des données dès la conception et par défaut [S43].

Le règlement précise que cette exigence concerne notamment :

- la quantité de données personnelles collectées ;  
- l'étendue de leur traitement ;  
- leur durée de conservation ;  
- leur accessibilité.

Cette disposition est particulièrement pertinente concernant une infrastructure appelée à traiter plusieurs milliards de factures électroniques par an et à permettre leur exploitation au sein d'une plateforme disposant d'importantes capacités de calcul [S37].

La question juridique ne porte donc pas uniquement sur l'existence d'une base permettant l'intégration des données.

Elle porte également sur la conception concrète de l'infrastructure :

> quelles données sont réellement nécessaires ?

> pendant combien de temps ?

> pour quels traitements ?

> accessibles à quels agents ?

> avec quel niveau de granularité ?

> et quelles mesures empêchent techniquement leur utilisation au-delà des finalités autorisées ?

La CNIL exige précisément que la plateforme sécurisée des données conserve un cloisonnement strict, que les données qui y sont versées soient uniquement traitées pour les finalités prévues et que son utilisation n'ouvre pas l'accès à de nouveaux destinataires non prévus [S37].

**GARANTIE JURIDIQUE ÉTABLIE :**

> Le RGPD impose que la protection des données et la minimisation soient intégrées à la conception même du traitement et que, par défaut, seules les données nécessaires à chaque finalité spécifique soient traitées [S43].

**POINT DE VIGILANCE :**

> L'augmentation de la capacité technique de stockage, de calcul ou de croisement ne constitue pas en elle-même une justification permettant d'élargir les données accessibles ou les traitements réalisés.

**QUESTION JURIDIQUE À DOCUMENTER :**

> Les mesures techniques et organisationnelles effectivement mises en œuvre dans CFVR et dans la plateforme sécurisée des données permettent-elles de démontrer, pour les données issues de la facturation électronique, l'application effective des principes de minimisation et de protection des données dès la conception et par défaut ?


---

### Quatrième zone de vulnérabilité : la maîtrise des accès

La CNIL insiste également sur la nécessité de limiter les accès à un nombre restreint d'agents et au strict besoin d'en connaître [S37].

Elle demande que la plateforme sécurisée :

> conserve un cloisonnement strict des données ;

> ne permette leur traitement que pour les finalités prévues ;

> n'ouvre pas l'accès à de nouveaux destinataires non prévus.

Cette exigence est particulièrement importante pour notre enquête.

Elle signifie qu'une infrastructure techniquement capable d'accueillir plusieurs catégories de données ne peut juridiquement devenir un espace général de réutilisation sans nouvel encadrement.

**GARANTIE JURIDIQUE ÉTABLIE :**

> Le cloisonnement des finalités et des accès constitue actuellement une protection juridiquement significative contre une réutilisation généralisée des données.

**POINT DE VIGILANCE :**

> Toute extension des catégories d'accédants, des finalités ou des données croisées doit être examinée séparément afin de déterminer si le fondement juridique et les garanties existantes demeurent suffisants.

---

### Une distinction fondamentale apparaît

Le résultat de cette première analyse est différent de deux positions extrêmes.

Il serait juridiquement incorrect d'affirmer :

> **« La réforme viole le RGPD parce que les données sont transmises sans consentement. »**

Une base légale existe et le consentement n'est pas la seule base permettant un traitement.

Mais il serait également incorrect d'affirmer :

> **« Puisque la collecte est prévue par la loi, l'administration peut ensuite faire ce qu'elle souhaite avec les données. »**

Le RGPD et les exigences constitutionnelles et européennes de protection de la vie privée continuent d'encadrer :

- les finalités ;  
- les catégories de données ;  
- leur nécessité ;  
- leur proportionnalité ;  
- leur conservation ;  
- leurs destinataires ;  
- leurs croisements ;  
- les décisions automatisées ;  
- les mesures de sécurité.

---

### Première conclusion juridique

**AVÉRÉ :**

> La réforme repose sur un cadre légal et réglementaire et a fait l'objet d'une consultation de la CNIL.

**AVÉRÉ :**

> Les données issues de la facturation électronique comprennent des données personnelles soumises aux garanties du RGPD.

**AVÉRÉ :**

> Ces données sont destinées à alimenter une infrastructure de la DGFiP permettant leur exploitation algorithmique à grande échelle pour le ciblage fiscal.

**AVÉRÉ :**

> La CNIL constate elle-même une augmentation substantielle de la volumétrie et identifie des risques relatifs à la minimisation, aux accès, à la conservation, à la sécurité, aux biais algorithmiques et à l'automatisation.

**AVÉRÉ :**

> Certains échanges et croisements entre administrations sont juridiquement possibles lorsqu'un texte les prévoit et que leurs finalités sont déterminées.

**GARANTIE JURIDIQUE ÉTABLIE :**

> Une collecte légalement instituée ne permet pas une réutilisation illimitée des données pour n'importe quelle finalité.

**VULNÉRABILITÉ POTENTIELLE :**

> Toute extension substantielle des finalités, des catégories de données, des destinataires ou des mécanismes de rapprochement doit pouvoir satisfaire aux exigences de base légale, de nécessité, de minimisation et de proportionnalité.

**À ÉTABLIR :**

> L'étendue exacte des garanties entourant chacun des traitements issus de la réforme et la possibilité de contester juridiquement certaines extensions ou modalités d'exploitation doivent être examinées dans les sections suivantes.

---

### Ce que 6.1 change dans l'enquête

Un élément qui était encore partiellement ouvert dans les premiers chapitres peut désormais être précisé.

La chaîne suivante est documentée :

```
facturation électronique
   ↓
données personnelles et économiques à très grande échelle
   ↓  
plateforme sécurisée des données DGFiP
   ↓
exploitation algorithmique
   ↓
croisements / analyses
   ↓
détection d'anomalies et ciblage fiscal
   ↓
décision humaine éventuelle d'engager un contrôle
```

La question juridique n'est donc plus de savoir si les données de facturation **peuvent techniquement être exploitées et croisées à grande échelle**.

Cette exploitation est désormais documentée dans le domaine fiscal.

La question devient :

> **jusqu'où cette exploitation peut-elle juridiquement aller avant de rencontrer les principes de limitation des finalités, de minimisation, de nécessité, de proportionnalité et de protection contre certaines décisions automatisées ?**

C'est cette frontière que les sections suivantes doivent rechercher.

---

## 6.2 Finalité des traitements et réutilisation des données

**Statut : GARANTIES JURIDIQUES ÉTABLIES / LATITUDES JURIDIQUES IDENTIFIÉES / FRONTIÈRES À ÉTABLIR**

Le principe de limitation des finalités constitue l'une des principales protections juridiques applicables aux architectures étudiées dans les chapitres précédents.

Mais sa portée doit être décrite avec précision.

Une interprétation trop simple consisterait à considérer que :

> **« toute nouvelle utilisation d'une donnée pour une finalité différente de celle annoncée lors de sa collecte est interdite. »**

Le RGPD ne pose pas une interdiction aussi absolue.

Il organise au contraire plusieurs mécanismes permettant, sous conditions, certains traitements ultérieurs [S36][S43][S46].

---

### Une finalité doit être déterminée, explicite et légitime

Le principe initial reste clair.

Les données personnelles doivent être collectées pour des finalités déterminées, explicites et légitimes et ne doivent pas être traitées ultérieurement d'une manière incompatible avec ces finalités [S36][S43].

Cette règle empêche en principe qu'une infrastructure constituée pour un objectif déterminé devienne, par sa seule existence technique, une réserve générale de données utilisable pour n'importe quel objectif futur.

Elle impose donc de distinguer :

```
capacité technique de réutilisation
   ↓
finalité juridiquement définie
   ↓
base juridique
   ↓
nécessité / proportionnalité
   ↓
traitement autorisé
```

La première étape ne suffit jamais à démontrer les suivantes.

**GARANTIE JURIDIQUE :**

> La disponibilité technique d'une donnée ne constitue pas, à elle seule, une finalité ni une base juridique permettant son utilisation.

---

### Une nouvelle finalité n'est cependant pas automatiquement interdite

L'article 6, paragraphe 4 du RGPD prévoit explicitement le cas dans lequel des données sont traitées ultérieurement pour une finalité autre que celle ayant justifié leur collecte initiale [S46].

Lorsque ce traitement ultérieur ne repose ni sur le consentement de la personne concernée ni sur une disposition pertinente du droit de l'Union ou d'un État membre, le responsable du traitement doit notamment déterminer si cette nouvelle finalité est compatible avec la finalité initiale.

Le règlement prévoit plusieurs critères permettant cette appréciation :

- le lien entre la finalité initiale et la finalité ultérieure ;  
- le contexte dans lequel les données ont été collectées ;  
- la nature des données ;  
- les conséquences possibles du nouveau traitement pour les personnes ;  
- les garanties mises en œuvre, notamment le chiffrement ou la pseudonymisation [S46].

Il existe donc juridiquement un :

> **test de compatibilité des finalités.**

**LATITUDE JURIDIQUE :**

> Une donnée collectée pour une finalité déterminée peut, sous certaines conditions, faire l'objet d'un traitement ultérieur compatible avec cette finalité.

Cela signifie que :

```
nouvelle utilisation
   ≠
illégalité automatique
```

Mais également que :

```
nouvelle utilisation
   ≠
compatibilité automatique
```

La compatibilité doit être appréciée au regard du traitement effectivement envisagé.

---

### Une seconde voie existe : l'intervention du droit

L'article 6, paragraphe 4 révèle une seconde possibilité importante pour cette enquête.

Le mécanisme du test de compatibilité qu'il décrit concerne le cas dans lequel le traitement ultérieur n'est pas fondé notamment sur le droit de l'Union ou d'un État membre constituant une mesure nécessaire et proportionnée dans une société démocratique pour garantir les objectifs prévus par l'article 23 du RGPD [S46].

Autrement dit, l'évolution des usages ne dépend pas uniquement de la compatibilité avec la finalité initiale.

Le droit peut également encadrer certains nouveaux traitements ou certaines restrictions dans les conditions prévues par le RGPD.

**LATITUDE JURIDIQUE :**

> Le cadre juridique peut évoluer et permettre certains traitements ultérieurs qui ne reposent pas uniquement sur la compatibilité avec la finalité initiale.

Cette latitude est fondamentale pour l'analyse des architectures étudiées dans ce dépôt.

Une infrastructure techniquement existante peut aujourd'hui être juridiquement limitée à certaines finalités, sans que cette limitation constitue nécessairement une impossibilité juridique définitive.

Une évolution du droit pourrait modifier les traitements autorisés.

Cela ne permet cependant pas de présumer qu'une telle évolution aura lieu.

---

### Le domaine fiscal bénéficie explicitement de cette latitude

Cette possibilité n'est pas purement abstraite dans le domaine étudié.

L'article 23 du RGPD prévoit expressément que le droit de l'Union ou le droit national peut, sous certaines conditions, limiter la portée de plusieurs obligations et droits prévus par le règlement afin de garantir certains objectifs importants d'intérêt public [S47].

Parmi les domaines explicitement mentionnés figurent notamment :

- les intérêts économiques ou financiers importants ;  
- le domaine monétaire ;  
- le domaine budgétaire ;  
- le domaine fiscal ;  
- la sécurité sociale ;  
- certaines missions de contrôle, d'inspection ou de réglementation liées à l'exercice de l'autorité publique [S47].

Cette possibilité reste conditionnée.

La mesure doit notamment :

> respecter l'essence des libertés et droits fondamentaux ;

et :

> être nécessaire et proportionnée dans une société démocratique [S47].

**GARANTIE JURIDIQUE :**

> Le RGPD n'autorise pas une restriction générale et sans contrôle des droits au nom de l'intérêt fiscal.

**LATITUDE JURIDIQUE :**

> Le RGPD prévoit explicitement la possibilité pour le législateur d'aménager certaines protections ou certains droits lorsque des objectifs fiscaux ou des missions de contrôle le justifient, sous réserve notamment des exigences de nécessité et de proportionnalité.

---

### Cette latitude est déjà utilisée dans le cadre CFVR

Le lien avec l'enquête devient particulièrement concret dans l'arrêté du 10 juillet 2026 modifiant CFVR [S45][S47].

Cet arrêté :

- intègre les données issues de la facturation électronique parmi les données traitées ;  
- étend ou précise plusieurs sources de données utilisées par le dispositif ;  
- organise certains accès et transmissions ;  
- et fait explicitement référence aux points e) et h) du paragraphe 1 de l'article 23 du RGPD [S45][S47].

Il ne s'agit donc pas seulement d'une possibilité théorique contenue dans le règlement européen.

Le cadre réglementaire actuel de CFVR mobilise déjà les mécanismes juridiques permettant certaines limitations dans le contexte fiscal et des missions de contrôle.

**AVÉRÉ :**

> Le cadre juridique de CFVR fait explicitement référence aux possibilités de limitation prévues par l'article 23 du RGPD pour certains objectifs d'intérêt public et certaines missions de contrôle [S45][S47].

---

### Le droit peut donc déplacer la frontière sans supprimer toutes les garanties

Cette observation conduit à une distinction importante.

Il serait incorrect d'écrire :

> **« Les finalités annoncées aujourd'hui interdisent définitivement toute nouvelle utilisation future. »**

Le droit peut évoluer.

Il serait tout aussi incorrect d'écrire :

> **« Il suffit d'adopter un nouveau texte pour rendre juridiquement possible n'importe quelle utilisation des données. »**

Les nouvelles dispositions restent elles-mêmes soumises aux normes juridiques supérieures applicables.

Selon les situations, cela peut notamment inclure :

- le RGPD ;  
- la Charte des droits fondamentaux de l'Union européenne ;  
- le droit au respect de la vie privée ;  
- le contrôle de nécessité ;  
- le contrôle de proportionnalité ;  
- le principe de minimisation ;  
- les garanties applicables aux personnes concernées [S39][S43][S44][S46][S47].

La véritable frontière n'est donc pas :

```
possible
   /
impossible
```

mais plutôt :

```
usage actuellement autorisé
   ↓
extension envisagée
   ↓
compatibilité éventuelle
   ou
nouvelle base juridique
   ↓
contrôle de nécessité
   ↓
contrôle de proportionnalité
   ↓
garanties applicables
```

---

### Première vulnérabilité juridique : l'extension progressive peut être légale

Cette conclusion fait apparaître une vulnérabilité particulière.

Elle ne résulte pas nécessairement d'une violation du droit.

Elle résulte au contraire de la capacité du droit à faire évoluer progressivement le périmètre des traitements autorisés.

Une infrastructure peut ainsi connaître successivement :

```
finalité A
   ↓
extension compatible A → A+
   ↓
nouveau fondement juridique
   ↓
extension vers B
   ↓
nouveaux rapprochements autorisés
```

Chaque étape peut être juridiquement encadrée et pourtant conduire, dans le temps, à une architecture dont le périmètre est beaucoup plus large que lors de sa création.

**VULNÉRABILITÉ JURIDIQUE :**

> La limitation des finalités constitue une protection contre les réutilisations incompatibles non suffisamment fondées, mais elle ne garantit pas l'immuabilité du périmètre juridique d'un traitement.

**IMPORTANT :**

> Cette possibilité d'évolution ne démontre ni qu'une extension particulière est envisagée ni qu'elle serait juridiquement admissible.

Elle démontre seulement que :

> **la frontière juridique peut évoluer sans nécessiter de modifier l'architecture technique déjà disponible.**

---

### Deuxième vulnérabilité : l'accumulation des extensions

L'analyse juridique d'une extension est généralement effectuée au regard d'un traitement et d'une finalité déterminés.

Mais l'enquête étudie également l'effet cumulé de plusieurs infrastructures et évolutions successives.

Une succession d'extensions individuellement justifiées peut progressivement augmenter :

- le nombre de données disponibles ;  
- le nombre de sources ;  
- le nombre de rapprochements possibles ;  
- le nombre de destinataires ;  
- la durée pendant laquelle certaines informations demeurent exploitables ;  
- la capacité de profilage ou d'analyse.

La question devient alors :

> **à quel moment l'effet cumulé de plusieurs extensions juridiquement fondées modifie-t-il suffisamment la nature ou l'intensité du traitement pour imposer une nouvelle appréciation de nécessité et de proportionnalité ?**

**À ÉTABLIR :**

> Dans quelle mesure le droit applicable impose-t-il de réévaluer la proportionnalité non seulement de chaque extension prise isolément, mais également de l'architecture résultant de leur accumulation ?

Cette question devra être rapprochée des analyses de nécessité, de proportionnalité et d'impact étudiées dans les sections suivantes.

---

### Une frontière essentielle pour les interconnexions du Chapitre 5

Cette analyse permet également de conserver une frontière méthodologique essentielle concernant les chaînes étudiées précédemment.

Le Chapitre 5 a identifié plusieurs capacités techniques ou expérimentales reliant notamment :

```
transaction
   ↓
produit
   ↓
DPP
   ↓
données environnementales
```

ainsi que :

```
données externes
   ↓
condition
   ↓
paiement conditionnel
```

L'existence du mécanisme de traitement ultérieur prévu par le RGPD ne permet pas de transformer ces possibilités techniques en usages juridiquement autorisés.

Elle ne permet pas davantage de conclure qu'une future base juridique sera créée pour les relier.

**NON ÉTABLI :**

> Aucun élément étudié dans cette section n'établit que les données environnementales du DPP puissent actuellement être utilisées afin de déterminer l'autorisation, le refus ou la limitation d'un paiement.

**DÉDUCTIBLE JURIDIQUEMENT :**

> Si une telle interconnexion impliquant des données personnelles devait être mise en œuvre, sa conformité devrait être examinée au regard de sa finalité, de sa base juridique et des garanties applicables, ainsi que, selon le mécanisme retenu, des exigences de nécessité, de proportionnalité et de minimisation.

Cette distinction empêche de confondre :

```
évolution juridiquement possible en théorie
   ↓
   et
usage juridiquement autorisé aujourd'hui
```

---

### Conclusion de 6.2

**AVÉRÉ :**

> Le RGPD interdit les traitements ultérieurs incompatibles avec les finalités initiales lorsqu'aucun autre fondement pertinent ne permet le traitement [S36][S43][S46].

**AVÉRÉ :**

> Le RGPD prévoit un mécanisme permettant d'évaluer la compatibilité d'une finalité ultérieure avec la finalité initiale [S46].

**AVÉRÉ :**

> Le droit de l'Union ou le droit national peut également prévoir certaines limitations ou certains traitements dans les conditions prévues par le RGPD, notamment pour des objectifs importants relevant du domaine fiscal et pour certaines missions de contrôle [S46][S47].

**AVÉRÉ :**

> Le cadre CFVR modifié en juillet 2026 fait explicitement référence aux points e) et h) de l'article 23, paragraphe 1 du RGPD [S45][S47].

**GARANTIE JURIDIQUE :**

> Une extension des usages ne devient pas licite du seul fait qu'elle est techniquement possible ou qu'elle poursuit un objectif d'intérêt général.

**LATITUDE JURIDIQUE :**

> Le droit permet néanmoins certaines réutilisations compatibles et peut faire évoluer le périmètre des traitements autorisés, sous réserve des conditions et garanties applicables.

**VULNÉRABILITÉ JURIDIQUE :**

> La limitation des finalités protège contre certaines réutilisations, mais ne fige pas définitivement le périmètre juridique d'une infrastructure de données.

**À ÉTABLIR :**

> Jusqu'où des extensions successives de finalités, de sources de données et de destinataires peuvent-elles s'accumuler avant que leur effet global impose une nouvelle appréciation de nécessité et de proportionnalité ?

**NON ÉTABLI :**

> Rien dans les sources étudiées ici ne démontre qu'une évolution juridique soit actuellement envisagée afin de relier les données environnementales du DPP à l'autorisation, au refus ou à la limitation d'un paiement.

---

## 6.3 Croisement, rapprochement et interconnexion des données

**Statut : INTERCONNEXIONS AVÉRÉES / GARANTIES DOCUMENTÉES / VULNÉRABILITÉS ET ANGLES MORTS IDENTIFIÉS**

Les chapitres précédents ont montré que plusieurs infrastructures étudiées disposent de capacités de rapprochement ou d'interconnexion.

Dans le domaine fiscal, cette question n'est désormais plus seulement technique.

Le traitement CFVR constitue déjà une architecture alimentée par de nombreuses sources de données et permettant leur analyse ou leur rapprochement [S37][S45].

L'enjeu juridique devient donc double :

> **quelles interconnexions sont effectivement autorisées ?**

et :

> **quelles garanties empêchent qu'une infrastructure de rapprochement de données à grande échelle devienne elle-même une source disproportionnée de risque, notamment en cas de compromission, de mésusage ou d'extension des accès ?**

---

### CFVR constitue déjà une infrastructure multi-sources

L'arrêté modifiant CFVR en juillet 2026 ne se limite pas à l'ajout des données issues de la facturation électronique [S45].

Le traitement est alimenté par de nombreuses autres sources.

La liste réglementaire comprend notamment des données issues :

- des dossiers fiscaux ;  
- des déclarations fiscales ;  
- du prélèvement à la source ;  
- des données foncières et d'occupation des logements ;  
- des successions ;  
- des coordonnées de comptes bancaires déclarées par les foyers fiscaux ;  
- des paiements transfrontaliers enregistrés dans CESOP ;  
- de la TVA intracommunautaire ;  
- des échanges de biens au sein de l'Union européenne ;  
- des traitements relatifs aux quittus automobiles ;  
- de traitements de données provenant d'organismes sociaux ;  
- de données publiquement accessibles collectées sur certaines plateformes en ligne ;  
- et désormais de la facturation électronique [S45].

L'arrêté prévoit également des données concernant des personnes physiques nécessaires à certains travaux portant sur l'intensité de l'activité économique [S45].

**AVÉRÉ :**

> CFVR n'est pas une base limitée aux seules données issues de la facturation électronique.

Il constitue une infrastructure analytique alimentée par un ensemble beaucoup plus large de sources fiscales, économiques, administratives et, dans certains cas, relatives à des personnes physiques.

---

### Le croisement est une fonction documentée du dispositif

La CNIL décrit explicitement le fonctionnement prévu pour les nouvelles données de facturation électronique [S37].

Une partie des données de CFVR ainsi que les données issues de la facturation électronique doivent alimenter la plateforme sécurisée des données de la DGFiP.

Les résultats des requêtes effectuées sur cette plateforme peuvent ensuite être croisés avec les données provenant de CFVR afin d'obtenir notamment des listes d'entreprises considérées comme présentant certains risques.

À terme :

> **l'ensemble des données de CFVR a vocation à alimenter cette plateforme** [S37].

La chaîne documentée devient donc :

```
multiples sources administratives / fiscales
   ↓
CFVR
   ↓
données de facturation électronique
   +
autres données CFVR
   ↓
plateforme sécurisée des données
   ↓
requêtes / modèles / analyses
   ↓
croisement de résultats
   ↓
détection d'anomalies
   ↓
sélection de dossiers présentant certains risques
```

**AVÉRÉ :**

> Le rapprochement de plusieurs ensembles de données constitue une fonction effective et réglementairement organisée de CFVR [S37][S45].

Il ne s'agit donc plus seulement d'une interconnexion techniquement envisageable.

---

### Les échanges entre administrations élargissent encore le périmètre

Les interconnexions documentées dépassent également la seule DGFiP.

L'article L. 152 du livre des procédures fiscales permet certains échanges entre l'administration fiscale et les organismes de sécurité sociale.

Le dispositif CFVR a été adapté en conséquence [S37][S45].

Les données peuvent être transmises aux organismes sociaux pour certaines missions de contrôle de l'assiette des cotisations.

En sens inverse, certaines données communiquées par ces organismes peuvent également alimenter CFVR.

La CNIL mentionne notamment des informations relatives :

- au travail dissimulé ;  
- aux rémunérations ;  
- aux résultats de contrôles fiscaux [S37].

**AVÉRÉ :**

> Il existe donc une circulation juridiquement organisée dans les deux sens entre l'administration fiscale et certains organismes sociaux.

Cette circulation repose sur une base légale et sur des finalités déterminées.

---

### Le périmètre des personnes ayant accès au système évolue également

L'arrêté de juillet 2026 prévoit plusieurs catégories d'agents habilités pouvant accéder aux données nécessaires aux travaux de modélisation et de visualisation [S45].

Il comprend notamment des agents appartenant :

- au réseau national d'analyse de données ;  
- aux structures de programmation interrégionales ;  
- à certains services nationaux spécialisés ;  
- à des directions départementales des finances publiques ;  
- à la direction nationale des enquêtes fiscales.

Les résultats utiles sont également accessibles, dans la limite du besoin d'en connaître, à certains agents chargés de la gestion, de la programmation et du contrôle des dossiers ainsi qu'à certains agents habilités des organismes de sécurité sociale [S45].

La CNIL indique que les membres du réseau national doivent être individuellement habilités, formés et supervisés et que certaines requêtes peuvent être validées ou refusées par le bureau compétent [S37].

**GARANTIE JURIDIQUE ET ORGANISATIONNELLE :**

> Les accès ne sont pas présentés comme ouverts indistinctement à l'ensemble des agents publics.

Ils reposent sur des habilitations et doivent être limités au besoin d'en connaître [S37][S45].

---

### Le croisement à grande échelle constitue lui-même un facteur de risque reconnu

Cette architecture doit cependant être rapprochée des critères utilisés par la CNIL en matière d'analyse d'impact.

Parmi les critères permettant d'identifier des traitements susceptibles d'engendrer un risque élevé figurent notamment :

- le traitement à grande échelle ;  
- le croisement ou la combinaison d'ensembles de données ;  
- l'évaluation ou le scoring ;  
- l'usage de technologies ou méthodes innovantes [S49].

CFVR présente publiquement plusieurs caractéristiques correspondant à ces critères :

```
volume massif
   +
croisements de données
   +
analyse / ciblage
   +
méthodes algorithmiques
```

La CNIL constate elle-même que l'arrivée de la facturation électronique augmente **substantiellement** le volume de données traitées et évoque plusieurs milliards de factures par an [S37].

**POINT DE VIGILANCE MAJEUR :**

> L'augmentation simultanée de la volumétrie, du nombre de sources et des capacités de rapprochement augmente non seulement la puissance analytique du système, mais également les conséquences potentielles d'une erreur, d'un mésusage ou d'une compromission.

---

### Première vulnérabilité : la concentration accroît l'impact potentiel d'une compromission

Une base ou une plateforme capable de rapprocher de nombreuses catégories de données présente un risque différent de plusieurs bases strictement cloisonnées.

Une compromission ne porterait plus nécessairement sur une seule information isolée.

Selon les accès effectivement obtenus, elle pourrait permettre de rapprocher plusieurs catégories d'informations.

Le RGPD impose précisément que le niveau de sécurité soit adapté :

- à la nature des données ;  
- à leur portée ;  
- au contexte du traitement ;  
- à la probabilité du risque ;  
- à sa gravité [S48].

La CNIL va ici beaucoup plus loin qu'une formule générale.

Dans son avis concernant CFVR, elle relève explicitement :

> le volume massif des données ;

> leur sensibilité ;

> l'évolution de la menace ;

> et l'évolution des modes opératoires d'attaque informatique [S37].

**VULNÉRABILITÉ JURIDIQUE ET TECHNIQUE :**

> Plus l'architecture concentre des données, des sources et des possibilités de rapprochement, plus le niveau de sécurité qui peut raisonnablement être exigé augmente.

Cela ne signifie pas que CFVR est actuellement compromis ou insuffisamment sécurisé.

Cela signifie que :

> **le changement d'échelle modifie également le niveau de risque dont l'administration doit pouvoir démontrer la maîtrise.**

---

### La CNIL demande elle-même des protections renforcées contre les accès compromis

L'avis de la CNIL apporte ici un élément particulièrement concret [S37].

Elle accueille favorablement l'engagement du ministère de systématiser :

- la double authentification ;  
- l'accès uniquement depuis des terminaux sécurisés.

Mais la CNIL va plus loin concernant les journaux de connexion et d'activité.

Elle considère que la journalisation doit s'accompagner de mécanismes permettant notamment :

- une analyse proactive des événements ;  
- la détection de comportements inattendus ;  
- la génération d'alertes ;  
- le blocage immédiat des comptes concernés jusqu'à la levée du doute par la hiérarchie [S37].

**GARANTIE DOCUMENTÉE :**

> La double authentification et l'utilisation de terminaux sécurisés font l'objet d'un engagement du ministère relevé positivement par la CNIL.

**ANGLE MORT DOCUMENTAIRE :**

> Dans son avis publié en 2026, la CNIL invite spécifiquement le ministère à mettre en œuvre des mécanismes proactifs d'analyse des journaux, d'alerte et de blocage des comptes en cas de comportement inattendu.

Les sources publiques étudiées ici ne permettent pas encore d'établir si l'ensemble de ces mécanismes recommandés est effectivement déployé sur tous les environnements concernés.

**À ÉTABLIR :**

> Les mécanismes proactifs de détection et de blocage demandés par la CNIL ont-ils depuis été effectivement déployés, avec quelle couverture et selon quelles procédures ?

Voilà une question très concrète qui peut être adressée à l'administration.

---

### Deuxième vulnérabilité : le risque ne provient pas uniquement d'une attaque extérieure

La sécurité d'une infrastructure de cette nature ne concerne pas uniquement un pirate obtenant un accès depuis Internet.

L'article 32 du RGPD couvre également les risques d'accès ou de divulgation non autorisés [S48].

La maîtrise des habilitations devient donc fondamentale.

Une infrastructure réunissant :

```text
plus de données
   +
plus de sources
   +
plus d'analyses
   +
plusieurs catégories d'accédants
```

augmente mécaniquement le nombre de situations dans lesquelles une habilitation erronée, un compte compromis, une mauvaise configuration ou un usage abusif pourrait avoir des conséquences importantes.

C'est précisément pour cette raison que la CNIL insiste sur :

- la limitation du nombre d'agents ;  
- l'habilitation individuelle ;  
- le strict besoin d'en connaître ;  
- la supervision ;  
- la journalisation ;  
- l'analyse des comportements [S37][S50].

**VULNÉRABILITÉ :**

> La sécurité du système dépend non seulement de la protection de son périmètre informatique mais également de la qualité permanente de la gestion des identités, des habilitations et de la détection des usages anormaux.

---

### Troisième vulnérabilité : l'interconnexion étend la surface de confiance

Les échanges avec d'autres administrations ajoutent une autre dimension.

La CNIL prend acte de l'utilisation d'un outil sécurisé de transfert de fichiers avec chiffrement conforme à l'état de l'art pour les échanges avec les organismes sociaux [S37].

C'est une garantie importante.

Mais une interconnexion crée nécessairement plusieurs environnements impliqués :

```
organisme A
   ↓
mécanisme de transfert
   ↓
organisme B
```

La sécurité globale ne dépend donc plus uniquement de l'infrastructure initiale.

Elle dépend également :

- des habilitations de chaque organisme ;  
- de la sécurité des équipements de chaque organisme ;  
- des copies éventuellement produites ;  
- des durées de conservation ;  
- de la suppression effective ;  
- de la journalisation ;  
- de la capacité de détecter un usage ou un transfert anormal.

**GARANTIE DOCUMENTÉE :**

> Les échanges DGFiP / organismes sociaux doivent utiliser un mécanisme de transfert sécurisé et chiffré [S37].

**VULNÉRABILITÉ STRUCTURELLE :**

> Toute multiplication des destinataires ou des environnements dans lesquels les données sont accessibles étend la surface sur laquelle les garanties de confidentialité, d'intégrité et de contrôle des accès doivent être maintenues.

Il ne s'agit pas d'une preuve de faiblesse actuelle d'un organisme déterminé.

Il s'agit d'une conséquence de l'architecture distribuée elle-même.

---

### Un angle mort très concret apparaît sur la conservation des données échangées

L'avis de la CNIL contient une observation particulièrement intéressante concernant les échanges avec les organismes sociaux [S37].

La Commission constate que le projet d'arrêté qui lui avait été soumis :

> **ne précisait pas la durée de conservation des données transmises dans le cadre de ces communications.**

Elle rappelle alors que les échanges entre administrations ne sont permis que si leurs modalités restent proportionnées aux objectifs poursuivis et insiste sur la nécessité de limiter la conservation à la durée nécessaire [S37].

**ANGLE MORT DOCUMENTAIRE IDENTIFIÉ :**

> Le texte soumis à la CNIL ne déterminait pas lui-même la durée de conservation des données transférées entre la DGFiP et les organismes de sécurité sociale.

Cela ne démontre pas que les données sont conservées sans limite.

Des durées peuvent être prévues dans d'autres textes, conventions, politiques internes ou traitements destinataires.

Mais cela produit une question juridiquement vérifiable :

**À ÉTABLIR :**

> Pour chaque catégorie de données transférée entre CFVR et les organismes sociaux, quelle est la durée maximale de conservation applicable chez le destinataire, par quel texte ou document est-elle déterminée, et comment sa suppression effective est-elle contrôlée ?

Ce point peut être beaucoup plus intéressant qu'une critique générale de la conservation.

---

### Quatrième vulnérabilité : une modification du risque peut imposer une nouvelle appréciation

Le RGPD contient un mécanisme particulièrement pertinent pour suivre l'évolution de ce type d'architecture.

L'article 35 prévoit que, lorsqu'une analyse d'impact existe, le responsable du traitement doit réexaminer si le traitement demeure conforme à cette analyse lorsqu'une modification du risque intervient [S48].

Or plusieurs transformations sont maintenant documentées :

- arrivée d'une nouvelle catégorie massive de données ;  
- plusieurs milliards de factures supplémentaires ;  
- utilisation d'une infrastructure de calcul renforcée ;  
- croisement avec d'autres informations ;  
- développement de nouvelles méthodes d'apprentissage ;  
- extension organisationnelle du réseau d'analyse ;  
- nouvelles relations avec des organismes sociaux [S37][S45].

**QUESTION JURIDIQUE MAJEURE :**

> Ces évolutions ont-elles été intégrées à une AIPD existante ou ont-elles donné lieu à une nouvelle analyse ou à une réévaluation formelle du risque conformément à l'article 35 du RGPD ?

Les sources publiques étudiées ne permettent pas, à ce stade, de répondre complètement à cette question.

**ANGLE MORT DOCUMENTAIRE :**

> L'existence possible d'une AIPD interne ne doit pas être confondue avec son absence. En revanche, nous ne disposons pas encore d'un document public permettant d'établir précisément quelle analyse d'impact couvre l'ensemble de la chaîne CFVR + PSD + facturation électronique + nouveaux croisements + échanges inter-administrations.

Cette distinction est essentielle.

---

### Une AIPD serait particulièrement pertinente au regard des critères de la CNIL

Sans préjuger de l'analyse juridique déjà réalisée par la DGFiP, plusieurs critères de risque élevé décrits par la CNIL apparaissent objectivement dans la documentation publique [S37][S49] :

```
traitement à grande échelle        ✓

croisement d'ensembles de données  ✓

évaluation / ciblage               ✓

méthodes algorithmiques            ✓
```

La présence de ces caractéristiques rend particulièrement importante la possibilité de vérifier :

- la description exacte du traitement étudié dans l'AIPD ;  
- les catégories de données couvertes ;  
- les interconnexions prises en compte ;  
- les risques de compromission ;  
- les risques liés aux habilitations ;  
- les risques de corrélation excessive ;  
- les mesures de réduction de ces risques ;  
- les modifications successives de l'analyse.

**À ÉTABLIR :**

> Quelle AIPD couvre aujourd'hui l'exploitation des données de facturation électronique dans CFVR et la PSD ?

> Quelle est sa date de dernière révision ?

> Intègre-t-elle l'arrivée de plusieurs milliards de factures par an ?

> Intègre-t-elle les croisements réalisés sur la PSD ?

> Intègre-t-elle les échanges avec les organismes sociaux ?

> Intègre-t-elle l'évolution des méthodes algorithmiques et l'élargissement du réseau d'analystes ?

---

### Cinquième vulnérabilité : le cloisonnement devient une garantie critique

La CNIL impose une condition particulièrement forte concernant la plateforme sécurisée des données [S37].

Elle considère que son utilisation suppose :

- un cloisonnement strict ;  
- que les données versées soient uniquement traitées pour les finalités actuellement prévues ;  
- qu'aucun nouvel accédant non prévu ne puisse y accéder ;  
- que les protections techniques soient équivalentes à celles existant hors de la PSD.

Cette formulation montre que le cloisonnement n'est pas une question accessoire.

Il constitue l'une des garanties permettant que la concentration technique ne conduise pas à une ouverture fonctionnelle des données.

**GARANTIE JURIDIQUE ET TECHNIQUE :**

> La PSD ne doit pas devenir, du seul fait qu'elle accueille plusieurs ensembles de données, une infrastructure permettant leur utilisation générale par des utilisateurs ou pour des finalités non autorisés.

**VULNÉRABILITÉ POTENTIELLE :**

> La solidité juridique de l'architecture dépend donc directement de garanties techniques de cloisonnement qui ne sont pas entièrement vérifiables depuis la documentation publique étudiée.

**À ÉTABLIR :**

> Comment les séparations entre jeux de données, finalités, traitements et profils d'accès sont-elles techniquement implémentées et auditées dans la PSD ?

---

### Le problème de sécurité ne peut donc pas être réduit à « tout peut être piraté »

Il serait trop faible juridiquement d'affirmer :

> **« Tout système informatique peut être piraté, donc cette architecture est dangereuse. »**

Le risque zéro n'existe pas et le RGPD n'exige pas l'impossibilité absolue d'une compromission.

L'exigence juridique est différente.

Elle porte sur l'adéquation entre :

```
niveau de risque
   ↓
mesures mises en œuvre
   ↓
état de l'art
   ↓
surveillance
   ↓
réévaluation régulière
   ↓
capacité à démontrer la conformité
```

[S48][S50]

C'est donc sur ce terrain que l'analyse doit se placer.

---

### Ce que 6.3 permet déjà de faire relever

Plusieurs questions précises peuvent maintenant être adressées à la DGFiP, à la CNIL ou au législateur :

> **1. Quelle AIPD couvre actuellement CFVR après l'intégration de la facturation électronique et son exploitation dans la PSD ?**

> **2. Quand cette AIPD a-t-elle été réévaluée pour la dernière fois au regard du changement massif de volumétrie et des nouvelles interconnexions ?**

> **3. Les mécanismes proactifs de détection des comportements anormaux et de blocage immédiat des comptes recommandés par la CNIL sont-ils intégralement déployés ?**

> **4. Quelle durée maximale de conservation s'applique aux données transférées entre la DGFiP et chaque organisme de sécurité sociale ?**

> **5. Comment la suppression effective des copies reçues par les organismes destinataires est-elle contrôlée ?**

> **6. Comment le cloisonnement entre jeux de données, finalités et catégories d'utilisateurs est-il techniquement garanti et audité dans la PSD ?**

> **7. Quels audits indépendants ou tests réguliers permettent de démontrer que le niveau de sécurité demeure adapté à l'évolution des menaces ?**

Ces questions ne présument aucune violation.

Elles demandent la démonstration des garanties que le droit rend précisément pertinentes.

---

### Conclusion de 6.3

**AVÉRÉ :**

> CFVR rapproche déjà de nombreuses sources fiscales, économiques, administratives et sociales et intègre désormais les données issues de la facturation électronique [S37][S45].

**AVÉRÉ :**

> Les données de facturation électronique doivent être exploitées dans la PSD et leurs résultats peuvent être croisés avec d'autres informations utilisées par CFVR [S37].

**AVÉRÉ :**

> Des échanges bidirectionnels de certaines données sont juridiquement organisés entre la DGFiP et des organismes de sécurité sociale [S37][S45].

**AVÉRÉ :**

> La CNIL considère explicitement que le volume massif, la sensibilité des données et l'évolution des modes d'attaque informatique imposent une vigilance particulière [S37].

**GARANTIE JURIDIQUE :**

> Le RGPD impose un niveau de sécurité adapté au risque ainsi qu'une réévaluation lorsque l'évolution des opérations entraîne une modification du risque [S48].

**GARANTIE DOCUMENTÉE :**

> La CNIL relève notamment des engagements concernant la double authentification, les terminaux sécurisés, le cloisonnement et la limitation des habilitations [S37].

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas encore d'établir si toutes les mesures proactives de détection et de blocage recommandées par la CNIL ont effectivement été déployées.

**ANGLE MORT DOCUMENTAIRE :**

> Le projet examiné par la CNIL ne précisait pas la durée de conservation des données transmises aux organismes sociaux ; il reste à établir précisément le régime applicable à chaque copie détenue par les destinataires [S37].

**ANGLE MORT DOCUMENTAIRE :**

> Nous n'avons pas encore identifié une AIPD publique permettant de vérifier précisément comment l'ensemble des évolutions CFVR + PSD + facturation électronique + nouveaux croisements + échanges inter-administrations a été évalué.

**VULNÉRABILITÉ JURIDIQUE :**

> L'accroissement simultané de la volumétrie, du nombre de sources, des capacités de rapprochement et des catégories d'accédants augmente les conséquences potentielles d'une compromission ou d'un mésusage et renforce donc les exigences de sécurité, de cloisonnement et de réévaluation du risque.

**À ÉTABLIR :**

> L'administration peut-elle démontrer que les mesures techniques, organisationnelles et les analyses d'impact ont été réévaluées à la hauteur du changement d'échelle introduit en 2026 ?

**NON ÉTABLI :**

> Aucun élément identifié ne permet d'affirmer que CFVR ou la PSD ont subi une compromission ou que les mesures de sécurité actuellement déployées seraient juridiquement insuffisantes.

---

## 6.4 Profilage et décisions automatisées

**Statut : TRAITEMENTS ALGORITHMIQUES AVÉRÉS / GARANTIE HUMAINE DOCUMENTÉE / FRONTIÈRE JURIDIQUE IDENTIFIÉE / VULNÉRABILITÉS À ÉTABLIR**

Les sections précédentes ont établi que les données issues de la facturation électronique doivent être exploitées à grande échelle, croisées avec d'autres informations et utilisées dans un traitement permettant notamment d'identifier des anomalies et des entreprises présentant certains risques fiscaux [S37][S45].

Cette architecture conduit directement à une question juridique supplémentaire :

> **à partir de quel moment un traitement qui analyse, classe ou sélectionne des personnes ou entreprises cesse-t-il d'être une simple aide à la décision et devient-il suffisamment déterminant pour relever des protections applicables aux décisions automatisées ?**

Cette frontière est particulièrement importante parce que le droit européen ne regarde pas uniquement l'existence formelle d'un algorithme.

Il s'intéresse également à son rôle concret dans la décision qui en résulte.

---

### Profilage et décision automatisée ne sont pas synonymes

Une première distinction doit être conservée.

Le profilage consiste à utiliser des données personnelles afin d'évaluer certains aspects personnels concernant une personne physique.

Une décision automatisée peut être fondée sur un profilage, mais les deux notions ne se confondent pas [S36][S43].

Un traitement peut donc :

```
analyser des données
   ↓
produire un score / signal / classification
   ↓
sans prendre lui-même
une décision produisant un effet juridique
```

Inversement, une décision peut être entièrement automatisée sans nécessairement reposer sur un profilage préalable.

**GARANTIE MÉTHODOLOGIQUE :**

> L'existence d'algorithmes, de modèles ou de classifications ne suffit pas, à elle seule, à démontrer l'existence d'une décision individuelle automatisée interdite ou spécialement encadrée par l'article 22 du RGPD.

---

### L'article 22 fixe cependant une frontière importante

L'article 22 du RGPD reconnaît à la personne concernée le droit de ne pas faire l'objet d'une décision fondée exclusivement sur un traitement automatisé, y compris le profilage, lorsque cette décision :

- produit des effets juridiques la concernant ;  
- ou l'affecte de manière significative de façon similaire [S36][S43].

Des exceptions existent.

Une telle décision peut notamment être autorisée lorsqu'elle est prévue par le droit de l'Union ou d'un État membre et que des mesures appropriées protègent les droits, libertés et intérêts légitimes des personnes [S43].

Le principe n'est donc pas :

```
algorithme
   =
interdiction
```

La question juridique est plus précise :

```
traitement automatisé
   ↓
décision
   ↓
caractère exclusivement automatisé
   ↓
effet juridique ou significatif
   ↓
article 22
```

---

### CFVR se situe actuellement en amont de cette frontière selon le dispositif documenté

La documentation publique relative à CFVR contient ici une garantie particulièrement importante.

La CNIL indique que le traitement a pour objet :

> d'orienter et d'éclairer l'analyse des agents,

et précise que :

> **les agents seuls peuvent décider d'engager une procédure de contrôle fiscal** [S37].

Elle insiste à nouveau sur cette séparation lors de l'examen des méthodes algorithmiques.

Les signalements générés par CFVR doivent demeurer un outil permettant aux agents d'apprécier l'opportunité d'ouvrir ou non un contrôle.

Ils ne doivent pas remplacer leur analyse [S37].

**AVÉRÉ :**

> Le fonctionnement juridiquement et organisationnellement documenté de CFVR ne prévoit pas qu'un algorithme décide seul de l'ouverture d'un contrôle fiscal.

**GARANTIE JURIDIQUE ET ORGANISATIONNELLE :**

> Une analyse humaine doit intervenir avant l'ouverture du contrôle.

Cette garantie interdit donc d'affirmer, sur la base des sources actuellement disponibles :

> **« CFVR ouvre automatiquement les contrôles fiscaux. »**

Cette affirmation n'est pas établie.

---

### Mais la CNIL considère elle-même cette intervention humaine comme indispensable

La formulation utilisée par la CNIL est particulièrement importante.

Elle considère :

> **indispensable à l'équilibre du dispositif**

que les signalements générés ne puissent en aucun cas remplacer l'analyse réalisée par les agents [S37].

Elle demande également au ministère de garantir :

> **une surveillance et une décision humaine effectives** [S37].

Elle recommande notamment :

- une documentation adaptée pour les analystes ;  
- des formations régulières ;  
- une analyse fiscale des pièces de chaque dossier ;  
- la prise en compte des dernières déclarations disponibles [S37].

La CNIL qualifie ces mesures d'essentielles pour prévenir :

> **l'automatisation de l'ouverture des contrôles fiscaux** [S37].

Cette formulation révèle une frontière juridique et organisationnelle très claire.

```
CFVR
   ↓
signalement algorithmique
   ↓
ANALYSE HUMAINE EFFECTIVE
   ↓
décision éventuelle
```

La solidité de la garantie dépend donc de ce qui se passe réellement dans l'étape centrale.

---

### SCHUFA empêche de réduire la question à la présence formelle d'un humain

La jurisprudence de la Cour de justice apporte ici un élément majeur.

Dans l'affaire SCHUFA, la Cour devait examiner un système dans lequel une société produisait automatiquement une valeur de probabilité concernant une personne, puis transmettait cette valeur à un tiers qui prenait formellement la décision finale [S51].

Il existait donc bien deux étapes :

```
système automatisé
   ↓
score
   ↓
tiers
   ↓
décision
```

La Cour a néanmoins considéré que l'établissement automatisé du score pouvait constituer lui-même une décision individuelle automatisée au sens de l'article 22 lorsque la décision du tiers dépendait **de manière déterminante** de cette valeur [S51].

**PRINCIPE JURISPRUDENTIEL :**

> L'existence d'un décideur humain ou d'un tiers en bout de chaîne ne suffit donc pas nécessairement à exclure l'article 22 lorsque le résultat automatisé joue en pratique un rôle déterminant dans la décision finale.

Cette jurisprudence ne concernait pas CFVR et ne permet pas de transposer automatiquement sa conclusion au contrôle fiscal.

Mais elle fournit un critère particulièrement pertinent pour examiner ce type d'architecture.

---

### Première vulnérabilité juridique : l'intervention humaine doit être réelle, pas seulement formelle

La question concernant CFVR devient donc plus précise.

Elle n'est pas seulement :

> **« un humain clique-t-il sur le bouton final ? »**

Elle est :

> **« cet humain dispose-t-il réellement des informations, du temps, de la compétence et de l'autonomie nécessaires pour remettre en cause le signal produit par le système ? »**

La CNIL semble elle-même identifier cette difficulté puisqu'elle demande une surveillance et une décision humaine **effectives** [S37].

**VULNÉRABILITÉ JURIDIQUE :**

> Si l'analyse humaine devenait purement formelle et que les signalements algorithmiques déterminaient en pratique l'ouverture des contrôles, la qualification juridique du processus devrait être réexaminée au regard notamment de l'article 22 et de la jurisprudence SCHUFA [S43][S51].

**NON ÉTABLI :**

> Les sources étudiées ne démontrent pas qu'une telle automatisation de fait existe actuellement dans CFVR.

**À ÉTABLIR :**

> Quelle proportion des signalements CFVR proposés aux agents est finalement retenue ou rejetée après analyse humaine ?

> Quels éléments permettent de mesurer concrètement la capacité des agents à écarter une recommandation algorithmique ?

> Existe-t-il des indicateurs permettant d'identifier une validation quasi systématique des signalements par certains modèles, services ou catégories d'agents ?

Ces données permettraient de mesurer l'effectivité réelle de la garantie humaine.

---

### Une deuxième vulnérabilité apparaît : la boucle de rétroaction algorithmique

La CNIL identifie explicitement un autre problème [S37].

Les résultats des contrôles fiscaux passés sont utilisés pour développer les modèles employés dans CFVR.

Cela crée potentiellement une boucle :

```
modèle
   ↓
sélection d'une population
   ↓
contrôles
   ↓
résultats des contrôles
   ↓
nouvelles données d'apprentissage
   ↓
nouveau modèle
   ↓
nouvelle sélection
```

Le problème apparaît lorsqu'un biais initial influence les contrôles réalisés.

Les populations davantage contrôlées produisent mécaniquement davantage de données issues de contrôles.

Ces données peuvent ensuite alimenter les modèles futurs.

La CNIL décrit précisément le risque d'une amplification conduisant à une concentration des contrôles sur certaines populations ou catégories d'entités qui ne serait plus justifiée par la prévalence actualisée de la fraude [S37].

**AVÉRÉ :**

> La CNIL identifie explicitement un risque d'amplification des biais dans CFVR en raison de la réutilisation des résultats des contrôles passés pour développer les modèles.

Ce n'est donc pas une vulnérabilité hypothétique inventée par l'enquête.

---

### La garantie des 50 % est intéressante mais reconnue comme insuffisante à elle seule

Le ministère a introduit une garantie particulière.

Il limite à 50 % le taux de contrôles fiscaux ouverts par les agents à la suite de l'analyse de signaux provenant de CFVR [S37].

La CNIL considère cette mesure utile pour limiter le développement de biais significatifs.

Mais elle ajoute immédiatement que :

> **cette limitation ne permet pas, à elle seule, de parer à tout risque de biais significatif** [S37].

Elle demande donc également :

- des analyses portant sur l'explicabilité des algorithmes ;  
- des travaux critiques sur les biais susceptibles d'émerger ;  
- un suivi de l'efficacité des garanties [S37].

Le ministère s'est engagé à réaliser ces études et à en rendre compte dans les bilans d'activité de CFVR.

**GARANTIE DOCUMENTÉE :**

> Le ministère limite à 50 % la part des contrôles ouverts à la suite de signaux CFVR.

**LIMITATION EXPLICITEMENT RECONNUE :**

> La CNIL considère elle-même que cette garantie ne suffit pas à éliminer tous les risques de biais.

**À ÉTABLIR :**

> Les études annoncées sur l'explicabilité et les biais ont-elles été réalisées ?

> Quels résultats ont-elles produits ?

> Quels indicateurs permettent de vérifier que certaines populations ou catégories d'entités ne sont pas progressivement surreprésentées dans les contrôles du seul fait d'une boucle d'apprentissage ?

---

### L'apprentissage non supervisé augmente encore l'enjeu

La CNIL relève également le développement de nouvelles méthodes d'apprentissage dans CFVR, notamment des méthodes dites non supervisées [S37].

Dans ce type de méthode, le modèle cherche notamment à distinguer des comportements considérés comme normaux ou anormaux sans étiquetage préalable.

La CNIL considère que :

- l'élargissement massif des données ;  
- le développement de ces nouvelles méthodes ;

ont pour effet d'amplifier les risques associés aux algorithmes et aux biais [S37].

Cette évolution est particulièrement importante avec l'arrivée des données issues de plusieurs milliards de factures.

La chaîne devient :

```
données massives
   ↓
détection automatisée de structures / anomalies
   ↓
classification ou signalement
   ↓
liste d'entreprises considérées à risque
   ↓
analyse humaine
   ↓
contrôle éventuel
```

**POINT DE VIGILANCE MAJEUR :**

> Plus le fonctionnement du modèle devient complexe et dépend de relations détectées automatiquement dans de très grands volumes de données, plus la capacité à comprendre, contrôler et expliquer les raisons d'un signalement devient juridiquement et opérationnellement importante.

---

### Troisième vulnérabilité : l'explicabilité devient une garantie centrale

Le droit européen contient désormais une jurisprudence particulièrement précise sur l'explication des décisions automatisées [S52].

Dans l'affaire C-203/22, la Cour de justice précise que, lorsque le régime concerné s'applique, la personne doit pouvoir obtenir des informations lui permettant de comprendre :

- la procédure effectivement utilisée ;  
- les principes appliqués ;  
- la manière dont ses données ont contribué au résultat [S52].

La Cour précise également que :

> la complexité du traitement ne dispense pas de fournir une explication intelligible.

Une formule mathématique complexe ne constitue pas nécessairement une explication suffisante.

La description exhaustive de toutes les opérations techniques ne l'est pas davantage [S52].

**GARANTIE JURIDIQUE :**

> Lorsqu'une décision relève du régime des décisions automatisées du RGPD, la complexité d'un algorithme ne peut pas être utilisée comme justification permettant de rendre son résultat juridiquement inexplicable.

---

### Une tension apparaît avec les modèles complexes

Cette jurisprudence produit une question importante pour l'évolution de CFVR.

La CNIL demande précisément au ministère de travailler sur :

> **l'explicabilité des algorithmes** [S37].

Dans le même temps, CFVR développe :

- des méthodes d'apprentissage ;  
- des méthodes non supervisées ;  
- des analyses sur des volumes massifs ;  
- des rapprochements entre de multiples sources [S37][S45].

Il apparaît donc une tension structurelle :

```
augmentation de la complexité
   ↓
augmentation des capacités de détection
   ↓
mais
   ↓
nécessité de conserver
compréhension
contrôle
explicabilité
contestabilité
```

**VULNÉRABILITÉ JURIDIQUE POTENTIELLE :**

> Une architecture dont les résultats deviendraient suffisamment déterminants pour produire ou conditionner des décisions significatives devrait rester capable de fournir les garanties de transparence et d'explication requises par le droit applicable.

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas de conclure que les modèles CFVR sont aujourd'hui juridiquement inexplicables.

---

### Quatrième vulnérabilité : la qualité des données peut influencer directement le ciblage

L'intervention humaine documentée par la CNIL comprend une précaution révélatrice.

Les agents doivent notamment vérifier :

> que les dernières déclarations déposées ont bien été prises en compte [S37].

Cette exigence montre qu'un signalement algorithmique peut être influencé par l'état des données disponibles au moment de son calcul.

Or les données de facturation électronique vont considérablement augmenter la quantité et la granularité des informations exploitables.

Une erreur peut provenir :

```
donnée incorrecte
   ↓
rapprochement
   ↓
anomalie détectée
   ↓
signalement
   ↓
entreprise sélectionnée
```

La garantie humaine doit donc permettre de casser cette chaîne avant qu'un signal algorithmique erroné ne produise des conséquences injustifiées.

**VULNÉRABILITÉ :**

> Plus le nombre de sources et de données utilisées augmente, plus la maîtrise de leur exactitude, de leur actualité et de leur contexte devient déterminante pour la qualité du résultat algorithmique.

---

### La frontière juridique devient particulièrement importante si les conséquences évoluent

Aujourd'hui, la documentation établit principalement :

```
signalement
   ↓
orientation d'un agent
   ↓
analyse humaine
   ↓
contrôle fiscal éventuel
```

Cette architecture bénéficie précisément de l'existence de cette étape humaine.

Mais la jurisprudence SCHUFA montre qu'une autre configuration doit être analysée différemment :

```
résultat automatisé
   ↓
résultat déterminant
   ↓
décision ayant un effet significatif
```

[S51]

La question ne concerne donc pas uniquement CFVR aujourd'hui.

Elle concerne également toute évolution future dans laquelle un score ou une classification issus d'une infrastructure publique deviendraient déterminants pour :

- déclencher automatiquement une procédure ;  
- refuser un droit ou un service ;  
- modifier les conditions d'accès à un service ;  
- produire une conséquence financière ;  
- imposer une restriction ;  
- ou conditionner une autre décision produisant un effet significatif sur une personne.

**FRONTIÈRE JURIDIQUE :**

> Plus le résultat algorithmique devient déterminant dans la production d'une conséquence individuelle significative, plus la question de l'application de l'article 22 et des garanties associées devient centrale [S43][S51].

---

### Cette frontière est essentielle pour le pont avec les autres infrastructures de l'enquête

Cette conclusion fournit un élément juridique important pour les architectures étudiées dans le Chapitre 5.

Les chapitres précédents ont identifié séparément des capacités concernant :

- les transactions ;  
- la facturation électronique ;  
- l'identité ;  
- les produits ;  
- le passeport numérique de produit ;  
- les données environnementales ;  
- certaines conditions de paiement.

Aucun élément étudié ne démontre actuellement l'existence d'un système utilisant l'ensemble de ces données afin de produire automatiquement une décision individuelle.

Mais le cadre juridique permet désormais d'identifier ce qu'il faudrait rechercher si de telles infrastructures étaient rapprochées.

La chaîne juridiquement sensible serait :

```
données économiques
   +
données transactionnelles
   +
données d'identité
   +
données produit
   +
données environnementales
   ↓
profil / score / classification
   ↓
résultat automatisé
   ↓
influence déterminante
   ↓
décision produisant
un effet juridique ou significatif
```

À ce stade, plusieurs protections devraient alors être examinées simultanément :

- finalité du traitement ;  
- base juridique ;  
- minimisation ;  
- proportionnalité ;  
- exactitude des données ;  
- transparence ;  
- explicabilité ;  
- intervention humaine ;  
- contestation ;  
- article 22 du RGPD lorsque ses conditions sont réunies [S43][S44][S46][S48][S51][S52].

**DÉDUCTIBLE JURIDIQUEMENT :**

> L'interconnexion technique de plusieurs infrastructures ne suffit pas à rendre juridiquement admissible une décision résultant de leur combinaison.

**DÉDUCTIBLE JURIDIQUEMENT :**

> Si leur combinaison devait produire un score ou une classification jouant un rôle déterminant dans une décision individuelle significative, l'existence formelle d'un intermédiaire humain ne suffirait pas nécessairement à écarter les protections applicables aux décisions automatisées [S51].

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement qu'un score environnemental, un DPP ou une donnée issue de la facturation électronique détermine l'autorisation ou le refus d'un paiement ou d'un autre droit individuel.

Cette frontière doit impérativement être conservée.

---

### Une vulnérabilité plus profonde apparaît néanmoins

Les infrastructures étudiées montrent progressivement trois phénomènes distincts :

```
1. augmentation des données disponibles

2. augmentation des possibilités de rapprochement

3. augmentation des capacités algorithmiques
```

Pris séparément, chacun peut disposer d'un fondement juridique et de garanties propres.

Mais leur combinaison augmente la possibilité technique de produire des classifications de plus en plus fines.

Le droit ne prohibe pas cette évolution par principe.

Il impose cependant que les garanties évoluent avec la nature et l'influence du traitement.

**VULNÉRABILITÉ STRUCTURELLE :**

> Une architecture peut rester juridiquement présentée comme une aide à la décision tant que l'intervention humaine demeure réelle et déterminante. La frontière devient beaucoup plus sensible si l'accroissement de la précision, du volume ou de l'autorité accordée aux résultats algorithmiques transforme progressivement cette intervention humaine en validation essentiellement formelle.

C'est précisément cette évolution qu'il faudrait pouvoir mesurer dans le temps.

---

### Questions permettant de tester cette garantie

L'analyse permet maintenant de formuler plusieurs questions vérifiables :

> **1. Quel est le taux de rejet par les agents des dossiers proposés par CFVR après analyse humaine ?**

> **2. Ce taux est-il suivi modèle par modèle et catégorie de signalement par catégorie de signalement ?**

> **3. Quels mécanismes permettent de détecter une dépendance excessive des agents aux recommandations algorithmiques ?**

> **4. Les études sur les biais et l'explicabilité annoncées à la CNIL ont-elles été réalisées et leurs résultats sont-ils communicables ?**

> **5. Comment est mesurée la surreprésentation éventuelle de certaines catégories de contribuables ou d'entreprises dans les signalements ?**

> **6. Comment l'administration vérifie-t-elle qu'une corrélation détectée par un modèle reste liée à une prévalence réelle et actualisée de la fraude ?**

> **7. Quelle information peut être fournie à une personne qui souhaite comprendre le rôle joué par un traitement algorithmique dans la sélection de son dossier ?**

> **8. Quelles garanties empêchent qu'une évolution future transforme une recommandation algorithmique en déclenchement automatique ou quasi automatique d'une procédure ?**

Ces questions ne présument aucune violation.

Elles permettent de tester l'effectivité des garanties invoquées.

---

### Conclusion de 6.4

**AVÉRÉ :**

> CFVR utilise des méthodes algorithmiques pour identifier des anomalies et orienter la programmation du contrôle fiscal [S37][S45].

**AVÉRÉ :**

> Le développement de méthodes d'apprentissage non supervisé et l'élargissement massif des données conduisent la CNIL elle-même à considérer que les risques algorithmiques et les risques de biais sont amplifiés [S37].

**AVÉRÉ :**

> Les résultats des contrôles antérieurs sont utilisés pour développer les modèles, ce qui expose selon la CNIL le dispositif à un risque d'amplification des biais dans le temps [S37].

**GARANTIE DOCUMENTÉE :**

> Les signalements CFVR ne doivent pas remplacer l'analyse des agents et l'ouverture d'un contrôle fiscal doit actuellement résulter d'une décision humaine [S37].

**GARANTIE DOCUMENTÉE :**

> Le ministère limite à 50 % le taux de contrôles ouverts à la suite de signaux provenant de CFVR [S37].

**LIMITATION EXPLICITEMENT RECONNUE :**

> La CNIL considère que cette limite de 50 % ne suffit pas, à elle seule, à prévenir tous les risques de biais significatifs et demande des travaux supplémentaires sur l'explicabilité et les biais [S37].

**PRINCIPE JURISPRUDENTIEL :**

> Selon la CJUE, un résultat automatisé peut lui-même relever de la notion de décision automatisée lorsque la décision ultérieure dépend de manière déterminante de ce résultat [S51].

**GARANTIE JURIDIQUE :**

> Lorsque le régime des décisions automatisées s'applique, la complexité technique du système ne supprime pas les exigences de transparence et d'explication [S52].

**VULNÉRABILITÉ JURIDIQUE :**

> La protection reposant sur l'intervention humaine dépend de son effectivité réelle. Une validation humaine essentiellement formelle d'un résultat algorithmique déterminant pourrait nécessiter une réévaluation de la qualification juridique du processus.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas de mesurer précisément le taux de rejet des signalements CFVR par les agents ni, par conséquent, le degré d'influence pratique des recommandations algorithmiques sur les décisions d'ouverture de contrôle.

**À ÉTABLIR :**

> Les études annoncées sur l'explicabilité et les biais permettent-elles de démontrer que l'élargissement massif des données et le développement de nouvelles méthodes n'entraînent pas une concentration injustifiée des contrôles sur certaines populations ou catégories d'entités ?

**À ÉTABLIR :**

> Quels mécanismes permettent de démontrer que l'intervention humaine demeure substantielle lorsque les capacités prédictives et la complexité des modèles augmentent ?

**DÉDUCTIBLE JURIDIQUEMENT :**

> Si une infrastructure future combinait des données économiques, transactionnelles, d'identité, de produit ou environnementales afin de produire un résultat déterminant pour une décision individuelle significative, cette chaîne devrait être examinée au regard des garanties applicables aux traitements automatisés, indépendamment de la seule présence formelle d'un humain en bout de chaîne [S51].

**NON ÉTABLI :**

> Aucun élément étudié ne permet actuellement d'affirmer que CFVR prend automatiquement la décision d'ouvrir un contrôle fiscal ou qu'une donnée environnementale, un DPP ou une donnée de facturation détermine automatiquement l'accès à un paiement, un service ou un droit.

---

## 6.5 Nécessité, proportionnalité et minimisation

**Statut : OBLIGATIONS JURIDIQUES ÉTABLIES / CHANGEMENT D'ÉCHELLE AVÉRÉ / JUSTIFICATIONS À ÉTABLIR**

Les sections précédentes ont établi plusieurs éléments importants.

Les données issues de la facturation électronique doivent alimenter une infrastructure permettant leur exploitation algorithmique à grande échelle.

Elles rejoignent un traitement déjà alimenté par de nombreuses autres sources.

Des rapprochements sont réalisés afin notamment de détecter des anomalies et d'identifier des entreprises présentant certains risques fiscaux.

La volumétrie annoncée atteint plusieurs milliards de factures électroniques par an [S37][S45].

La question juridique devient alors différente.

Elle n'est plus seulement :

> **« la lutte contre la fraude constitue-t-elle une finalité légitime ? »**

Cette finalité est établie.

La question devient :

> **« l'ensemble des données collectées, leur granularité, leurs croisements, leurs durées de conservation et leurs modalités d'exploitation sont-ils nécessaires et proportionnés à cette finalité ? »**

Cette distinction est essentielle.

---

### Une finalité légitime ne suffit pas à démontrer la nécessité de chaque donnée

Le principe de minimisation prévu par l'article 5 du RGPD impose que les données personnelles soient :

> **adéquates, pertinentes et limitées à ce qui est nécessaire au regard des finalités poursuivies** [S36][S43].

Cette exigence porte donc non seulement sur l'existence d'une finalité légitime, mais également sur le rapport entre cette finalité et les données effectivement utilisées.

La chaîne juridique n'est pas :

```
objectif d'intérêt général
   ↓
toutes les données susceptibles d'être utiles
```

Elle est :

```
objectif précisément déterminé
   ↓
données nécessaires
   ↓
quantité nécessaire
   ↓
durée nécessaire
   ↓
accès nécessaires
   ↓
traitements nécessaires
```

**GARANTIE JURIDIQUE :**

> L'utilité potentielle d'une donnée ne suffit pas nécessairement à démontrer sa nécessité juridique.

---

### La CJUE applique directement cette exigence aux administrations fiscales

L'arrêt C-175/20 est particulièrement important pour cette enquête parce qu'il concerne précisément une administration fiscale [S53].

La Cour de justice y rappelle que les limitations à la protection des données doivent rester limitées à ce qui est strictement nécessaire.

Elle en déduit qu'un responsable du traitement, même lorsqu'il agit dans le cadre d'une mission d'intérêt public :

> **ne peut procéder de manière générale et indifférenciée à la collecte de données personnelles** [S53].

Il doit également :

> **s'abstenir de collecter les données qui ne sont pas strictement nécessaires aux finalités du traitement** [S53].

La Cour ajoute que le responsable doit rechercher une minimisation aussi importante que possible de la quantité de données collectées.

**PRINCIPE JURISPRUDENTIEL :**

> Une administration fiscale ne dispose donc pas, du seul fait de sa mission de lutte contre la fraude, d'un droit général à collecter indifféremment toutes les données personnelles susceptibles de présenter un intérêt analytique.

---

### La charge de la démonstration constitue un élément particulièrement important

La Cour ajoute une exigence essentielle.

Le responsable du traitement doit pouvoir démontrer le respect des principes prévus par l'article 5 du RGPD [S53].

Concernant la minimisation, elle indique qu'il appartient à l'administration concernée d'établir qu'elle a cherché à minimiser autant que possible la quantité de données collectées.

Concernant la durée, elle précise également que la période concernée ne peut dépasser celle qui est strictement nécessaire à l'objectif d'intérêt général poursuivi [S53].

La question n'est donc pas uniquement :

> **« peut-on démontrer que ces données sont utiles ? »**

Elle devient :

> **« peut-on démontrer pourquoi cette quantité précise de données est nécessaire ? »**

et :

> **« peut-on démontrer pourquoi une quantité moindre, une granularité inférieure ou une période plus courte ne permettrait pas d'atteindre suffisamment l'objectif poursuivi ? »**

**GARANTIE JURIDIQUE :**

> Le principe de responsabilité impose au responsable du traitement d'être en mesure de démontrer le respect de la minimisation.

---

### Cette jurisprudence rencontre directement le changement d'échelle de CFVR

La CNIL constate que l'arrivée des données issues de la facturation électronique augmente substantiellement le volume de données traitées dans CFVR [S37].

Elle indique que le volume des factures électroniques est estimé à :

> **2 à 3 milliards par an** [S37].

La volumétrie est telle que le ministère indique que ces données ne pourraient pas être exploitées dans l'infrastructure CFVR existante.

Une infrastructure disposant d'une puissance de calcul renforcée, la PSD, devient nécessaire précisément pour permettre leur exploitation [S37].

La chaîne documentée est donc :

```
nouvelle catégorie de données
   ↓
augmentation substantielle du volume
   ↓
2 à 3 milliards de factures / an
   ↓
infrastructure existante insuffisante
   ↓
PSD à puissance de calcul renforcée
   ↓
exploitation
   ↓
croisement des résultats
   ↓
ciblage fiscal
```

**AVÉRÉ :**

> L'intégration de la facturation électronique ne constitue pas une augmentation marginale du traitement.

Elle entraîne un changement d'échelle suffisamment important pour nécessiter une infrastructure de calcul renforcée [S37].

---

### Première vulnérabilité : le changement d'échelle doit pouvoir être justifié donnée par donnée

Le changement d'échelle ne constitue pas en lui-même une violation du principe de minimisation.

Une collecte massive peut être nécessaire lorsqu'une mission légitime ne peut raisonnablement être accomplie autrement.

Mais C-175/20 interdit de raisonner uniquement à partir de l'intérêt général poursuivi [S53].

Il faut également examiner les données effectivement nécessaires.

La question devient donc :

> **Toutes les catégories de données personnelles provenant de la facturation électronique qui sont intégrées ou exploitées dans cette chaîne sont-elles nécessaires aux modèles et analyses poursuivis ?**

Et plus précisément :

> **Chaque champ personnel exploité apporte-t-il une contribution nécessaire à une finalité déterminée ?**

> **Certaines analyses pourraient-elles fonctionner avec moins de champs ?**

> **Certaines données pourraient-elles être agrégées, pseudonymisées ou supprimées avant l'exploitation ?**

> **La même efficacité pourrait-elle être obtenue sans conserver certains éléments au niveau transactionnel ?**

**VULNÉRABILITÉ JURIDIQUE :**

> Plus une infrastructure absorbe systématiquement de données, plus la démonstration de nécessité ne peut raisonnablement se limiter à l'affirmation générale que ces données peuvent améliorer la lutte contre la fraude.

**À ÉTABLIR :**

> Quelle démonstration documentée justifie, catégorie par catégorie, les données personnelles issues de la facturation électronique effectivement nécessaires aux traitements réalisés dans la PSD et CFVR ?

---

### La jurisprudence oblige également à rechercher si un ciblage plus limité est possible

L'arrêt C-175/20 contient ici un raisonnement particulièrement intéressant [S53].

Dans cette affaire, la Cour demande précisément s'il serait possible d'atteindre l'objectif fiscal sans disposer potentiellement des données relatives à toutes les annonces concernées.

Elle envisage explicitement la possibilité de :

> **cibler certaines annonces au moyen de critères spécifiques** [S53].

Le principe est important.

Lorsque l'objectif peut être atteint par une collecte plus ciblée, la collecte généralisée devient plus difficile à justifier.

Appliqué à l'architecture étudiée, cela produit une question qui n'est plus théorique :

```
exploitation de données de facturation
à très grande échelle
   VS
sélection préalable
de catégories / opérations / situations
présentant des critères de risque
```

**QUESTION JURIDIQUE MAJEURE :**

> L'exploitation de la masse des données de facturation électronique est-elle nécessaire pour les finalités poursuivies ou certaines analyses pourraient-elles être réalisées à partir d'une sélection préalable moins intrusive ?

La réponse nécessite des informations techniques et statistiques qui ne sont pas présentes dans les sources publiques étudiées.

**ANGLE MORT DOCUMENTAIRE :**

> Nous n'avons pas encore identifié de démonstration publique comparant l'exploitation massive prévue avec des architectures moins intrusives permettant éventuellement d'obtenir des résultats comparables.

---

### Deuxième vulnérabilité : la minimisation concerne également la granularité

Deux traitements peuvent exploiter le même nombre de documents tout en présentant des niveaux d'ingérence très différents.

Il faut distinguer :

```
existence d'une facture
```

de :

```
contenu détaillé de la facture
```

et encore de :

```
contenu détaillé
   +
historique
   +
contreparties
   +
rapprochements avec d'autres bases
```

Le principe de minimisation s'applique à la quantité de données, mais également à l'étendue du traitement et à leur accessibilité [S43].

La question pertinente n'est donc pas uniquement :

> **combien de factures sont traitées ?**

Elle est également :

> **quel niveau de détail provenant de chacune de ces factures est réellement nécessaire pour chaque modèle ou requête ?**

**VULNÉRABILITÉ JURIDIQUE :**

> Une justification portant sur la nécessité d'utiliser les factures ne démontre pas automatiquement la nécessité d'utiliser chaque donnée personnelle qu'elles contiennent.

---

### Troisième vulnérabilité : le rapprochement change l'intensité du traitement

Une donnée isolée et la même donnée rapprochée de nombreuses autres informations ne présentent pas nécessairement la même intensité d'ingérence.

CFVR permet précisément de rapprocher plusieurs sources [S37][S45].

La PSD doit progressivement accueillir l'ensemble des données du traitement CFVR [S37].

Ainsi :

```
donnée A
   +
donnée B
   +
donnée C
   +
facturation électronique
   +
historique fiscal
   +
autres sources
   ↓
capacité d'inférence accrue
```

Le principe de minimisation doit donc être examiné non seulement au niveau de chaque base prise séparément, mais également au regard des traitements effectivement réalisés à partir de leur combinaison.

**VULNÉRABILITÉ STRUCTURELLE :**

> Des données individuellement nécessaires à plusieurs traitements peuvent produire, lorsqu'elles sont rapprochées, une capacité d'analyse beaucoup plus intrusive que celle résultant de chacune des sources prises isolément.

**À ÉTABLIR :**

> Comment la nécessité et la proportionnalité sont-elles appréciées pour les combinaisons de données et non uniquement pour chaque source prise séparément ?

---

### Le Conseil constitutionnel impose également un contrôle de proportionnalité

Cette exigence ne provient pas uniquement du RGPD et de la jurisprudence européenne.

Le Conseil constitutionnel rattache la protection des données personnelles au droit au respect de la vie privée garanti par l'article 2 de la Déclaration des droits de l'homme et du citoyen [S44].

Il juge que :

> **la collecte, l'enregistrement, la conservation, la consultation et la communication de données personnelles doivent être justifiés par un motif d'intérêt général et mis en œuvre de manière adéquate et proportionnée à cet objectif** [S44].

Le contrôle porte donc sur plusieurs opérations successives :

```
collecte
   ↓
enregistrement
   ↓
conservation
   ↓
consultation
   ↓
communication
```

**GARANTIE CONSTITUTIONNELLE :**

> La présence d'un motif d'intérêt général ne dispense pas le dispositif d'un contrôle portant sur l'adéquation et la proportionnalité de ses modalités concrètes.

---

### Quatrième vulnérabilité : la conservation doit être justifiée séparément

Une donnée nécessaire aujourd'hui ne devient pas automatiquement nécessaire pendant toute la durée techniquement possible de sa conservation.

Le principe de limitation de la conservation impose que les données permettant l'identification des personnes ne soient pas conservées plus longtemps que nécessaire au regard des finalités poursuivies [S43].

C-175/20 applique également la logique de stricte nécessité à la période concernée par une collecte fiscale [S53].

Cette question devient particulièrement importante dans une infrastructure algorithmique.

Plus l'historique disponible est long :

```
plus de données historiques
   ↓
plus de comparaisons possibles
   ↓
plus de modèles possibles
   ↓
plus de capacités d'inférence
```

Mais :

```
utilité analytique
   ≠
nécessité juridique automatique
```

**VULNÉRABILITÉ JURIDIQUE :**

> Une durée longue doit pouvoir être justifiée par rapport aux finalités poursuivies et ne peut reposer uniquement sur l'intérêt potentiel de disposer d'un historique plus riche.

---

### Un premier point concret existe déjà concernant les échanges sociaux

La CNIL a précisément appliqué ce raisonnement aux échanges entre la DGFiP et les organismes de sécurité sociale [S37].

Elle constate que le projet qui lui avait été soumis ne précisait pas la durée de conservation des données transmises.

Elle rappelle alors que les échanges entre administrations ne sont permis que lorsque leurs modalités restent proportionnées aux objectifs poursuivis.

Elle demande que la conservation soit limitée à la durée nécessaire [S37].

Le ministère s'est engagé à prévoir une durée maximale de dix ans.

Mais la CNIL demande également quelque chose de plus précis :

> que les durées applicables soient déterminées **catégorie de données par catégorie de données** dans les conventions conclues avec les organismes sociaux [S37].

Cette précision est particulièrement intéressante.

Elle montre que :

```
une durée maximale générale
   ≠
justification individualisée
de la durée nécessaire
pour chaque catégorie
```

**AVÉRÉ :**

> La CNIL demande elle-même une appréciation plus granulaire des durées de conservation pour les données échangées avec les organismes sociaux [S37].

---

### Cinquième vulnérabilité : « au maximum dix ans » ne signifie pas « dix ans nécessaires »

Cette distinction doit être conservée.

Le fait qu'une réglementation autorise une conservation jusqu'à une certaine durée ne signifie pas nécessairement que toutes les catégories de données doivent effectivement être conservées pendant cette durée.

Le principe de minimisation et de limitation de la conservation conduit à rechercher la durée nécessaire au traitement concerné [S43][S53].

Ainsi :

```
durée maximale juridiquement possible
   ≠
durée nécessaire pour chaque donnée
```

**QUESTION À ÉTABLIR :**

> Parmi les données susceptibles d'être conservées jusqu'à dix ans, lesquelles nécessitent effectivement cette durée et lesquelles pourraient être supprimées ou anonymisées plus tôt ?

---

### Sixième vulnérabilité : l'accumulation progressive peut déplacer le contrôle de proportionnalité

Le 6.2 avait identifié une question laissée volontairement ouverte :

> jusqu'où des extensions successives de finalités, de sources et de destinataires peuvent-elles s'accumuler avant que leur effet global impose une nouvelle appréciation de nécessité et de proportionnalité ?

Cette question devient ici beaucoup plus concrète.

CFVR n'est plus le traitement qu'il était lors de sa création.

Son périmètre a évolué.

Ses sources ont évolué.

Ses méthodes ont évolué.

Ses capacités de calcul ont évolué.

Les catégories d'agents impliqués ont évolué.

Les échanges inter-administrations ont évolué.

Et plusieurs milliards de factures électroniques viennent désormais rejoindre cette architecture [S37][S45].

On peut donc représenter l'évolution ainsi :

```
traitement initial
   ↓
nouvelles sources
   ↓
nouveaux rapprochements
   ↓
nouveaux algorithmes
   ↓
nouveaux accédants
   ↓
nouveaux échanges
   ↓
nouvelle infrastructure de calcul
   ↓
plusieurs milliards de factures / an
```

Chaque extension peut disposer séparément d'un fondement juridique.

Mais cela ne répond pas entièrement à une autre question :

> **l'architecture résultante demeure-t-elle, dans son ensemble, nécessaire et proportionnée ?**

**VULNÉRABILITÉ JURIDIQUE STRUCTURELLE :**

> L'appréciation isolée de chaque extension peut ne pas suffire à rendre compte de l'intensité globale du traitement résultant de leur accumulation.

---

### Le principe de responsabilité renverse ici une partie du raisonnement

L'un des apports les plus importants de C-175/20 est que la démonstration de la minimisation incombe au responsable du traitement [S53].

Cela change la manière de formuler les questions de cette enquête.

Nous n'avons pas nécessairement à démontrer :

> **« cette donnée est inutile ».**

La question juridiquement pertinente peut être :

> **« quelle démonstration établit que cette donnée est nécessaire ? »**

De même, il n'est pas nécessaire d'affirmer :

> **« cette durée est excessive ».**

On peut demander :

> **« quelle démonstration établit que cette durée est nécessaire à cette finalité ? »**

Ou encore :

> **« quelle démonstration établit que le même objectif ne pourrait pas être atteint avec une quantité moindre de données ? »**

C'est une différence méthodologique fondamentale.

---

### Septième vulnérabilité : les capacités techniques ne constituent pas la mesure de la nécessité

La CNIL explique que la PSD est nécessaire techniquement parce que la volumétrie des données de facturation électronique dépasse les capacités de l'environnement CFVR existant [S37].

Cela établit :

> **la nécessité technique d'une infrastructure plus puissante pour traiter le volume envisagé.**

Cela ne répond cependant pas à une question différente :

> **la nécessité juridique de traiter l'intégralité du volume envisagé.**

Les deux raisonnements ne doivent pas être confondus.

```
« nous avons besoin de la PSD
pour traiter autant de données »
   ≠
« nous avons démontré qu'il est nécessaire
de traiter autant de données »
```

**VULNÉRABILITÉ DOCUMENTAIRE :**

> Les sources étudiées expliquent pourquoi une puissance de calcul renforcée est nécessaire pour exploiter la volumétrie prévue, mais elles ne permettent pas, à elles seules, de démontrer pourquoi cette volumétrie précise constitue le niveau minimal nécessaire à chaque finalité poursuivie.

Cette distinction est particulièrement importante.

---

### Ce raisonnement devient crucial pour les autres infrastructures de l'enquête

Le principe de nécessité ne concerne pas uniquement CFVR.

Il fournit également un test juridique pour toute interconnexion future impliquant des données personnelles.

Les chapitres précédents ont identifié différentes infrastructures relatives notamment :

- aux transactions ;  
- à la facturation ;  
- à l'identité ;  
- aux produits ;  
- au DPP ;  
- aux informations environnementales ;  
- à certaines infrastructures de paiement.

L'existence séparée de bases juridiques permettant certains traitements dans chacune de ces infrastructures ne suffirait pas nécessairement à justifier leur combinaison.

La question devrait être reposée pour le traitement résultant :

```
donnée nécessaire dans système A
   +
donnée nécessaire dans système B
   +
donnée nécessaire dans système C

   ≠ automatiquement

combinaison A + B + C nécessaire
```

**DÉDUCTIBLE JURIDIQUEMENT :**

> La nécessité de collecter une donnée dans son système d'origine ne démontre pas automatiquement la nécessité de la rapprocher des données d'une autre infrastructure.

C'est une frontière juridique importante pour le pont construit dans cette enquête.

---

### Application au pont environnement / identité / paiement

Aucun élément étudié ne démontre actuellement l'existence d'un traitement combinant l'ensemble de ces infrastructures afin de produire une décision individuelle.

Mais si une évolution future conduisait par exemple à :

```
identité
   +
transaction
   +
produit
   +
DPP
   +
information environnementale
   +
paiement
   ↓
analyse / classification
   ↓
conséquence individuelle
```

la seule existence d'une base juridique propre à chaque composant ne suffirait pas nécessairement à établir la nécessité et la proportionnalité du traitement résultant.

Il faudrait notamment examiner :

- la finalité précise du rapprochement ;  
- les données strictement nécessaires ;  
- la granularité nécessaire ;  
- la durée nécessaire ;  
- les personnes pouvant y accéder ;  
- les alternatives moins intrusives ;  
- les conséquences pour les personnes ;  
- les garanties contre les usages secondaires [S43][S44][S53].

**DÉDUCTIBLE JURIDIQUEMENT :**

> Plus plusieurs infrastructures sont rapprochées, plus la justification doit porter sur le traitement résultant de leur combinaison et non uniquement sur la légalité individuelle de chacun de leurs composants.

**NON ÉTABLI :**

> Rien dans les sources étudiées ne démontre actuellement qu'une telle interconnexion globale soit mise en œuvre ou juridiquement prévue.

---

### Une véritable ligne de contrôle apparaît

Après 6.1 à 6.5, le raisonnement juridique peut maintenant être résumé ainsi :

```
base juridique
   ↓
finalité légitime
   ↓
   MAIS
   ↓
données nécessaires ?
   ↓
quantité nécessaire ?
   ↓
granularité nécessaire ?
   ↓
croisements nécessaires ?
   ↓
durée nécessaire ?
   ↓
accédants nécessaires ?
   ↓
alternative moins intrusive ?
   ↓
proportionnalité globale ?
```

Une réponse positive aux deux premières étapes ne répond donc pas automatiquement aux suivantes.

---

### Questions permettant de tester concrètement la proportionnalité

L'analyse permet désormais de poser des questions beaucoup plus précises :

> **1. Quelles catégories exactes de données personnelles issues des factures sont exploitées dans la PSD pour chaque modèle ou requête ?**

> **2. Quelle analyse démontre la nécessité de chacune de ces catégories ?**

> **3. Quels tests ont été réalisés avec un jeu de données moins étendu ou moins granulaire ?**

> **4. L'administration a-t-elle comparé l'efficacité de l'exploitation massive avec celle d'une collecte ou sélection préalable fondée sur des critères de risque ?**

> **5. Quelles données sont supprimées avant exploitation parce qu'elles ne sont pas nécessaires ?**

> **6. Quelles données sont agrégées, pseudonymisées ou anonymisées avant leur rapprochement ?**

> **7. Pour chaque catégorie de données, quelle durée de conservation est effectivement appliquée et pourquoi cette durée est-elle nécessaire ?**

> **8. Quelle analyse porte sur l'effet cumulé des différentes sources utilisées dans CFVR ?**

> **9. L'AIPD examine-t-elle des architectures alternatives moins intrusives ?**

> **10. Quelle démonstration permet d'établir que le changement d'échelle introduit par plusieurs milliards de factures demeure proportionné aux gains obtenus pour les finalités poursuivies ?**

Ces questions ne demandent pas à l'administration de démontrer que le traitement présente un risque nul.

Elles demandent la démonstration de sa nécessité et de sa proportionnalité.

---

### Conclusion de 6.5

**AVÉRÉ :**

> Le principe de minimisation impose que les données personnelles soient adéquates, pertinentes et limitées à ce qui est nécessaire aux finalités poursuivies [S36][S43].

**PRINCIPE JURISPRUDENTIEL :**

> Une administration fiscale ne peut pas procéder de manière générale et indifférenciée à la collecte de données personnelles et doit s'abstenir de collecter celles qui ne sont pas strictement nécessaires [S53].

**PRINCIPE JURISPRUDENTIEL :**

> Le responsable du traitement doit pouvoir démontrer qu'il a cherché à minimiser autant que possible la quantité de données collectées et la période concernée [S53].

**GARANTIE CONSTITUTIONNELLE :**

> La collecte, l'enregistrement, la conservation, la consultation et la communication de données personnelles doivent être justifiés par un motif d'intérêt général et mis en œuvre de manière adéquate et proportionnée à cet objectif [S44].

**AVÉRÉ :**

> L'intégration de la facturation électronique entraîne une augmentation substantielle du volume de données de CFVR, estimée à plusieurs milliards de factures par an, nécessitant le recours à une infrastructure de calcul renforcée [S37].

**AVÉRÉ :**

> La CNIL demande déjà, concernant certains échanges inter-administrations, que les durées de conservation soient précisées catégorie de données par catégorie de données [S37].

**VULNÉRABILITÉ JURIDIQUE :**

> La légitimité de la lutte contre la fraude ne dispense pas de démontrer la nécessité de la quantité, de la granularité, de la durée et des rapprochements de données effectivement utilisés.

**VULNÉRABILITÉ STRUCTURELLE :**

> La nécessité individuelle de données provenant de plusieurs systèmes ne démontre pas automatiquement la nécessité de leur combinaison.

**VULNÉRABILITÉ DOCUMENTAIRE :**

> Les sources publiques étudiées expliquent pourquoi une infrastructure de calcul renforcée est nécessaire pour exploiter le volume envisagé, mais ne suffisent pas à démontrer pourquoi l'exploitation de cette volumétrie précise constitue elle-même le moyen minimal nécessaire à chaque finalité poursuivie.

**ANGLE MORT DOCUMENTAIRE :**

> Nous n'avons pas identifié dans les sources publiques étudiées une comparaison permettant de déterminer si certaines finalités de CFVR pourraient être atteintes avec une quantité moindre de données, une granularité inférieure ou un ciblage préalable plus restrictif.

**À ÉTABLIR :**

> L'administration peut-elle démontrer, conformément au principe de responsabilité, la nécessité de chaque catégorie de données personnelles exploitée et l'absence d'une solution raisonnablement moins intrusive permettant d'atteindre les mêmes finalités ?

**À ÉTABLIR :**

> L'effet cumulé des extensions successives de CFVR fait-il l'objet d'une appréciation globale et régulièrement réévaluée de nécessité et de proportionnalité ?

**DÉDUCTIBLE JURIDIQUEMENT :**

> Toute future interconnexion de données personnelles provenant de la facturation, de l'identité, des produits, du DPP, de données environnementales ou d'infrastructures de paiement devrait justifier la nécessité du rapprochement lui-même et non seulement la légalité séparée de chaque source.

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas de conclure que l'intégration actuelle des données de facturation électronique dans CFVR est disproportionnée ou contraire au RGPD.

---

## 6.6 Droits des personnes et contrôle par la CNIL

**Statut : DROITS ÉTABLIS / RESTRICTIONS EXPRESSÉMENT PRÉVUES / CONTRÔLE INDÉPENDANT / EFFECTIVITÉ À EXAMINER**

Les sections précédentes ont établi qu'une quantité importante de données personnelles peut être collectée, rapprochée et analysée dans le cadre de CFVR.

Elles ont également établi que :

- les données de facturation électronique doivent rejoindre cette architecture ;  
- certains résultats sont produits par des traitements algorithmiques ;  
- ces résultats peuvent contribuer à la sélection de dossiers ;  
- des échanges existent avec d'autres administrations ;  
- les données et résultats peuvent circuler entre plusieurs environnements et catégories de destinataires [S37][S45].

Une question devient alors centrale :

> **Quels moyens une personne possède-t-elle pour savoir quelles données la concernant sont utilisées, vérifier leur exactitude, obtenir leur correction et contester un traitement qui porterait atteinte à ses droits ?**

Cette question concerne l'effectivité des garanties.

Un droit inscrit dans un texte et un droit effectivement exerçable ne constituent pas nécessairement la même chose.

---

### Le RGPD reconnaît des droits importants aux personnes

Le RGPD prévoit notamment :

- un droit à l'information ;  
- un droit d'accès ;  
- un droit de rectification ;  
- dans certaines conditions, un droit à l'effacement ;  
- un droit à la limitation du traitement ;  
- dans certaines conditions, un droit d'opposition ;  
- des garanties relatives à certaines décisions automatisées ;  
- un droit de saisir une autorité de contrôle ;  
- un droit à un recours juridictionnel effectif [S43].

Le droit d'accès prévu à l'article 15 permet notamment de connaître :

- les finalités du traitement ;  
- les catégories de données personnelles concernées ;  
- les destinataires ou catégories de destinataires ;  
- la durée de conservation ou ses critères de détermination ;  
- l'existence de certains autres droits ;  
- l'origine des données lorsqu'elles n'ont pas été collectées auprès de la personne ;  
- dans les situations prévues par le RGPD, certaines informations relatives à la logique d'une décision automatisée [S43].

**GARANTIE JURIDIQUE :**

> Une personne n'est donc pas juridiquement dépourvue de moyens de contrôle sur l'utilisation de ses données par une administration.

---

### CFVR prévoit explicitement l'exercice de certains de ces droits

L'article 6 de l'arrêté instituant CFVR prévoit expressément que les droits d'accès et de rectification des articles 15 et 16 du RGPD peuvent être exercés [S45].

Selon l'origine des données, ces droits s'exercent :

- auprès du bureau SJCF-1D ;  
- ou auprès du centre des finances publiques dont relève la personne [S45].

Le droit à la limitation prévu à l'article 18 du RGPD s'exerce également auprès du bureau SJCF-1D [S45].

**AVÉRÉ :**

> CFVR n'est pas un traitement placé en dehors des droits d'accès, de rectification et de limitation.

Mais l'arrêté prévoit immédiatement plusieurs restrictions.

---

### Première restriction majeure : le droit d'opposition ne s'applique pas à CFVR

L'article 6 de l'arrêté CFVR dispose explicitement que :

> **le droit d'opposition prévu à l'article 21 du RGPD ne s'applique pas au traitement** [S45].

Depuis la modification de juillet 2026, cette exclusion est expressément rattachée aux objectifs mentionnés aux e et h du paragraphe 1 de l'article 23 du RGPD [S45].

Ces dispositions concernent notamment :

- des objectifs importants d'intérêt public général de l'Union ou d'un État membre, notamment en matière fiscale ;  
- des missions de contrôle, d'inspection ou de réglementation liées notamment à ces objectifs [S43].

La conséquence pratique est importante.

Une personne ne peut pas simplement décider :

```
« je refuse que mes données
soient utilisées dans CFVR »
   ↓
arrêt du traitement
```

Le droit d'opposition est expressément écarté pour ce traitement.

**LATITUDE JURIDIQUE :**

> Le droit européen permet, sous conditions, que certains droits soient restreints pour protéger notamment des intérêts fiscaux importants et les missions de contrôle associées.

**RESTRICTION AVÉRÉE :**

> Dans CFVR, le droit d'opposition prévu à l'article 21 du RGPD n'est pas applicable [S45].

Cette restriction ne constitue donc pas en elle-même une violation du RGPD.

Elle constitue néanmoins une limitation concrète du contrôle individuel exercé par la personne sur l'utilisation de ses données.

---

### Deuxième restriction : accès et rectification peuvent eux-mêmes être limités

L'arrêté CFVR prévoit également que les droits d'accès et de rectification peuvent faire l'objet de restrictions dans les conditions prévues par l'article 52 de la loi Informatique et Libertés [S45][S54].

Cette disposition concerne précisément certains traitements utilisés par les administrations pour contrôler ou recouvrer des impositions [S54].

La logique est compréhensible :

```
droit d'accès
   ↓
mais
   ↓
ne pas révéler une information
qui compromettrait
le contrôle fiscal
```

Une personne faisant l'objet d'une analyse de risque ne peut donc pas nécessairement obtenir immédiatement l'intégralité des informations qui permettraient de révéler les méthodes de contrôle ou de compromettre leur finalité.

**LATITUDE JURIDIQUE :**

> Le droit prévoit expressément la possibilité de restreindre certains droits afin de préserver l'efficacité de certaines missions fiscales.

Mais cette possibilité crée une tension évidente :

```
pour contester efficacement
   ↓
il faut comprendre
ce qui est fait

   mais

pour préserver le contrôle
   ↓
certaines informations
peuvent être restreintes
```

---

### La CNIL devient alors un intermédiaire essentiel

Lorsque les restrictions prévues pour CFVR s'appliquent, la personne exerce ses droits par l'intermédiaire de la CNIL dans les conditions prévues par l'article 118 de la loi Informatique et Libertés [S45][S54].

La CNIL procède alors aux vérifications nécessaires.

Elle peut faire procéder aux modifications nécessaires.

Elle informe ensuite la personne qu'il a été procédé aux vérifications et lui indique l'existence d'un recours juridictionnel [S54].

Lorsque certaines informations peuvent être communiquées sans compromettre les finalités protégées, leur communication peut intervenir dans les conditions prévues par la loi [S54].

**GARANTIE JURIDIQUE :**

> La restriction de l'accès direct n'entraîne donc pas nécessairement l'absence de contrôle.

Un tiers institutionnel indépendant peut vérifier le traitement.

---

### Mais une différence fondamentale apparaît entre vérification et compréhension personnelle

Cette architecture protège simultanément deux intérêts :

```
efficacité du contrôle fiscal
   ↕
droits de la personne
```

Mais elle peut produire une situation particulière :

```
la personne soupçonne
une donnée ou analyse erronée
   ↓
elle demande accès / rectification
   ↓
certaines informations sont restreintes
   ↓
la CNIL effectue des vérifications
   ↓
la personne peut être informée
que les vérifications ont été réalisées
   ↓
sans nécessairement connaître
l'intégralité des informations protégées
```

**VULNÉRABILITÉ JURIDIQUE STRUCTURELLE :**

> Plus les informations nécessaires pour comprendre l'origine d'un signalement sont protégées contre leur divulgation, plus l'effectivité de la contestation individuelle dépend du contrôle exercé par la CNIL et, le cas échéant, par le juge.

Cela ne signifie pas que le recours devient fictif.

Cela signifie que le contrôle individuel peut devenir en partie **médiatisé par une autorité indépendante** plutôt que directement exercé par la personne.

---

### La rectification devient particulièrement importante dans une architecture interconnectée

Le droit de rectification permet d'obtenir la correction de données personnelles inexactes [S43].

Mais l'architecture étudiée ne se limite plus nécessairement à une donnée stockée dans une seule base.

Une donnée peut suivre une chaîne :

```
donnée source
   ↓
transmission
   ↓
rapprochement
   ↓
analyse
   ↓
indicateur
   ↓
résultat algorithmique
   ↓
dossier proposé
```

Le RGPD prévoit également que lorsqu'une rectification, un effacement ou une limitation intervient, le responsable du traitement doit en principe la communiquer aux destinataires auxquels les données ont été transmises, sauf impossibilité ou effort disproportionné [S43].

Cette garantie devient particulièrement importante dans une architecture multi-sources.

---

### Première question difficile : corriger la donnée corrige-t-il ses conséquences ?

Prenons une situation hypothétique :

```
donnée A incorrecte
   ↓
croisement avec B et C
   ↓
indicateur D
   ↓
score / classification E
   ↓
signalement F
```

La correction de A est juridiquement encadrée.

Mais plusieurs questions supplémentaires apparaissent :

> **D est-il automatiquement recalculé ?**

> **E est-il supprimé ou réévalué ?**

> **F est-il retiré s'il reposait sur l'information incorrecte ?**

> **Les destinataires de F sont-ils informés ?**

> **Les données dérivées demeurent-elles dans d'autres environnements ?**

Le RGPD contient des mécanismes de rectification, de limitation et de notification aux destinataires [S43].

Mais leur application à des chaînes complexes de données dérivées doit être examinée concrètement.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas de déterminer précisément le mécanisme technique par lequel une rectification effectuée dans une donnée source est propagée aux résultats, indicateurs, classifications ou signalements déjà produits à partir de cette donnée dans CFVR et la PSD.

---

### Cette question n'est pas théorique pour CFVR

La CNIL demande que les agents vérifient notamment que les dernières déclarations déposées ont bien été prises en compte avant de décider de l'ouverture d'un contrôle [S37].

Cette exigence constitue une garantie importante.

Mais elle confirme également qu'un résultat algorithmique peut être affecté par l'état des données utilisées au moment de sa production.

La chaîne suivante est donc juridiquement pertinente :

```
donnée ancienne / inexacte / incomplète
   ↓
analyse algorithmique
   ↓
anomalie apparente
   ↓
signalement
   ↓
vérification humaine
```

La vérification humaine constitue ici une barrière essentielle.

**GARANTIE DOCUMENTÉE :**

> L'agent ne doit pas traiter le signal algorithmique comme une vérité autonome et doit analyser le dossier à partir des informations pertinentes et actualisées [S37].

---

### Le droit à la limitation offre une protection supplémentaire

L'article 18 du RGPD prévoit notamment qu'une personne peut demander la limitation du traitement lorsqu'elle conteste l'exactitude de données, pendant la période permettant au responsable de vérifier leur exactitude [S43].

CFVR prévoit expressément l'exercice de ce droit auprès du bureau SJCF-1D [S45].

La limitation peut donc constituer une protection particulièrement importante lorsqu'une information susceptible d'influencer un traitement est contestée.

**GARANTIE JURIDIQUE :**

> La contestation de l'exactitude d'une donnée peut, dans les conditions prévues par le RGPD, conduire à limiter temporairement son traitement pendant sa vérification [S43][S45].

**À ÉTABLIR :**

> Comment cette limitation est-elle techniquement propagée lorsque la donnée contestée a déjà contribué à produire des résultats dans plusieurs environnements ?

---

### Le problème devient plus complexe avec les données dérivées

Une infrastructure algorithmique ne se contente pas nécessairement de recopier les données sources.

Elle peut produire :

- des indicateurs ;  
- des catégories ;  
- des relations ;  
- des anomalies ;  
- des scores ;  
- des résultats de requêtes ;  
- des propositions de contrôle.

CFVR alimente notamment GALAXIE concernant certains liens entre individus et entités et PILOT CF concernant les dossiers proposés pour contrôle [S45].

La question de rectification doit donc potentiellement être envisagée à plusieurs niveaux :

```
niveau 1
donnée source

niveau 2
donnée rapprochée

niveau 3
inférence / indicateur

niveau 4
résultat algorithmique

niveau 5
conséquence opérationnelle
```

**VULNÉRABILITÉ STRUCTURELLE :**

> Plus une architecture produit de données dérivées à partir de plusieurs sources, plus la correction effective d'une information erronée nécessite de maîtriser non seulement la donnée initiale, mais également les résultats qui en ont été tirés.

---

### Deuxième question difficile : peut-on savoir pourquoi son dossier a été sélectionné ?

Le droit d'accès permet d'obtenir de nombreuses informations relatives au traitement [S43].

Mais CFVR est précisément un dispositif de détection et de programmation du contrôle fiscal.

Une divulgation trop détaillée des règles de détection pourrait compromettre certaines de ses finalités.

D'où la possibilité de restreindre certains droits [S45][S54].

La personne peut donc se trouver face à une difficulté structurelle :

```
pour contester un signalement
   ↓
comprendre pourquoi
le système l'a produit

   mais

expliquer précisément
la méthode de détection
   ↓
peut compromettre
l'efficacité du contrôle
```

**VULNÉRABILITÉ JURIDIQUE :**

> L'effectivité du droit de contestation dépend de l'équilibre entre le niveau d'information accessible à la personne et le niveau de secret nécessaire à la protection des méthodes de contrôle.

---

### Cette tension rejoint directement l'explicabilité étudiée en 6.4

La jurisprudence étudiée en 6.4 montre que, lorsque le régime des décisions automatisées est applicable, la complexité d'un système ne dispense pas le responsable de fournir les explications juridiquement requises [S52].

CFVR ne constitue pas, selon les sources actuelles, un système décidant automatiquement de l'ouverture d'un contrôle.

Mais la question de l'explicabilité reste importante parce que la CNIL demande elle-même au ministère de mener des travaux sur l'explicabilité et les biais [S37].

On obtient donc une frontière :

```
secret nécessaire
des méthodes de contrôle

   ↕

compréhension nécessaire
pour exercer les droits
```

**À ÉTABLIR :**

> Quel niveau d'explication peut être fourni à une personne concernant le rôle d'un résultat CFVR dans la sélection de son dossier sans compromettre les méthodes de contrôle ?

---

### L'information des personnes reste néanmoins obligatoire

Concernant les nouveaux échanges entre la DGFiP et les organismes de sécurité sociale, la CNIL rappelle expressément que chacune des administrations concernées doit informer les personnes conformément aux articles 12 à 14 du RGPD [S37].

Le ministère a indiqué que les conventions organisant ces échanges rappelleront cette obligation [S37].

C'est un point important.

L'existence d'échanges légalement autorisés ne supprime donc pas automatiquement l'obligation d'information.

**GARANTIE DOCUMENTÉE :**

> La CNIL exige que les personnes concernées soient informées des échanges de données entre la DGFiP et les organismes de sécurité sociale dans les conditions prévues par le RGPD [S37].

---

### Mais l'information générale ne signifie pas connaissance individuelle de chaque utilisation

Il faut distinguer :

```
être informé
de l'existence d'un traitement
   ≠
savoir qu'une donnée précise
a été utilisée dans une analyse précise

   ≠

connaître le résultat
de cette analyse
   ≠
savoir que ce résultat
a contribué à une décision
```

Ces quatre niveaux d'information n'ont ni le même objet ni nécessairement le même régime juridique.

**VULNÉRABILITÉ DOCUMENTAIRE :**

> L'information générale sur l'existence et les finalités de CFVR ne permet pas, à elle seule, de déterminer dans quelle mesure une personne peut retracer concrètement l'utilisation de ses données dans une analyse particulière.

---

### La CNIL dispose de pouvoirs de contrôle importants

La CNIL ne se limite pas à rendre des avis lors de la création ou de la modification des traitements.

Le RGPD lui confère notamment des pouvoirs permettant :

- d'exiger les informations nécessaires ;  
- de mener des enquêtes et audits ;  
- d'accéder aux données personnelles nécessaires à sa mission ;  
- d'accéder aux installations et moyens de traitement ;  
- d'ordonner certaines mises en conformité ;  
- de limiter ou interdire certains traitements dans les conditions prévues par le droit [S43].

Une personne peut également introduire une réclamation auprès d'une autorité de contrôle lorsqu'elle estime qu'un traitement la concernant viole le RGPD [S43].

**GARANTIE INSTITUTIONNELLE :**

> Le contrôle de la légalité du traitement ne dépend donc pas uniquement de l'administration qui exploite les données.

---

### L'avis préalable de la CNIL ne constitue cependant pas une validation définitive du système

CFVR existe depuis 2014.

Depuis, son périmètre a connu de nombreuses évolutions [S37][S45].

Il a notamment été étendu :

- aux professionnels ;  
- aux personnes physiques liées aux entreprises ;  
- aux particuliers ;  
- à de nouvelles sources ;  
- à de nouvelles méthodes algorithmiques ;  
- à des données issues de plateformes ;  
- à de nouveaux échanges administratifs ;  
- à une nouvelle infrastructure de calcul ;
- et désormais aux données issues de la facturation électronique [S37][S45].

La CNIL a rendu plusieurs avis successifs sur ces évolutions [S37].

Mais un avis rendu à un instant donné porte sur le dispositif qui lui est présenté à cet instant.

**GARANTIE :**

> Les modifications importantes du dispositif font l'objet d'un encadrement juridique et certaines ont donné lieu à de nouveaux avis de la CNIL.

**VULNÉRABILITÉ STRUCTURELLE :**

> La conformité d'une architecture évolutive ne peut être considérée comme définitivement acquise du seul fait qu'une version antérieure ou une modification particulière a fait l'objet d'un avis de la CNIL.

Le respect du RGPD constitue une obligation continue.

---

### Le contrôle ex post devient donc essentiel

La CNIL peut contrôler un organisme :

- à la suite d'une plainte ;  
- à la suite d'un signalement ;  
- ou de sa propre initiative [S43].

Elle peut procéder à des contrôles sur place, sur pièces, sur audition ou en ligne.

En cas de manquement, différentes mesures correctrices peuvent être mises en œuvre.

Cette distinction est fondamentale :

```
avis sur un projet
   ≠
contrôle du fonctionnement réel
   ≠
constat de conformité permanent
```

**GARANTIE INSTITUTIONNELLE :**

> L'existence d'un avis favorable ou comportant des observations ne prive pas la CNIL de ses pouvoirs ultérieurs de contrôle.

---

### Une vulnérabilité particulière apparaît avec l'évolution permanente des systèmes

Les sections 6.3 à 6.5 ont montré que plusieurs caractéristiques peuvent évoluer simultanément :

```
plus de données
   +
plus de sources
   +
plus de croisements
   +
nouveaux algorithmes
   +
nouveaux destinataires
   +
nouvelle infrastructure
```

Or chacune de ces évolutions peut modifier le niveau de risque pour les droits et libertés.

Une garantie conçue pour une architecture donnée peut donc devenir insuffisante si l'architecture change profondément.

**VULNÉRABILITÉ JURIDIQUE :**

> Dans un traitement évolutif, l'effectivité des garanties dépend de leur réévaluation lorsque la nature, l'ampleur ou les risques du traitement changent.

Cette question rejoint directement l'obligation de réexaminer l'analyse d'impact lorsque l'évolution du risque le justifie [S48].

---

### Le recours juridictionnel constitue la dernière garantie

Le RGPD reconnaît :

- le droit d'introduire une réclamation auprès d'une autorité de contrôle ;  
- le droit à un recours juridictionnel effectif contre certaines décisions de cette autorité ;  
- le droit à un recours juridictionnel effectif contre un responsable du traitement ou un sous-traitant lorsque la personne estime que ses droits ont été violés [S43].

La procédure particulière prévue par l'article 118 de la loi Informatique et Libertés rappelle également l'existence d'un recours juridictionnel [S54].

**GARANTIE JURIDIQUE :**

> Même lorsqu'une personne ne peut pas obtenir directement certaines informations protégées, le traitement n'échappe pas à tout contrôle extérieur.

---

### Mais un recours effectif suppose de pouvoir identifier suffisamment le problème

Une difficulté demeure néanmoins.

Pour contester efficacement un traitement, une personne doit généralement pouvoir identifier au moins l'existence d'un problème.

Dans une architecture complexe :

```
collecte
   ↓
croisement
   ↓
inférence
   ↓
signalement
   ↓
transmission
   ↓
conséquence
```

une erreur peut apparaître loin de la donnée initiale.

La personne peut connaître la conséquence sans nécessairement connaître immédiatement :

- la donnée qui l'a provoquée ;  
- la source de cette donnée ;  
- le rapprochement effectué ;  
- l'inférence produite ;  
- le système ayant généré le signal ;  
- les destinataires qui l'ont reçu.

**VULNÉRABILITÉ STRUCTURELLE :**

> Plus la chaîne de traitement comporte d'étapes, de responsables et de données dérivées, plus l'exercice effectif des droits dépend de la traçabilité interne du traitement et de la capacité des autorités de contrôle à reconstruire cette chaîne.

---

### Cette question dépasse CFVR et rejoint les autres infrastructures de l'enquête

Les chapitres précédents ont identifié séparément plusieurs infrastructures capables de traiter des informations concernant :

- l'identité ;  
- les transactions ;  
- la facturation ;  
- les produits ;  
- le DPP ;  
- les caractéristiques environnementales ;  
- les paiements.

Aucune source étudiée ne démontre aujourd'hui l'existence d'un système unique exploitant l'ensemble de ces informations afin de prendre une décision individuelle.

Mais si plusieurs de ces infrastructures étaient un jour rapprochées, la question des droits deviendrait plus complexe.

```
système A
identité
       ↓
système B
transaction
       ↓
système C
produit / DPP
       ↓
système D
information environnementale
       ↓
système E
paiement
```

La question ne serait plus uniquement :

> **« ai-je un droit d'accès dans chacun de ces systèmes ? »**

Elle deviendrait :

> **« puis-je reconstruire la chaîne qui a conduit à la conséquence qui me concerne ? »**

---

### Le droit d'accès à chaque composant ne garantit pas automatiquement la compréhension du système résultant

Cette distinction est essentielle.

Supposons que chaque infrastructure fournisse séparément :

```
A → accès possible
B → accès possible
C → accès possible
D → accès possible
E → accès possible
```

Il ne s'ensuit pas automatiquement :

```
A + B + C + D + E
   ↓
compréhension possible
de la décision résultante
```

**VULNÉRABILITÉ JURIDIQUE STRUCTURELLE :**

> Dans une architecture interconnectée, l'effectivité des droits doit être appréciée non seulement traitement par traitement, mais également au regard de la capacité de la personne à comprendre et contester la chaîne de traitement qui produit une conséquence à son égard.

Cette conclusion constitue un nouveau pont juridique avec les chapitres précédents.

---

### Le rapprochement avec les libertés fondamentales doit cependant rester rigoureux

Le droit à la protection des données personnelles n'est pas seulement une exigence technique.

Il participe à la protection des droits et libertés des personnes.

Mais toute collecte de données ou tout traitement administratif ne constitue pas automatiquement une violation d'une liberté fondamentale.

La question juridiquement pertinente est :

```
ingérence / traitement
   ↓
base juridique
   ↓
finalité légitime
   ↓
nécessité
   ↓
proportionnalité
   ↓
garanties
   ↓
droits effectifs
   ↓
contrôle indépendant
   ↓
recours effectif
```

Une atteinte juridiquement problématique peut apparaître lorsque cet équilibre n'est plus respecté.

---

### Le véritable point de fragilité est donc l'effectivité

Après les sections précédentes, une ligne commune apparaît.

La protection ne repose pas sur une impossibilité technique d'utiliser les données.

Elle repose sur une succession de garanties juridiques et organisationnelles :

```
limitation des finalités
   ↓
minimisation
   ↓
proportionnalité
   ↓
sécurité
   ↓
intervention humaine
   ↓
information
   ↓
accès
   ↓
rectification
   ↓
limitation
   ↓
contrôle CNIL
   ↓
recours juridictionnel
```

Plus les infrastructures deviennent capables de collecter, rapprocher et analyser des données, plus l'effectivité de chacune de ces garanties devient importante.

**VULNÉRABILITÉ STRUCTURELLE :**

> La protection des libertés ne repose donc pas uniquement sur l'existence formelle de droits, mais sur la possibilité concrète de les exercer et sur l'existence d'autorités capables de contrôler les traitements lorsque l'accès individuel doit être restreint.

---

### Questions permettant de tester cette effectivité

L'enquête peut désormais poser des questions beaucoup plus précises :

> **1. Une personne peut-elle obtenir la liste des données la concernant effectivement utilisées dans CFVR et leur origine ?**

> **2. Peut-elle connaître les destinataires auxquels les résultats la concernant ont été transmis ?**

> **3. Lorsqu'une donnée est rectifiée, quels mécanismes garantissent la correction ou le recalcul des résultats dérivés de cette donnée ?**

> **4. Une limitation demandée au titre de l'article 18 est-elle propagée aux environnements et résultats dans lesquels la donnée a déjà été utilisée ?**

> **5. Peut-on connaître le rôle joué par CFVR dans la sélection d'un dossier sans révéler les méthodes dont la confidentialité est nécessaire au contrôle fiscal ?**

> **6. Quelles informations sont effectivement communiquées à une personne lorsque son droit d'accès est exercé par l'intermédiaire de la CNIL ?**

> **7. Quels mécanismes permettent à la CNIL de reconstruire la chaîne complète lorsqu'une donnée a circulé entre plusieurs traitements ou administrations ?**

> **8. Les personnes sont-elles informées de manière suffisamment précise des nouveaux échanges DGFiP / organismes sociaux ?**

> **9. Comment les droits sont-ils exercés lorsque plusieurs responsables de traitement interviennent successivement dans une même chaîne ?**

> **10. Les évolutions de CFVR entraînent-elles une réévaluation régulière de l'effectivité des droits et des restrictions qui leur sont apportées ?**

Ces questions ne présument aucune violation.

Elles permettent de tester si les garanties sont réellement opérationnelles.

---

### Conclusion de 6.6

**AVÉRÉ :**

> CFVR prévoit l'exercice des droits d'accès, de rectification et de limitation [S45].

**RESTRICTION AVÉRÉE :**

> Le droit d'opposition prévu à l'article 21 du RGPD ne s'applique pas à CFVR [S45].

**RESTRICTION AVÉRÉE :**

> Les droits d'accès et de rectification peuvent faire l'objet de restrictions dans les conditions prévues par la loi Informatique et Libertés [S45][S54].

**GARANTIE JURIDIQUE :**

> Lorsqu'une restriction s'applique, une procédure d'exercice des droits par l'intermédiaire de la CNIL est prévue et un recours juridictionnel demeure possible [S54].

**GARANTIE JURIDIQUE :**

> Le RGPD prévoit des mécanismes permettant notamment la rectification de données inexactes, la limitation de certains traitements et la notification de certaines rectifications ou limitations aux destinataires [S43].

**GARANTIE DOCUMENTÉE :**

> La CNIL rappelle que la DGFiP et les organismes de sécurité sociale doivent informer les personnes concernées des échanges de données prévus entre eux [S37].

**GARANTIE INSTITUTIONNELLE :**

> La CNIL dispose de pouvoirs d'enquête et de contrôle indépendants de ses avis préalables et une personne peut introduire une réclamation lorsqu'elle estime que le traitement de ses données viole le RGPD [S43].

**VULNÉRABILITÉ JURIDIQUE :**

> La protection individuelle devient plus dépendante du contrôle de la CNIL et du juge lorsque les informations nécessaires à la compréhension directe du traitement peuvent légalement être restreintes.

**VULNÉRABILITÉ STRUCTURELLE :**

> Dans une architecture multi-sources, la rectification effective d'une donnée suppose de maîtriser les résultats, inférences et transmissions déjà produits à partir de cette donnée.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas de déterminer précisément comment une rectification ou une limitation est propagée aux résultats algorithmiques et aux données dérivées déjà produits dans CFVR, la PSD ou les applications alimentées par leurs résultats.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas de mesurer précisément le niveau d'information effectivement obtenu par une personne lorsque certaines informations relatives à CFVR sont soumises aux restrictions prévues par le droit fiscal.

**À ÉTABLIR :**

> Une personne peut-elle reconstruire suffisamment la chaîne ayant conduit d'une donnée source à un signalement ou à une proposition de contrôle pour exercer effectivement ses droits lorsque plusieurs traitements ont participé au résultat ?

**À ÉTABLIR :**

> Les mécanismes de traçabilité permettent-ils à la CNIL de reconstruire cette chaîne complète lorsque la personne elle-même ne peut accéder directement à certaines informations ?

**DÉDUCTIBLE JURIDIQUEMENT :**

> Si plusieurs infrastructures relatives à l'identité, aux transactions, à la facturation, aux produits, aux données environnementales ou au paiement étaient un jour interconnectées pour produire une conséquence individuelle, l'existence de droits séparés dans chaque infrastructure ne suffirait pas nécessairement à garantir un recours effectif contre le résultat produit par leur combinaison.

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas de conclure que les restrictions actuellement prévues dans CFVR privent les personnes d'un recours effectif ou sont contraires au RGPD.

---

## 6.7 Garanties propres aux infrastructures étudiées

**Statut : GARANTIES SPÉCIFIQUES ÉTABLIES / INTERFACES DOCUMENTÉES / FRONTIÈRES JURIDIQUES IDENTIFIÉES**

Les sections précédentes ont étudié les garanties générales applicables aux traitements de données :

- finalité ;  
- base juridique ;  
- minimisation ;  
- proportionnalité ;  
- sécurité ;  
- profilage ;  
- décisions automatisées ;  
- droits des personnes ;  
- contrôle par les autorités indépendantes.

Mais les infrastructures étudiées dans les chapitres précédents disposent également de garanties qui leur sont propres.

Cette section examine donc séparément :

```
facturation électronique
   +
identité numérique
   +
passeport numérique de produit
   +
données environnementales
   +
paiement / euro numérique
```

L'objectif est ensuite de déterminer ce que deviennent ces garanties lorsque plusieurs infrastructures sont susceptibles d'interagir.

---

### Première constatation : les infrastructures ne sont pas juridiquement conçues comme une base de données unique

Les chapitres précédents ont identifié plusieurs possibilités techniques d'interconnexion.

Mais les textes juridiques étudiés organisent au contraire plusieurs séparations.

On retrouve notamment :

```
données fiscales
→ finalités fiscales déterminées

identité numérique
→ contrôle de l'utilisateur
→ divulgation sélective
→ cloisonnement

DPP
→ information produit
→ droits d'accès déterminés
→ protection des données clients

paiement
→ finalités propres
→ protection des données
→ garanties spécifiques
```

**GARANTIE STRUCTURELLE :**

> Aucun des textes étudiés n'établit un droit général permettant de fusionner librement l'ensemble des données issues de ces infrastructures.

L'interopérabilité technique ne constitue donc pas une autorisation générale d'interconnexion juridique.

---

### L'identité numérique européenne comporte des garanties particulièrement fortes

Le règlement eIDAS 2 prévoit que le portefeuille européen d'identité numérique fonctionne sous le contrôle de l'utilisateur [S55].

L'utilisateur doit notamment pouvoir :

- sélectionner les données qu'il souhaite présenter ;  
- combiner différents attributs ;  
- utiliser la divulgation sélective ;  
- consulter les parties utilisatrices avec lesquelles il a interagi ;  
- connaître, le cas échéant, les données échangées ;  
- demander l'effacement de certaines données ;  
- signaler une demande suspecte à l'autorité de protection des données [S55].

Le portefeuille peut également générer et stocker localement des pseudonymes.

Le règlement envisage même des technologies permettant de démontrer qu'une condition est satisfaite sans révéler les données sous-jacentes.

Exemple :

```
attribut complet
« date de naissance : ... »
   ↓
preuve minimale
« plus de 18 ans : OUI »
```

plutôt que :

```
transmission de
l'identité complète
   +
date de naissance
   +
autres attributs inutiles
```

**GARANTIE JURIDIQUE ET TECHNIQUE :**

> L'architecture de l'identité numérique européenne intègre explicitement des mécanismes destinés à réduire la quantité d'informations révélées lors de l'accès à un service [S55].

---

### Le fournisseur du portefeuille ne doit pas devenir un observateur général de son utilisateur

Une garantie particulièrement importante apparaît dans le règlement.

Le fournisseur du portefeuille ne doit pas collecter d'informations sur son utilisation qui ne soient pas nécessaires à la fourniture du service [S55].

Il doit assurer une forme d'« inobservabilité » lui empêchant d'obtenir une visibilité générale sur les transactions réalisées par l'utilisateur.

Il lui est également interdit de combiner les données d'identification ou autres données personnelles liées au portefeuille avec les données provenant d'autres services lorsque cette combinaison n'est pas nécessaire au service du portefeuille, sauf demande expresse de l'utilisateur [S55].

Les services d'attestation d'attributs font également l'objet d'obligations de séparation.

**GARANTIE MAJEURE :**

> Le portefeuille européen d'identité numérique n'est juridiquement pas conçu pour permettre à son fournisseur de reconstruire librement l'ensemble des activités numériques de son utilisateur.

Cette garantie répond directement à l'un des risques identifiés dans les chapitres précédents.

---

### Le refus d'utiliser le portefeuille ne doit pas devenir un motif général d'exclusion

Le règlement prévoit également que l'accès aux services publics et privés, au marché du travail et à la liberté d'entreprendre ne doit pas être restreint ou rendu désavantageux du seul fait qu'une personne n'utilise pas le portefeuille européen d'identité numérique [S55].

Des moyens alternatifs doivent rester disponibles.

La conséquence est importante.

```
utilisation du wallet
   ↓
possible

   mais

refus du wallet
   ↓
ne doit pas, par lui-même,
entraîner une exclusion
```

**GARANTIE DE LIBERTÉ DE CHOIX :**

> Le cadre actuel cherche explicitement à empêcher que le portefeuille européen d'identité numérique devienne une condition générale et obligatoire d'accès aux services.

Cette garantie sera particulièrement importante à surveiller lors du déploiement pratique du dispositif.

---

### Mais le portefeuille est également conçu pour combiner des attributs

La même infrastructure possède une autre caractéristique.

Le portefeuille doit permettre à son utilisateur de :

> demander, obtenir, sélectionner, combiner, stocker, supprimer, partager et présenter des données d'identification et des attestations électroniques d'attributs [S55].

Il est donc conçu pour pouvoir présenter à une partie utilisatrice plusieurs attributs provenant de sources distinctes.

```
identité
   +
attribut A
   +
attribut B
   +
attestation C
   ↓
présentation à un service
```

Cette capacité n'est pas en elle-même une vulnérabilité.

Elle constitue précisément l'une des fonctions du portefeuille.

Mais elle crée une frontière importante.

**FRONTIÈRE JURIDIQUE :**

> La protection ne repose pas sur une impossibilité technique de combiner des attributs. Elle repose sur le contrôle de l'utilisateur, la limitation des données demandées, la finalité du service et les règles applicables à la partie utilisatrice.

---

### Les parties utilisatrices doivent déclarer les données qu'elles demandent

Une partie souhaitant utiliser le portefeuille européen d'identité numérique doit s'enregistrer et déclarer notamment l'usage prévu ainsi que les données qu'elle prévoit de demander [S55].

Elle ne doit ensuite pas demander à l'utilisateur d'autres données que celles déclarées.

Elle doit également s'identifier auprès de l'utilisateur.

**GARANTIE JURIDIQUE :**

> Une partie utilisatrice ne dispose donc pas d'un accès indifférencié aux attributs présents dans le portefeuille.

L'architecture fonctionne selon une logique d'accès déterminé :

```
service
   ↓
finalité déclarée
   ↓
attributs déclarés
   ↓
demande
   ↓
présentation sélective
```

et non :

```
service
   ↓
accès à tout le wallet
```

---

### Le DPP contient lui aussi une séparation fondamentale

Le passeport numérique de produit est conçu comme une infrastructure de données relatives au produit [S56].

Il peut contenir notamment des informations relatives :

- aux caractéristiques du produit ;  
- à sa conformité ;  
- à son cycle de vie ;  
- à sa durabilité ;  
- à certaines caractéristiques environnementales ;  
- à sa traçabilité.

Le DPP doit être associé à un identifiant unique de produit et fonctionner dans un environnement de données ouvert et interopérable [S56].

Selon les exigences applicables, il peut être établi au niveau :

```
modèle
   ou
lot
   ou
article
```

Cette dernière possibilité augmente fortement la granularité potentielle de la traçabilité du produit.

Mais le règlement introduit immédiatement une garantie importante.

---

### Le DPP n'est pas juridiquement un dossier environnemental du consommateur

Le règlement ESPR prévoit explicitement :

> les données personnelles relatives aux clients ne doivent pas être stockées dans le passeport numérique de produit sans leur consentement explicite [S56].

Cette règle casse une association qui pourrait sinon sembler évidente :

```
produit identifiable
   ↓
acheteur identifiable
```

Le premier élément ne produit pas juridiquement le second.

Un DPP peut identifier précisément un produit ou un article sans identifier son propriétaire ou son utilisateur.

**GARANTIE JURIDIQUE MAJEURE :**

> Le cadre actuel du DPP sépare explicitement l'identification du produit de l'identification personnelle du client.

**NON ÉTABLI :**

> Le DPP européen ne constitue pas, dans les textes étudiés, un « passeport environnemental individuel » enregistrant les achats ou l'empreinte environnementale personnelle d'un citoyen.

Cette distinction doit impérativement être conservée.

---

### Mais l'identifiant unique et l'interopérabilité rendent techniquement possible une autre opération

La garantie précédente ne signifie pas qu'un produit ne puisse jamais être relié à une personne dans un autre système.

Une transaction commerciale peut déjà contenir :

```
acheteur
   +
vendeur
   +
produit
   +
date
   +
montant
```

Le DPP peut de son côté contenir :

```
identifiant produit
   +
caractéristiques produit
   +
données environnementales
```

Une association externe pourrait donc théoriquement produire :

```
transaction
   ↓
produit identifié
   ↓
DPP
   ↓
caractéristiques environnementales
```

Cette possibilité technique a déjà été identifiée dans les chapitres précédents.

Mais juridiquement :

**FRONTIÈRE JURIDIQUE :**

> La protection du DPP contre le stockage de données personnelles du client ne constitue pas une interdiction générale de tout rapprochement externe entre un produit et une transaction.

Un tel rapprochement constituerait cependant un traitement distinct devant disposer de sa propre finalité, de sa propre base juridique et respecter les exigences de nécessité, de proportionnalité et de minimisation lorsqu'il implique des données personnelles [S43][S44][S53][S56].

---

### Une première asymétrie apparaît donc

Le DPP protège son propre contenu :

```
DPP
   ↓
pas de données personnelles client
sans consentement explicite
```

Mais cette garantie porte sur :

> **ce qui est stocké dans le DPP.**

Elle ne signifie pas nécessairement :

> **qu'aucun autre système ne peut utiliser l'identifiant du produit pour effectuer un rapprochement autorisé par un autre fondement juridique.**

**VULNÉRABILITÉ STRUCTURELLE :**

> Une garantie empêchant la centralisation d'une donnée personnelle dans une infrastructure ne constitue pas nécessairement une interdiction de reconstruire la relation entre plusieurs données au moyen d'un traitement externe.

C'est une distinction importante pour l'ensemble de cette enquête.

---

### L'euro numérique comporte lui aussi une garantie particulièrement forte

Le cadre proposé pour l'euro numérique contient une interdiction explicite :

> **l'euro numérique ne doit pas être de la monnaie programmable** [S57].

Une unité d'euro numérique ne doit donc pas comporter une logique intrinsèque imposant :

```
utilisable seulement
pour produit X
   ou
interdit pour produit Y
   ou
utilisable seulement
avant telle date
   ou
utilisable seulement
auprès de tel bénéficiaire
```

La BCE rappelle également que de telles limitations seraient incompatibles avec la conception retenue de l'euro numérique [S57].

**GARANTIE MONÉTAIRE MAJEURE :**

> Le cadre proposé interdit que l'euro numérique devienne intrinsèquement une monnaie dont l'utilisation serait limitée selon les biens, services, dates ou bénéficiaires.

Cette garantie répond directement à l'une des préoccupations les plus fortes pouvant apparaître autour d'une monnaie numérique de banque centrale.

---

### Mais « monnaie non programmable » ne signifie pas « paiement non conditionnable »

C'est ici qu'apparaît une frontière beaucoup plus subtile.

La proposition distingue explicitement :

```
**MONNAIE PROGRAMMABLE**
logique inscrite dans la monnaie
qui limite sa fongibilité
   ↓
INTERDITE
```

de :

```
**PAIEMENT CONDITIONNEL**
logiciel
   +
condition prédéfinie
   +
accord payeur / bénéficiaire
   +
déclenchement automatique
   ↓
PRÉVU
```

[S57]

Une opération conditionnelle est définie comme une opération déclenchée automatiquement lorsque des conditions prédéfinies convenues par le payeur et le bénéficiaire sont satisfaites.

La proposition permet même à la BCE de fournir les standards et fonctionnalités nécessaires à ces paiements, notamment la réservation de fonds [S57].

**LATITUDE JURIDIQUE EXPLICITE :**

> Le cadre proposé interdit la programmation intrinsèque de la monnaie mais autorise la programmation de certaines conditions d'exécution du paiement.

Cette distinction est fondamentale.

---

### La protection porte donc sur la monnaie, pas sur l'existence de toute logique conditionnelle autour du paiement

On peut représenter la frontière ainsi :

```
« cet euro ne peut acheter
que certaines catégories de produits »
   ↓
monnaie programmable
   ↓
INTERDITE
```

mais :

```
« exécute ce paiement
si la condition convenue X
est satisfaite »
   ↓
paiement conditionnel
   ↓
PRÉVU
```

**POINT DE FRICTION JURIDIQUE :**

> L'interdiction de la monnaie programmable ne constitue donc pas une interdiction générale de toute infrastructure capable de conditionner automatiquement l'exécution d'un paiement.

C'est probablement l'une des distinctions les plus importantes identifiées dans cette enquête.

---

### Cela ne signifie toujours pas qu'une condition environnementale soit prévue

Il faut immédiatement conserver la frontière documentaire.

Les exemples officiels de paiements conditionnels concernent notamment :

- le paiement à la livraison ;  
- le paiement à l'usage ;  
- des paiements liés à certaines étapes ;  
- certains paiements automatisés entre machines [S57].

Aucune source étudiée ne démontre qu'un paiement en euro numérique serait destiné à être conditionné :

- à un score environnemental individuel ;  
- à une empreinte carbone personnelle ;  
- à un DPP ;  
- à un historique d'achats ;  
- ou à une classification environnementale d'une personne.

**NON ÉTABLI :**

> Aucun mécanisme officiel étudié ne relie actuellement une donnée environnementale ou un DPP à l'autorisation ou au refus d'un paiement en euro numérique.

---

### Mais la condition peut provenir d'une information extérieure au paiement

Un paiement conditionnel suppose nécessairement qu'un système puisse déterminer si :

```
condition X
   =
satisfaite
   ou
non satisfaite
```

Les travaux étudiés dans les chapitres précédents ont déjà établi expérimentalement la possibilité pour un système externe de vérifier une condition utilisée pour déclencher un paiement.

La structure technique générale est donc :

```
source externe
   ↓
vérification de condition
   ↓
condition satisfaite ?
   ↓
OUI / NON
   ↓
exécution du paiement
```

La nature de la source externe dépend du service concerné.

**FRONTIÈRE JURIDIQUE :**

> Le cadre proposé autorise l'existence d'une condition externe au paiement, mais la légalité de la condition elle-même dépendrait de sa finalité, du mécanisme utilisé, des données traitées, de l'accord des parties et des autres règles applicables.

Autrement dit :

> **la capacité de conditionner existe ; la liberté juridique de choisir n'importe quelle condition n'est pas établie.**

---

### L'identité numérique et l'euro numérique possèdent une interface explicitement prévue

Un autre élément est particulièrement important.

La proposition de règlement sur l'euro numérique prévoit que les services front-end soient :

> **interopérables ou intégrés aux portefeuilles européens d'identité numérique** [S57].

Le portefeuille européen d'identité numérique permet de son côté la présentation d'identité et d'attestations d'attributs à des services publics ou privés [S55].

On dispose donc ici d'une interconnexion qui n'est plus seulement déduite techniquement :

```
portefeuille européen
d'identité numérique
   ↕
services euro numérique
```

**INTERFACE DOCUMENTÉE :**

> Le cadre proposé pour l'euro numérique prévoit explicitement une interopérabilité ou une intégration avec le portefeuille européen d'identité numérique.

Cette interface ne signifie pas que l'ensemble des attributs du portefeuille deviennent accessibles au système de paiement.

Les garanties du règlement eIDAS 2 continuent de s'appliquer.

Mais l'existence de l'interface elle-même est documentée.

---

### Le pont identité → paiement est donc établi, mais strictement limité dans sa portée

La conclusion doit être précise.

On peut désormais établir :

```
identité numérique
   ↕
interface prévue
   ↕
euro numérique
```

Mais pas :

```
tous les attributs d'identité
   ↓
tous les paiements
```

et encore moins :

```
identité
   +
environnement
   ↓
autorisation de paiement
```

**AVÉRÉ AU NIVEAU DU CADRE PROPOSÉ :**

> Une interface entre le portefeuille européen d'identité numérique et les services de paiement en euro numérique est explicitement prévue [S57].

**NON ÉTABLI :**

> Cette interface ne démontre aucune utilisation d'attributs environnementaux ou de DPP pour autoriser, refuser ou limiter un paiement.

---

### Le cadre de l'euro numérique prévoit également des protections fortes de la vie privée

Le projet distingue notamment les paiements en ligne et hors ligne [S57].

Pour les paiements hors ligne, le niveau de confidentialité recherché doit se rapprocher de celui des espèces.

Les détails des transactions hors ligne ne doivent pas être accessibles à la BCE ou aux banques centrales nationales dans les mêmes conditions que les paiements en ligne.

Pour les paiements en ligne, la proposition prévoit des mesures techniques et organisationnelles destinées à empêcher que les données transmises à l'Eurosystème permettent d'identifier directement les utilisateurs individuels [S57].

**GARANTIE DE CONFIDENTIALITÉ :**

> L'architecture proposée ne repose pas sur l'idée que la BCE devrait disposer d'un historique nominatif général des paiements individuels.

---

### Les autorités européennes de protection des données ont néanmoins demandé des garanties supplémentaires

L'EDPB et l'EDPS ont examiné la proposition d'euro numérique.

Ils reconnaissent les efforts réalisés en matière de protection de la vie privée, notamment :

- la modalité hors ligne ;  
- la protection des données dès la conception ;  
- la minimisation ;  
- le maintien du choix entre espèces et euro numérique.

Mais ils ont également demandé que la conception évite une centralisation excessive des données personnelles par la BCE ou les banques centrales nationales.

**POINT DE VIGILANCE INSTITUTIONNEL :**

> Même une architecture explicitement conçue pour offrir un haut niveau de confidentialité doit être examinée au regard de la quantité de données centralisées et de la répartition des responsabilités entre les différents acteurs.

---

### La possibilité de payer en espèces constitue elle-même une garantie importante

Le cadre proposé pour l'euro numérique ne vise pas à supprimer les espèces.

L'euro numérique doit constituer un moyen de paiement supplémentaire.

Les autorités européennes de protection des données ont expressément salué le maintien du choix entre euro numérique et espèces.

La BCE affirme également que l'euro numérique doit compléter les billets et pièces.

**GARANTIE DE LIBERTÉ DE CHOIX :**

> Dans le cadre actuellement proposé, l'euro numérique ne doit pas constituer l'unique moyen de paiement disponible.

Cette garantie réduit fortement le risque qu'une restriction propre à l'euro numérique devienne automatiquement une impossibilité générale de payer.

---

### Une architecture intéressante apparaît lorsqu'on assemble uniquement les interfaces documentées

À ce stade, il faut distinguer ce qui est réellement établi de ce qui reste hypothétique.

Les éléments documentés permettent déjà d'écrire :

```
IDENTITÉ NUMÉRIQUE
   ↓
interface prévue
   ↓
EURO NUMÉRIQUE

EURO NUMÉRIQUE
   ↓
paiements conditionnels possibles
   ↓
condition externe vérifiée

PRODUIT
   ↓
identifiant unique
   ↓
DPP
   ↓
données produit / environnementales

TRANSACTION
   ↓
peut identifier un produit
```

En revanche, le lien suivant reste absent :

```
DPP / environnement
   ↓
condition de paiement
```

**FRONTIÈRE DOCUMENTAIRE :**

> Plusieurs segments de la chaîne existent séparément ou disposent d'interfaces documentées, mais la jonction permettant à une donnée environnementale issue du DPP de déterminer une condition de paiement n'est pas établie.

---

### Le véritable point faible potentiel n'est donc pas l'absence de garanties

Les garanties sont nombreuses.

On trouve notamment :

```
IDENTITÉ
→ contrôle utilisateur
→ divulgation sélective
→ inobservabilité
→ séparation des données
→ alternatives au wallet

DPP
→ droits d'accès
→ architecture décentralisée
→ pas de données personnelles client
  sans consentement explicite

EURO NUMÉRIQUE
→ confidentialité
→ espèces maintenues
→ monnaie programmable interdite
```

Mais chacune de ces garanties protège principalement **son propre périmètre**.

La question transversale devient :

> **Que se passe-t-il lorsqu'une information quitte son infrastructure d'origine et devient une entrée juridiquement autorisée d'un autre traitement ?**

C'est là que se situe le point de friction le plus intéressant de 6.7.

---

### Une garantie locale ne constitue pas nécessairement une interdiction globale de rapprochement

Trois exemples permettent de comprendre cette distinction.

#### DPP

```
pas de données personnelles client
dans le DPP sans consentement
```

ne signifie pas automatiquement :

```
impossibilité de rapprocher ailleurs
une transaction et l'identifiant produit
```

#### Identité numérique

```
fournisseur du wallet
ne doit pas observer
toutes les transactions
```

ne signifie pas :

```
aucun service autorisé
ne peut recevoir un attribut
présenté par l'utilisateur
```

#### Euro numérique

```
monnaie programmable interdite
```

ne signifie pas :

```
paiement conditionnel interdit
```

**VULNÉRABILITÉ STRUCTURELLE :**

> Plusieurs garanties fortes identifiées dans les textes sont des garanties de périmètre : elles limitent ce qu'une infrastructure ou un acteur peut faire directement, sans nécessairement constituer une interdiction générale de tout traitement ultérieur ou de toute interface autorisée avec une autre infrastructure.

---

### C'est ici que les sections 6.2 à 6.6 reprennent toute leur importance

Une information quittant son silo ne tombe pas dans un vide juridique.

Son traitement ultérieur devrait toujours satisfaire les exigences précédemment étudiées :

```
base juridique
   ↓
finalité
   ↓
compatibilité / nouveau fondement
   ↓
nécessité
   ↓
minimisation
   ↓
proportionnalité
   ↓
sécurité
   ↓
droits
   ↓
contrôle
```

Ainsi, l'existence d'interfaces techniques ne supprime pas les garanties générales.

Mais inversement :

> **les garanties propres à chaque infrastructure ne suffisent pas nécessairement à elles seules à empêcher toute interconnexion future.**

---

### Une frontière particulièrement importante apparaît autour du consentement

Plusieurs protections identifiées reposent sur une action ou une demande de l'utilisateur.

Par exemple :

- présentation volontaire d'attributs dans le portefeuille ;  
- consentement explicite pour certaines données personnelles dans le DPP ;  
- conditions de paiement convenues entre payeur et bénéficiaire.

Cela constitue une protection importante.

Mais le consentement n'est juridiquement valable que lorsqu'il répond aux exigences applicables, notamment lorsqu'il doit être libre.

Une question apparaîtrait donc si l'accès à un bien, un service ou un moyen de paiement devenait pratiquement conditionné à l'acceptation d'un rapprochement de données.

**FRONTIÈRE JURIDIQUE :**

> L'existence formelle d'un consentement ou d'un accord ne suffirait pas nécessairement si les conditions juridiques permettant de le considérer comme libre et valable n'étaient plus réunies.

**NON ÉTABLI :**

> Les sources étudiées ne démontrent pas l'existence actuelle d'un dispositif imposant à une personne de partager des données environnementales pour accéder à un paiement ou à un service essentiel.

---

### La liberté de choix constitue donc une garantie transversale à surveiller

Deux infrastructures comportent des protections particulièrement intéressantes sur ce point.

Pour l'identité numérique :

```
wallet
   ↓
ne doit pas devenir
l'unique moyen d'accès
```

Pour l'euro numérique :

```
euro numérique
   ↓
complément des espèces
   ↓
pas remplacement obligatoire
```

Cette redondance constitue une protection forte.

Elle signifie que le cadre actuel conserve des voies alternatives.

**GARANTIE TRANSVERSALE :**

> Tant que des alternatives réelles demeurent accessibles sans désavantage injustifié, la capacité d'une infrastructure numérique à imposer seule une condition à l'ensemble de la vie économique ou administrative reste juridiquement et pratiquement limitée.

Le mot important est cependant :

> **réelles.**

Une alternative existant uniquement en droit mais devenant impraticable en pratique poserait une question différente.

---

### À ce stade, la frontière la plus importante est identifiable

L'enquête ne permet pas d'établir :

```
identité
   +
facturation
   +
DPP
   +
environnement
   +
paiement
   ↓
contrôle individuel
```

Mais elle permet désormais d'établir quelque chose de plus précis :

```
chaque infrastructure
dispose de garanties propres
   ↓
certaines interfaces
entre infrastructures
sont explicitement prévues
   ↓
certaines capacités externes
peuvent fournir des conditions
   ↓
les garanties locales
ne valent pas nécessairement
interdiction globale
d'un rapprochement futur
   ↓
tout nouveau rapprochement
devrait alors franchir
les garanties générales
étudiées en 6.1 à 6.6
```

C'est cette frontière qu'il faudra conserver pour la suite.

---

### Questions désormais ouvertes

> **1. Quelles catégories d'attributs pourront effectivement être utilisées dans l'intégration entre portefeuille européen d'identité numérique et services en euro numérique ?**

> **2. Les données présentées lors de cette interaction pourront-elles être techniquement et juridiquement réutilisées pour d'autres finalités que l'authentification ou l'exécution du service demandé ?**

> **3. Comment l'inobservabilité du portefeuille sera-t-elle auditée dans les interactions avec des services de paiement ?**

> **4. Quelles garanties empêchent qu'un identifiant produit ou transactionnel soit utilisé pour reconstruire indirectement une relation entre une personne et un DPP sans stocker cette relation dans le DPP lui-même ?**

> **5. Quelles catégories de sources externes pourront alimenter les conditions utilisées par les futurs services de paiement conditionnels ?**

> **6. Jusqu'où une condition de paiement peut-elle porter sur un attribut concernant le payeur sans devenir incompatible avec les règles de protection des données, de proportionnalité ou de non-discrimination ?**

> **7. Comment sera garantie l'existence d'alternatives réelles lorsque le portefeuille européen d'identité numérique ou l'euro numérique seront intégrés à des services publics ou privés ?**

> **8. Une architecture juridiquement conforme silo par silo peut-elle devenir disproportionnée lorsque ses interfaces permettent de reconstruire des informations que chaque silo avait précisément été conçu pour ne pas centraliser ?**

La dernière question constitue probablement le principal point de recherche transversal issu de cette section.

---

### Conclusion de 6.7

**GARANTIE ÉTABLIE :**

> Le portefeuille européen d'identité numérique prévoit le contrôle de l'utilisateur, la divulgation sélective, l'inobservabilité de son utilisation par le fournisseur et des limitations à la combinaison des données [S55].

**GARANTIE ÉTABLIE :**

> Le refus d'utiliser le portefeuille européen d'identité numérique ne doit pas, à lui seul, restreindre ou désavantager l'accès aux services publics ou privés ; des alternatives doivent demeurer disponibles [S55].

**GARANTIE ÉTABLIE :**

> Le DPP ne doit pas stocker de données personnelles relatives aux clients sans leur consentement explicite [S56].

**GARANTIE ÉTABLIE :**

> L'identification d'un produit ou d'un article dans un DPP ne constitue pas juridiquement, par elle-même, l'identification de son acheteur [S56].

**GARANTIE PROPOSÉE :**

> Le cadre proposé pour l'euro numérique interdit la monnaie programmable et maintient le principe d'une monnaie pleinement fongible [S57].

**LATITUDE JURIDIQUE EXPLICITE DANS LA PROPOSITION :**

> Cette interdiction ne s'étend pas aux paiements conditionnels : le cadre proposé prévoit expressément des paiements déclenchés automatiquement lorsque des conditions prédéfinies et convenues sont satisfaites [S57].

**INTERFACE DOCUMENTÉE DANS LA PROPOSITION :**

> Les services front-end de l'euro numérique doivent être interopérables ou intégrés aux portefeuilles européens d'identité numérique [S57].

**FRONTIÈRE JURIDIQUE :**

> L'interdiction de la monnaie programmable protège la fongibilité de la monnaie, mais ne constitue pas une interdiction générale de toute logique conditionnelle appliquée à l'exécution d'un paiement.

**VULNÉRABILITÉ STRUCTURELLE :**

> Les garanties propres aux infrastructures étudiées protègent principalement leur périmètre respectif. Elles ne constituent pas nécessairement une interdiction générale de toute association externe de données lorsqu'un autre traitement dispose d'un fondement juridique valable.

**VULNÉRABILITÉ STRUCTURELLE :**

> Une architecture peut éviter de centraliser une relation dans chacun de ses composants tout en permettant techniquement que cette relation soit reconstruite dans un traitement distinct par rapprochement de leurs identifiants ou données.

**À ÉTABLIR :**

> Les garanties de cloisonnement prévues séparément pour l'identité, les produits et les paiements suffisent-elles à empêcher qu'une interconnexion future reconstitue, dans un autre traitement, des relations que chaque infrastructure prise isolément ne conserve pas ?

**À ÉTABLIR :**

> Quelles limites juridiques s'appliqueraient au choix d'une condition externe utilisée pour déclencher un paiement conditionnel lorsque cette condition concerne des données ou attributs relatifs à une personne ?

**NON ÉTABLI :**

> Aucun élément étudié ne démontre qu'une donnée environnementale, un DPP, un historique de consommation ou un score environnemental individuel soit actuellement destiné à autoriser, refuser ou limiter un paiement en euro numérique.

**NON ÉTABLI :**

> L'euro numérique n'est pas encore adopté ni émis au 3 septembre 2026. Les dispositions étudiées relatives à son architecture juridique restent celles du cadre législatif en cours de négociation.

---

## 6.8 Évolution des finalités et du cadre juridique

**Statut : ÉVOLUTION JURIDIQUE AVÉRÉE / GARANTIES NON IMMUTABLES / FRONTIÈRES FUTURES À ÉTABLIR**

Les sections précédentes ont établi un ensemble important de garanties.

Elles montrent notamment que le droit actuel :

- limite les finalités des traitements ;  
- impose une base juridique ;  
- encadre les réutilisations ;  
- impose nécessité, proportionnalité et minimisation ;  
- protège certaines décisions individuelles contre une automatisation excessive ;  
- organise des droits et des voies de recours ;  
- impose des garanties particulières à certaines infrastructures ;  
- interdit actuellement certains usages, comme la monnaie programmable dans le cadre proposé pour l'euro numérique.

Une question reste cependant essentielle :

> **ces garanties figent-elles définitivement les finalités et les usages juridiquement autorisés ?**

La réponse est négative.

Une protection juridique applicable aujourd'hui ne constitue pas nécessairement une impossibilité juridique permanente.

---

### Il faut distinguer trois situations différentes

L'évolution d'une infrastructure peut résulter de mécanismes juridiquement très différents.

```
1. même finalité
   +
   évolution technique

2. nouvelle utilisation
   compatible avec la finalité initiale

3. nouvelle finalité
   +
   nouveau fondement juridique
```

Ces trois situations ne doivent pas être confondues.

Le RGPD encadre les traitements ultérieurs et prévoit notamment l'examen de la compatibilité d'une nouvelle finalité avec celle ayant initialement justifié la collecte [S43][S46].

Mais lorsqu'un nouveau traitement repose sur une disposition du droit de l'Union ou du droit national satisfaisant aux exigences applicables, le droit peut également créer ou modifier le fondement juridique permettant ce traitement [S43][S46][S47].

**GARANTIE JURIDIQUE :**

> Une administration ne peut pas simplement décider qu'une donnée collectée pour une finalité déterminée peut désormais être utilisée pour n'importe quelle autre finalité.

**LATITUDE JURIDIQUE :**

> Le législateur ou l'autorité réglementaire compétente peut néanmoins faire évoluer le périmètre juridiquement autorisé d'un traitement lorsque les conditions prévues par le droit supérieur sont respectées.

La différence est fondamentale.

---

### La limitation des finalités n'est donc pas une garantie d'immuabilité

Une lecture trop simple du principe de limitation des finalités conduirait à penser :

```
donnée collectée pour X
   ↓
utilisable uniquement pour X
pour toujours
```

Le droit fonctionne de manière plus complexe.

Selon les circonstances, une évolution peut résulter :

```
finalité initiale
   ↓
traitement ultérieur compatible
```

ou :

```
finalité initiale
   ↓
nouveau texte juridique
   ↓
nouveau traitement autorisé
sous nouvelles conditions
```

[S43][S46]

**VULNÉRABILITÉ JURIDIQUE :**

> Une garantie fondée sur la finalité actuelle d'un traitement limite les usages présents, mais ne garantit pas que le périmètre légal de ce traitement ne pourra jamais évoluer.

Cela ne signifie pas que toute évolution serait autorisée.

Cela signifie que la frontière est juridique et non techniquement immuable.

---

### CFVR fournit un exemple concret d'évolution progressive d'une même infrastructure

Cette possibilité n'est pas seulement théorique.

CFVR existe depuis 2014 [S58].

Depuis sa création, son cadre a été modifié à plusieurs reprises.

```
2014
création de CFVR
   ↓
2017
modification du traitement
   +
extension expérimentale
aux fraudes relatives aux particuliers
   ↓
2021
nouvelle modification
   +
articulation avec la collecte
de certaines données publiques
issues des plateformes en ligne
   ↓
2024
nouvelle modification
   ↓
2026
nouvelle modification
   +
facturation électronique
   +
nouvelles sources
   +
échanges avec organismes sociaux
   +
exploitation dans la PSD
```

[S37][S45][S58]

**AVÉRÉ :**

> Le périmètre juridique de CFVR a évolué par étapes successives depuis sa création.

Le traitement conserve pourtant la même identité générale :

> **« ciblage de la fraude et valorisation des requêtes ».**

---

### Une infrastructure peut donc conserver son nom tout en changeant profondément d'échelle

Cette observation est importante.

L'évolution d'un système public ne suppose pas nécessairement :

```
ancien système
   ↓
suppression
   ↓
nouveau système
```

Elle peut prendre la forme :

```
même infrastructure
   ↓
nouvelle source
   ↓
nouvelle catégorie de données
   ↓
nouveau destinataire
   ↓
nouvelle capacité
   ↓
nouvelle modification juridique
```

CFVR fournit précisément un exemple documenté de cette évolution [S58].

**AVÉRÉ :**

> La continuité institutionnelle d'un traitement ne signifie pas la stabilité de son périmètre de données, de sources, de destinataires ou de modalités d'exploitation.

---

### Le passage de 2017 est particulièrement révélateur

En 2017, le cadre CFVR distinguait explicitement :

```
fraudes relatives
aux professionnels
   ↓
traitement pérenne
```

et :

```
fraudes relatives
aux particuliers
   ↓
expérimentation
de deux ans
```

[S58]

Le traitement pouvait ainsi utiliser, à titre expérimental, des données concernant des particuliers sans lien avec une entreprise.

Le cadre actuel concerne désormais les fraudes relatives aux professionnels **et aux particuliers** [S45][S58].

Cette évolution fournit un exemple particulièrement clair :

```
capacité limitée / expérimentale
   ↓
évaluation et évolution juridique
   ↓
intégration dans un périmètre
plus large
```

**VULNÉRABILITÉ JURIDIQUE :**

> Le caractère expérimental ou limité d'un traitement à une date donnée ne garantit pas que ce périmètre restera expérimental ou limité.

Cela ne signifie pas que toute expérimentation devient nécessairement permanente.

Cela démontre seulement que la pérennisation constitue une évolution juridiquement possible lorsqu'un nouveau cadre l'autorise.

---

### L'intégration de la facturation électronique fournit un second exemple

Avant la réforme étudiée dans ce dossier, CFVR existait déjà.

La facturation électronique constitue une infrastructure distincte, développée pour répondre notamment à des obligations fiscales et économiques propres.

En 2026, les données issues de cette infrastructure sont expressément intégrées parmi les catégories de données utilisées par CFVR [S37][S45].

La séquence est donc documentée :

```
infrastructure A
facturation électronique
   +
infrastructure B
CFVR
   ↓
modification juridique
   ↓
données de A
utilisées dans B
```

**AVÉRÉ :**

> Une infrastructure de données existante peut ultérieurement devenir une nouvelle source juridiquement autorisée d'un traitement préexistant.

Cette observation est centrale pour l'ensemble de l'enquête.

---

### La question n'est donc plus seulement de savoir si deux infrastructures sont reliées aujourd'hui

Il faut distinguer :

```
INTERCONNEXION ACTUELLE
   ↓
question factuelle
```

de :

```
INTERCONNEXION FUTURE
   ↓
question juridique
   +
évolution éventuelle du droit
```

L'absence actuelle d'une interconnexion constitue une information importante.

Mais elle ne permet pas d'affirmer :

> **« cette interconnexion ne pourra juridiquement jamais exister ».**

Inversement, la possibilité de modifier le droit ne permet absolument pas d'affirmer :

> **« cette interconnexion sera créée ».**

**GARANTIE JURIDIQUE :**

> Toute nouvelle interconnexion impliquant des données personnelles devrait respecter le cadre juridique applicable au moment de sa mise en œuvre.

**NON ÉTABLI :**

> La possibilité juridique abstraite de faire évoluer un traitement ne démontre aucune intention institutionnelle de créer une interconnexion déterminée.

---

### Cette distinction est essentielle pour le DPP

Le cadre actuel du DPP prévoit des garanties fortes [S56].

Mais le règlement ESPR prévoit lui-même que les actes délégués applicables aux différents groupes de produits préciseront notamment :

```
données du DPP
   +
niveau modèle / lot / article
   +
acteurs disposant d'un accès
   +
données accessibles à chacun
   +
durée de disponibilité
```

[S56]

Le règlement prévoit également que lorsque d'autres dispositions du droit de l'Union exigent ou autorisent l'inclusion de données spécifiques dans le DPP, ces données peuvent y être intégrées conformément à l'acte délégué applicable.

**AVÉRÉ :**

> Le contenu concret et les droits d'accès au DPP ne sont pas entièrement figés dans le règlement-cadre : ils doivent être précisés pour les différents groupes de produits par des actes délégués [S56].

---

### Mais certaines limites du DPP demeurent inscrites dans le règlement lui-même

Cette capacité d'évolution n'efface pas les garanties supérieures.

Le règlement prévoit notamment que les données personnelles relatives aux clients ne doivent pas être stockées dans le DPP sans leur consentement explicite [S56].

Une évolution par acte délégué ne signifie donc pas :

```
Commission
   ↓
liberté illimitée
   ↓
n'importe quelle donnée
dans le DPP
```

Les actes délégués doivent rester dans le cadre de l'habilitation et respecter le droit supérieur applicable.

**GARANTIE JURIDIQUE :**

> La capacité de préciser ou de faire évoluer le contenu d'une infrastructure par des actes ultérieurs ne supprime pas les limites prévues par le règlement qui l'encadre.

---

### Le portefeuille européen d'identité numérique possède lui aussi une architecture évolutive

Le règlement eIDAS 2 fixe les garanties fondamentales du portefeuille [S55].

Mais son fonctionnement concret repose également sur des actes d'exécution déterminant des standards, spécifications et procédures techniques.

Cela concerne notamment :

- les interfaces du portefeuille ;  
- l'émission et la présentation des attributs ;  
- l'identification des parties utilisatrices ;  
- les procédures d'enregistrement ;  
- certaines modalités de certification ;  
- l'interopérabilité [S55].

Le règlement permet en outre la combinaison de plusieurs attestations d'attributs sous le contrôle de l'utilisateur.

**AVÉRÉ :**

> Le cadre juridique fondamental du portefeuille est fixé par le règlement, tandis qu'une partie importante de son fonctionnement concret est précisée par des actes d'exécution et des spécifications techniques [S55].

---

### Une évolution technique peut donc modifier fortement les capacités pratiques sans supprimer les garanties juridiques

C'est une distinction supplémentaire.

```
règle juridique stable
   ↓
nouvelle spécification
   ↓
nouvelle capacité technique
```

n'est pas nécessairement :

```
nouvelle finalité juridique
```

Mais l'évolution des standards peut augmenter :

- l'interopérabilité ;  
- le nombre d'attributs disponibles ;  
- le nombre de services compatibles ;  
- la facilité avec laquelle certaines preuves peuvent être présentées ;  
- le nombre d'interactions possibles entre infrastructures.

**VULNÉRABILITÉ JURIDIQUE :**

> L'évolution des capacités pratiques d'une infrastructure peut précéder ou accompagner l'évolution de ses usages, ce qui rend nécessaire de réexaminer régulièrement si les garanties juridiques initiales restent adaptées aux capacités réellement déployées.

---

### La frontière est encore plus évidente pour l'euro numérique

Contrairement à eIDAS 2 et au règlement ESPR, le règlement établissant l'euro numérique n'est pas encore définitivement adopté au moment de cette enquête [S57].

Les garanties étudiées en 6.7 concernant notamment :

- l'interdiction de la monnaie programmable ;  
- les paiements conditionnels ;  
- la confidentialité ;  
- l'intégration avec le portefeuille européen d'identité numérique ;

doivent donc être qualifiées selon leur statut dans le processus législatif.

**GARANTIE JURIDIQUE :**

> Tant que le texte n'est pas adopté, il ne faut pas présenter les dispositions de la proposition comme un cadre définitif et immuable.

**À ÉTABLIR :**

> Quelles garanties, définitions et possibilités techniques relatives aux paiements conditionnels et à l'interopérabilité avec le portefeuille européen d'identité numérique figureront dans le texte finalement adopté ?

---

### Le point central apparaît maintenant : la protection juridique est dynamique

Les chapitres précédents pourraient donner l'impression d'une architecture statique :

```
système
   +
finalité
   +
garanties
   =
équilibre définitif
```

L'historique de CFVR montre une réalité différente.

L'équilibre ressemble davantage à :

```
infrastructure
   ↓
premier cadre juridique
   ↓
nouvelle capacité
   ↓
nouvelle source
   ↓
modification du cadre
   ↓
nouvelles garanties
   ↓
nouvelle capacité
   ↓
nouvelle modification
   ↓
etc.
```

[S58]

**VULNÉRABILITÉ JURIDIQUE :**

> La conformité d'une infrastructure à une date donnée ne garantit pas que son périmètre futur restera identique ; elle impose au contraire de réexaminer la conformité lorsque les finalités, données, sources, destinataires ou capacités évoluent.

---

### Cela change la manière d'interpréter les garanties identifiées en 6.7

En 6.7, nous avons établi notamment :

```
DPP
→ pas de données personnelles client
  sans consentement explicite

WALLET
→ contrôle utilisateur
→ divulgation sélective
→ limitation des demandes
→ alternatives

EURO NUMÉRIQUE
→ monnaie programmable interdite
→ paiements conditionnels prévus
  dans le cadre proposé
```

Ces garanties sont réelles.

Mais elles doivent être lues comme :

> **garanties du cadre juridique applicable.**

Pas comme :

> **impossibilités techniques éternelles.**

La distinction est fondamentale.

---

### Une évolution peut également intervenir sans fusionner physiquement les bases

C'est probablement le point le plus important pour l'architecture étudiée.

Une évolution juridique n'a pas nécessairement besoin de créer :

```
MEGA BASE CENTRALE
identité
   +
factures
   +
produits
   +
environnement
   +
paiements
```

Elle pourrait théoriquement autoriser :

```
système A
   ↓
résultat / attribut

système B
   ↓
résultat / attribut

   ↓
traitement C
```

Autrement dit, la question des libertés ne dépend pas uniquement de l'existence d'une base centralisée.

Elle dépend aussi :

- des données accessibles ;  
- des identifiants permettant les rapprochements ;  
- des attributs pouvant être présentés ;  
- des résultats pouvant être transmis ;  
- des conditions pouvant être vérifiées ;  
- des conséquences attachées à ces résultats.

**VULNÉRABILITÉ JURIDIQUE :**

> Une évolution du cadre peut augmenter les possibilités de rapprochement sans nécessiter la fusion physique des infrastructures concernées.

---

### C'est précisément pourquoi les interfaces identifiées dans le Chapitre 5 et en 6.7 sont importantes

Nous avons documenté séparément :

```
transaction
↔ produit

produit
↔ DPP

DPP
↔ données environnementales

wallet
↔ attributs vérifiés

wallet
↔ services euro numérique
   dans le cadre proposé

condition externe
↔ paiement conditionnel
```

La chaîne complète :

```
identité
   +
historique économique
   +
produit
   +
environnement
   ↓
condition
   ↓
autorisation / refus / limitation
d'un paiement
```

n'est **pas établie**.

Mais la question juridique pertinente n'est plus seulement :

> **« cette chaîne existe-t-elle aujourd'hui ? »**

Elle devient également :

> **« quelles modifications juridiques seraient nécessaires pour permettre chacune de ses jonctions, et quelles garanties s'y opposeraient ? »**

C'est une question beaucoup plus précise et vérifiable.

---

### Une frontière juridique importante apparaît autour des droits et libertés

Le droit de l'Union et le droit constitutionnel ne permettent pas au législateur de supprimer librement toute protection simplement en adoptant un nouveau texte.

Une évolution demeure notamment confrontée :

```
droits fondamentaux
   ↓
vie privée
   +
protection des données
   +
nécessité
   +
proportionnalité
   +
garanties effectives
```

[S39][S44][S53]

Lorsqu'une restriction aux droits protégés par le RGPD entre dans le champ de l'article 23, elle doit notamment respecter l'essence des libertés et droits fondamentaux et constituer une mesure nécessaire et proportionnée dans une société démocratique [S47].

**GARANTIE JURIDIQUE :**

> Le fait que le législateur puisse faire évoluer le droit ne signifie pas qu'il puisse juridiquement autoriser n'importe quelle surveillance, n'importe quel profilage ou n'importe quelle restriction.

---

### La vraie vulnérabilité se situe donc entre deux affirmations fausses

Première affirmation excessive :

```
« c'est interdit aujourd'hui,
donc ce sera impossible demain »
```

Faux.

Deuxième affirmation excessive :

```
« le droit peut changer,
donc ils pourront tout faire »
```

Faux également.

La position juridiquement défendable est :

```
architecture techniquement capable
   +
usage non autorisé aujourd'hui
   ↓
évolution juridique possible
   ↓
mais soumise aux normes supérieures
   ↓
contrôle de nécessité
   +
proportionnalité
   +
droits fondamentaux
   +
garanties
   +
contrôle juridictionnel
```

---

### L'historique de CFVR montre néanmoins pourquoi cette distinction n'est pas théorique

Entre 2014 et 2026, le même traitement a connu plusieurs modifications successives [S58].

Au fil de ces évolutions apparaissent notamment :

```
plus de catégories de personnes
   +
plus de sources
   +
plus de données
   +
plus de possibilités d'analyse
   +
plus d'échanges
   +
nouvelle infrastructure de calcul
   +
facturation électronique
```

[S37][S45][S58]

Chaque évolution prise isolément peut disposer de sa justification et de ses garanties.

La question transversale devient cependant :

> **à quel moment faut-il réexaminer non seulement chaque extension séparément, mais également l'effet cumulé de toutes les extensions précédentes ?**

Cette question rejoint directement 6.5.

**À ÉTABLIR :**

> Existe-t-il une appréciation globale et périodique permettant de mesurer l'effet cumulé des modifications successives d'un traitement sur la vie privée et les libertés, au-delà de l'examen juridique de chaque modification prise séparément ?

---

### Le risque documentaire est celui d'une normalisation progressive

Il faut ici rester particulièrement prudent.

Les sources ne démontrent aucune stratégie visant à introduire progressivement un système de contrôle généralisé.

Une telle intention ne peut pas être déduite de la seule succession des textes.

Mais une propriété objective peut être étudiée :

```
extension A
→ juridiquement autorisée

extension B
→ juridiquement autorisée

extension C
→ juridiquement autorisée

extension D
→ juridiquement autorisée
```

n'implique pas automatiquement que :

```
A + B + C + D
```

ait fait l'objet d'une appréciation publique globale distincte.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas d'établir systématiquement comment l'effet cumulé de toutes les extensions successives d'une infrastructure est évalué lorsqu'une nouvelle modification est adoptée.

Cette formulation est beaucoup plus solide que d'affirmer l'existence d'une dérive.

---

### Une garantie peut aussi changer de nature lorsque l'écosystème change

Une garantie efficace dans une infrastructure isolée peut devenir moins protectrice si l'environnement technique évolue.

Exemple abstrait :

```
identifiant produit
seul
   ↓
faible capacité
d'identification personnelle
```

puis :

```
identifiant produit
   +
transaction identifiable
   +
attribut d'identité
   ↓
capacité de rapprochement
beaucoup plus importante
```

La règle propre au DPP peut rester exactement la même.

Mais l'écosystème autour du DPP a changé.

Même raisonnement pour :

```
attribut wallet
   +
service de paiement
   +
condition externe
```

**VULNÉRABILITÉ JURIDIQUE :**

> L'efficacité réelle d'une garantie de cloisonnement doit être appréciée dans l'écosystème technique et juridique dans lequel l'infrastructure fonctionne, et pas seulement à partir du contenu de son propre texte fondateur.

---

### La question ultime devient celle du changement de conséquence

Un système peut initialement servir uniquement à :

```
informer
```

puis éventuellement :

```
recommander
```

puis :

```
classer
```

puis :

```
orienter
```

puis, si le droit le permettait :

```
conditionner une décision
```

Ce dernier passage change profondément l'analyse juridique.

Les sections 6.4 et 6.5 ont montré que plus un résultat automatisé devient déterminant dans une décision produisant un effet juridique ou significatif, plus les garanties relatives aux décisions automatisées, à la nécessité et à la proportionnalité deviennent centrales [S43][S51][S53].

**GARANTIE JURIDIQUE :**

> Le fait qu'une donnée puisse juridiquement être utilisée pour informer ou orienter ne signifie pas automatiquement qu'elle puisse être utilisée pour produire une restriction individuelle.

---

### Appliqué à l'environnement, ce point devient déterminant

Le DPP et les infrastructures environnementales peuvent produire des informations concernant les caractéristiques d'un produit.

Une utilisation informative pourrait prendre la forme :

```
produit
   ↓
information environnementale
   ↓
information du consommateur
```

Une architecture beaucoup plus intrusive serait :

```
produit
   +
historique de consommation
   +
identité
   ↓
profil environnemental individuel
   ↓
conséquence sur
paiement / droit / service
```

Ces deux architectures ne sont juridiquement pas équivalentes.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement l'existence ou la préparation d'un dispositif européen attribuant aux personnes un score environnemental individuel utilisé pour limiter leurs paiements, leurs achats ou leurs droits.

**GARANTIE JURIDIQUE :**

> Le passage d'une information environnementale relative au produit à une restriction individuelle fondée sur un profil personnel constituerait un changement substantiel de traitement et devrait être examiné au regard des bases juridiques et des garanties applicables.

---

### L'absence actuelle de la chaîne complète reste donc une conclusion importante

À ce stade :

```
DPP
   ↓
information produit / environnement

wallet
   ↓
identité / attributs

paiement conditionnel
   ↓
condition externe possible
```

sont documentés séparément.

Mais :

```
DPP environnemental
   ↓
profil individuel
   ↓
condition imposée
   ↓
paiement refusé
```

reste :

> **NON ÉTABLI.**

Cette frontière ne doit pas être affaiblie.

Elle rend au contraire l'enquête plus solide.

---

### Ce qu'il faut désormais surveiller n'est donc pas une intention, mais des modifications vérifiables

Les indicateurs pertinents seraient notamment :

```
nouvelle catégorie de données
   ↓
nouvel identifiant
   ↓
nouvelle catégorie d'accédants
   ↓
nouvelle interface
   ↓
nouvelle finalité
   ↓
nouvelle possibilité de croisement
   ↓
nouvelle conséquence individuelle
```

Une évolution de l'un de ces éléments peut être documentée objectivement.

Il n'est pas nécessaire de spéculer sur les intentions.

---

### Questions ouvertes après 6.8

> **1. Quelles modifications successives ont précisément augmenté le périmètre de chaque infrastructure étudiée depuis sa création ?**

> **2. Lorsqu'une nouvelle source est ajoutée à un traitement existant, l'effet cumulé avec l'ensemble des sources déjà présentes fait-il l'objet d'une analyse distincte ?**

> **3. Comment les futures évolutions des actes délégués du DPP modifieront-elles les données disponibles, leur granularité et les catégories d'acteurs pouvant y accéder ?**

> **4. Quelles nouvelles catégories d'attestations seront progressivement utilisables dans le portefeuille européen d'identité numérique ?**

> **5. Quelles données seront réellement échangées entre le portefeuille européen d'identité numérique et les futurs services en euro numérique ?**

> **6. Quelles sources externes pourront être utilisées par les services proposant des paiements conditionnels ?**

> **7. Une nouvelle base juridique serait-elle nécessaire si une donnée environnementale relative à un produit devait être transformée en attribut relatif à une personne ?**

> **8. Quelle base juridique et quelles garanties seraient nécessaires si un tel attribut devait ensuite influencer l'accès à un paiement, un service ou un droit ?**

> **9. Existe-t-il un mécanisme permettant d'identifier le moment où plusieurs extensions juridiquement admissibles séparément produisent ensemble une architecture nécessitant une nouvelle appréciation globale de proportionnalité ?**

---

### Conclusion de 6.8

**AVÉRÉ :**

> Le périmètre juridique d'une infrastructure publique de données peut évoluer dans le temps. CFVR en fournit un exemple documenté depuis 2014 [S58].

**AVÉRÉ :**

> CFVR a connu plusieurs modifications successives concernant notamment les personnes concernées, les sources de données, les traitements associés et, en 2026, l'intégration des données issues de la facturation électronique [S37][S45][S58].

**AVÉRÉ :**

> Le règlement ESPR prévoit que le contenu concret, la granularité et les droits d'accès au DPP soient précisés pour les différents groupes de produits par des actes délégués [S56].

**AVÉRÉ :**

> Le fonctionnement concret du portefeuille européen d'identité numérique repose également sur des actes d'exécution et des spécifications techniques, dans les limites fixées par le règlement eIDAS 2 [S55].

**GARANTIE JURIDIQUE :**

> Une modification du droit ne permet pas d'écarter librement les exigences supérieures relatives aux droits fondamentaux, à la protection des données, à la nécessité et à la proportionnalité.

**LATITUDE JURIDIQUE :**

> Une finalité, une source de données, un destinataire ou une interconnexion qui ne sont pas juridiquement autorisés aujourd'hui peuvent, selon les circonstances, faire ultérieurement l'objet d'un nouveau fondement juridique, sous réserve du respect des normes supérieures applicables.

**VULNÉRABILITÉ JURIDIQUE :**

> Une garantie reposant sur le périmètre actuel d'un traitement constitue une protection présente, mais non une garantie d'immuabilité de ce périmètre.

**VULNÉRABILITÉ JURIDIQUE :**

> Une évolution peut augmenter les possibilités de rapprochement entre infrastructures sans nécessiter leur fusion physique dans une base de données unique.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas d'établir systématiquement comment l'effet cumulé de toutes les extensions successives d'une infrastructure est réévalué lorsqu'une nouvelle extension est adoptée.

**À ÉTABLIR :**

> Jusqu'où plusieurs extensions successives, chacune juridiquement encadrée séparément, peuvent-elles modifier l'équilibre global d'une infrastructure avant qu'une nouvelle appréciation d'ensemble de nécessité et de proportionnalité devienne indispensable ?

**NON ÉTABLI :**

> Aucun élément étudié ne démontre qu'une évolution juridique soit actuellement engagée afin de créer un profil environnemental individuel relié à l'identité numérique et utilisé pour autoriser, refuser ou limiter un paiement, un achat, un service ou un droit.

**NON ÉTABLI :**

> La possibilité juridique de modifier ultérieurement les finalités ou les interfaces d'une infrastructure ne constitue pas la preuve qu'une telle modification est envisagée.

---

## 6.9 Vulnérabilités juridiques et limites de l'analyse

**Statut : VULNÉRABILITÉS IDENTIFIÉES / GARANTIES SUPÉRIEURES / LIMITES FACTUELLES DE L'ENQUÊTE**

L'enquête permet désormais de répondre à une question plus importante que celle de savoir si chaque infrastructure étudiée est, prise isolément, juridiquement encadrée.

La question finale est :

> **que se passe-t-il lorsque plusieurs infrastructures juridiquement distinctes augmentent simultanément leurs capacités de collecte, d'identification, de rapprochement, d'analyse et d'action ?**

Les sections précédentes ont établi que le droit contient de nombreuses protections.

Elles ont également montré que ces protections ne constituent pas toutes des impossibilités techniques et que le périmètre juridique des infrastructures peut évoluer.

La vulnérabilité principale identifiée par cette enquête se situe précisément dans cet écart.

```
CAPACITÉ TECHNIQUE
   ↓
plus large que
   ↓
USAGE JURIDIQUEMENT AUTORISÉ
AUJOURD'HUI
```

Cette différence protège actuellement contre certains usages.

Mais elle signifie également que l'évolution du droit devient une variable essentielle de l'architecture.

---

### Première vulnérabilité : la centralisation fonctionnelle peut exister sans base centrale unique

L'enquête n'a pas identifié une base européenne unique réunissant :

```
identité
   +
factures
   +
transactions
   +
produits
   +
données environnementales
   +
paiements
```

Une telle affirmation serait incorrecte.

Les chapitres précédents ont en revanche documenté plusieurs infrastructures spécialisées disposant d'identifiants, d'interfaces, de registres, de mécanismes de vérification ou de capacités de rapprochement.

La facturation électronique française fournit un exemple particulièrement concret.

Les données issues des factures électroniques constituent désormais une source de CFVR et doivent alimenter la plateforme sécurisée des données de la DGFiP afin d'être exploitées à grande échelle [S37][S45].

CFVR rapproche déjà de nombreuses autres sources fiscales, économiques, administratives et sociales.

**AVÉRÉ :**

> Une centralisation physique dans une base unique n'est pas nécessaire pour permettre des rapprochements entre informations provenant de systèmes distincts.

**VULNÉRABILITÉ JURIDIQUE :**

> L'encadrement séparé de plusieurs infrastructures ne suffit pas nécessairement à apprécier les conséquences résultant de leur combinaison lorsqu'elles deviennent interopérables ou lorsque les résultats produits par l'une peuvent être utilisés par une autre.

La question déterminante n'est donc pas seulement :

> **« où sont stockées les données ? »**

mais également :

> **« quelles informations peuvent être reliées, vérifiées, transmises ou utilisées pour produire une conséquence ? »**

---

### Deuxième vulnérabilité : une finalité légalement limitée aujourd'hui peut évoluer demain

La section 6.8 a établi que CFVR fournit déjà un exemple historique de modifications successives d'un même traitement [S58].

Une infrastructure peut conserver son existence institutionnelle tout en voyant évoluer :

- ses sources ;  
- ses catégories de données ;  
- les personnes concernées ;  
- ses destinataires ;  
- ses capacités techniques ;  
- ses modalités d'exploitation.

**GARANTIE JURIDIQUE :**

> Une administration ne peut pas modifier librement une finalité ou réutiliser librement des données en dehors du cadre juridique applicable.

**VULNÉRABILITÉ JURIDIQUE :**

> L'absence actuelle d'un usage ne constitue pas nécessairement une interdiction juridique définitive : un nouveau texte peut modifier le périmètre autorisé, sous réserve du respect du droit supérieur.

Cette distinction interdit deux conclusions opposées.

```
« ce n'est pas autorisé aujourd'hui
donc ce sera toujours impossible »
```

n'est pas démontré.

Mais :

```
« le droit peut évoluer
donc cet usage sera autorisé demain »
```

ne l'est pas davantage.

---

### Troisième vulnérabilité : l'accumulation peut devenir plus importante que chaque extension prise isolément

L'analyse de CFVR révèle une difficulté transversale.

Une succession peut prendre la forme :

```
extension A
   +
extension B
   +
nouvelle source C
   +
nouvel échange D
   +
nouvelle capacité E
```

Chacune peut être examinée juridiquement lors de son introduction.

Mais l'enjeu final devient :

```
A + B + C + D + E
   ↓
CAPACITÉ GLOBALE
```

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas d'établir systématiquement comment l'effet cumulé de toutes les extensions successives d'une infrastructure est réévalué indépendamment de l'examen de chaque nouvelle modification.

Cette question devient particulièrement importante lorsque progressent simultanément :

```
volume
   +
nombre de sources
   +
précision
   +
interopérabilité
   +
capacité algorithmique
   +
nombre de destinataires
```

---

### Quatrième vulnérabilité : l'interopérabilité peut produire une capacité nouvelle sans fusion des systèmes

Les infrastructures étudiées sont de plus en plus conçues autour :

- d'identifiants ;  
- d'interfaces ;  
- de registres ;  
- d'attestations vérifiables ;  
- de mécanismes de présentation d'attributs ;  
- de services capables de vérifier des conditions ;  
- de standards communs.

Cela permet une architecture dans laquelle une infrastructure n'a pas nécessairement besoin de recevoir toutes les données brutes d'une autre.

```
SYSTÈME A
   ↓
attribut / preuve / résultat

SYSTÈME B
   ↓
vérification

SYSTÈME C
   ↓
conséquence
```

**VULNÉRABILITÉ JURIDIQUE :**

> Une infrastructure distribuée peut produire des conséquences comparables à celles d'un système centralisé sans nécessiter la constitution d'une base contenant physiquement l'intégralité des données concernées.

Cette propriété rend l'analyse des seules bases de données insuffisante.

Il faut également examiner les interfaces.

---

### Cinquième vulnérabilité : le passage de l'information à la conséquence

Cette frontière constitue probablement la plus importante de l'ensemble du chapitre.

Une donnée peut être utilisée pour :

```
INFORMER
```

puis :

```
VÉRIFIER
```

puis :

```
CLASSER
```

puis :

```
ORIENTER
```

et éventuellement :

```
CONDITIONNER
```

Ces fonctions ne produisent pas les mêmes conséquences juridiques.

CFVR fournit déjà un exemple de cette distinction.

Les résultats algorithmiques peuvent orienter les agents, mais la CNIL exige qu'ils ne remplacent pas leur analyse et que la décision humaine demeure effective [S37][S51].

**GARANTIE JURIDIQUE :**

> L'autorisation d'utiliser une donnée pour informer, détecter ou vérifier ne constitue pas automatiquement une autorisation de l'utiliser pour produire une restriction individuelle.

**VULNÉRABILITÉ JURIDIQUE :**

> Plus une donnée ou un résultat algorithmique devient déterminant pour l'accès à un paiement, un service, un droit ou une autre possibilité importante, plus les exigences relatives à la base juridique, à la proportionnalité, à l'exactitude, à la transparence, à la contestation et aux décisions automatisées deviennent déterminantes.

---

### Sixième vulnérabilité : une erreur peut changer de nature lorsqu'elle traverse plusieurs infrastructures

Les sections précédentes ont identifié les droits d'accès et de rectification.

Mais une architecture interconnectée pose une difficulté supplémentaire.

```
donnée A erronée
   ↓
traitement B
   ↓
classification C
   ↓
attribut D
   ↓
décision E
```

Corriger A ne garantit pas techniquement, à lui seul, que :

```
B
C
D
E
```

aient tous été recalculés, corrigés ou neutralisés.

Le droit prévoit différentes obligations de rectification, de limitation et de communication aux destinataires lorsque les conditions correspondantes sont réunies [S43].

**VULNÉRABILITÉ JURIDIQUE :**

> Dans une architecture distribuée, l'effectivité du droit de rectification dépend non seulement de la correction de la donnée source, mais également de la capacité à identifier et corriger les conséquences dérivées encore associées à cette donnée.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées ne permettent pas d'établir l'existence d'un mécanisme transversal permettant à une personne de connaître puis de faire corriger automatiquement toutes les données dérivées ou conséquences propagées à travers plusieurs infrastructures juridiquement distinctes.

---

### Septième vulnérabilité : la protection dépend parfois du maintien d'une séparation fonctionnelle

Plusieurs garanties identifiées reposent sur des frontières.

Pour CFVR :

```
algorithme
   ↓
signalement
   ↓
analyse humaine
   ↓
décision
```

Pour le DPP :

```
information produit
   ≠
profil personnel du consommateur
```

Pour l'euro numérique dans le cadre proposé :

```
paiement conditionnel
   ≠
monnaie programmable
```

Pour le portefeuille européen :

```
présentation d'un attribut nécessaire
   ≠
divulgation systématique
de l'ensemble de l'identité
```

Ces séparations constituent de véritables garanties.

Mais leur efficacité dépend de leur maintien.

**VULNÉRABILITÉ JURIDIQUE :**

> Lorsqu'une protection repose sur une séparation entre deux fonctions techniquement rapprochables, toute évolution réduisant cette séparation doit faire l'objet d'une nouvelle analyse juridique.

---

### Huitième vulnérabilité : l'euro numérique pourrait être créé sans consentement individuel de chaque citoyen

Il faut ici distinguer création d'une monnaie et obligation individuelle de l'utiliser.

Le cadre européen proposé prévoit une procédure législative permettant d'établir l'euro numérique.

Une fois ce cadre adopté, la décision d'émettre ou non l'euro numérique appartiendrait à la BCE [S57].

Il ne s'agit donc pas d'un mécanisme reposant sur le consentement individuel de chaque citoyen à la création de cette nouvelle forme de monnaie.

**AVÉRÉ :**

> La création éventuelle de l'euro numérique relève du processus institutionnel et législatif européen puis, dans le cadre envisagé, d'une décision d'émission de la BCE ; elle n'est pas conditionnée à l'accord individuel de chaque utilisateur.

Mais cette constatation ne signifie pas :

```
euro numérique créé
   =
obligation pour chaque citoyen
d'abandonner les espèces
```

Le cadre actuellement négocié prévoit au contraire la coexistence de l'euro numérique avec les espèces et des mesures destinées à préserver l'accès et l'acceptation du cash [S57].

**NON ÉTABLI :**

> Aucun élément étudié ne permet d'affirmer que le cadre actuel prévoit la suppression des espèces ou l'obligation générale pour chaque citoyen d'utiliser exclusivement l'euro numérique.

---

### Neuvième vulnérabilité : le contrôle d'une monnaie numérique et le contrôle de l'usage de chaque unité ne sont pas juridiquement équivalents

Une infrastructure de monnaie numérique de banque centrale implique nécessairement des règles concernant notamment :

- son émission ;  
- sa distribution ;  
- son fonctionnement ;  
- ses intermédiaires ;  
- ses limites éventuelles de détention ;  
- ses mécanismes de paiement.

Le cadre actuellement proposé envisage effectivement des limites de détention [S57].

Mais une autre frontière existe.

La BCE considère que limiter intrinsèquement :

```
où
 +
quand
 +
à qui
```

une unité d'euro numérique peut être dépensée reviendrait à créer une monnaie programmable incompatible avec son caractère de monnaie pleinement fongible et avec son cours légal [S57].

**GARANTIE JURIDIQUE :**

> Le cadre proposé exclut la transformation de l'euro numérique en monnaie programmable dont les unités imposeraient intrinsèquement des restrictions concernant les biens, services, lieux, moments ou bénéficiaires auxquels elles pourraient être utilisées.

Cette garantie est importante.

Elle ne doit pas être confondue avec les paiements conditionnels.

---

### Dixième vulnérabilité : les paiements conditionnels créent néanmoins une interface avec des conditions externes

Les chapitres précédents ont documenté la possibilité technique et expérimentale d'utiliser une condition vérifiée extérieurement afin de déclencher un paiement.

Le cadre proposé pour l'euro numérique distingue précisément :

```
MONNAIE PROGRAMMABLE
   ↓
restriction intrinsèque
de la monnaie
   ≠
PAIEMENT CONDITIONNEL
   ↓
paiement déclenché
selon une condition convenue
```

[S22][S27][S28][S57]

**AVÉRÉ :**

> Le cadre proposé interdit la monnaie programmable tout en permettant le développement de services de paiement conditionnel.

Cette distinction constitue simultanément :

```
une GARANTIE
   +
une INTERFACE À SURVEILLER
```

La garantie est que la monnaie elle-même ne peut pas être limitée à certains usages.

L'interface à surveiller concerne la nature des conditions utilisées par les services de paiement.

---

### C'est ici que la question environnementale doit être formulée avec une précision maximale

Les chapitres précédents ont établi :

```
produit
   ↓
DPP
   ↓
données environnementales
```

et séparément :

```
condition externe
   ↓
vérification
   ↓
paiement conditionnel
```

Mais ils n'ont pas établi :

```
identité
   ↓
historique d'achats
   ↓
score environnemental personnel
   ↓
quota
   ↓
autorisation / refus de paiement
```

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement l'existence, le déploiement ou l'adoption juridique d'un « pass environnemental » individuel utilisant les données du DPP pour déterminer si une personne peut ou non effectuer un paiement.

Cette conclusion doit rester explicite.

Mais elle n'épuise pas la question juridique.

---

### La vraie question devient : quelles protections s'activeraient si cette frontière était franchie ?

Une architecture hypothétique :

```
IDENTITÉ
   +
TRANSACTIONS
   +
PRODUITS
   +
DONNÉES ENVIRONNEMENTALES
   ↓
PROFIL INDIVIDUEL
   ↓
CONDITION
   ↓
PAIEMENT / SERVICE / DROIT
```

ne pourrait pas être analysée comme une simple extension technique.

Elle devrait notamment être examinée au regard :

- de sa base juridique ;  
- de sa finalité ;  
- de la nécessité ;  
- de la proportionnalité ;  
- de la minimisation ;  
- des droits d'accès et de rectification ;  
- des règles relatives au profilage ;  
- des décisions automatisées lorsque leurs conditions sont réunies ;  
- des droits fondamentaux affectés ;  
- des voies de recours.

[S43][S44][S47][S51][S53]

**GARANTIE JURIDIQUE :**

> Une infrastructure techniquement capable de produire une restriction n'est pas juridiquement autorisée à la produire du seul fait que cette capacité existe.

---

### Et même une nouvelle loi ne constitue pas un pouvoir sans limite

C'est probablement la frontière juridique la plus importante de ce chapitre.

Une nouvelle loi ou un nouveau règlement peut faire évoluer les usages autorisés.

Mais :

```
NOUVELLE LOI
   ≠
POUVOIR JURIDIQUE ILLIMITÉ
```

Lorsqu'une mesure limite des droits fondamentaux protégés par le droit de l'Union, cette limitation doit notamment :

```
être prévue par la loi
   +
respecter le contenu essentiel du droit
   +
être nécessaire
   +
être proportionnée
   +
répondre effectivement
à un objectif d'intérêt général
ou protéger les droits d'autrui
```

[S39][S44]

**GARANTIE JURIDIQUE :**

> L'évolution du droit peut déplacer certaines frontières, mais elle reste elle-même soumise aux normes juridiques supérieures et au contrôle juridictionnel.

Cette garantie constitue la limite à l'idée selon laquelle :

> **« il suffirait de changer la loi pour pouvoir tout faire ».**

---

### La réforme de la facturation électronique constitue néanmoins un changement d'échelle majeur

Il faut ici revenir au point de départ de l'enquête.

Une facture électronique structurée n'est pas seulement un PDF envoyé autrement.

Elle transforme des informations économiques auparavant dispersées en données :

```
structurées
   +
standardisées
   +
exploitables automatiquement
   +
transmissibles
   +
rapprochables
   +
analysables à grande échelle
```

Les chapitres 1 et 2 ont établi la nature et le cycle de ces données.

Le Chapitre 5 a étudié les possibilités d'interconnexion.

Le présent chapitre a montré que certaines données de facturation électronique sont désormais intégrées à CFVR et exploitées dans une infrastructure algorithmique capable de traiter une volumétrie de plusieurs milliards de factures annuelles [S37][S45].

**AVÉRÉ :**

> La réforme augmente fortement la quantité de données économiques structurées susceptibles d'être traitées automatiquement par l'administration fiscale.

---

### Mais « centraliser tout » serait une conclusion excessive

Le dossier ne démontre pas :

```
FACTURATION ÉLECTRONIQUE
   ↓
BASE UNIQUE
   ↓
toute l'identité
   +
tous les produits
   +
tout l'environnement
   +
tous les paiements
```

**NON ÉTABLI :**

> La réforme française de la facturation électronique ne constitue pas, sur la base des sources étudiées, une base centrale réunissant l'ensemble des infrastructures analysées dans cette enquête.

La conclusion exacte est différente :

> **elle crée une nouvelle couche massive de données économiques structurées qui peut devenir une source pour d'autres traitements lorsque le droit l'autorise.**

CFVR en fournit désormais un exemple concret.

---

### C'est précisément ce qui fait de la facturation électronique une infrastructure structurante

Le point critique n'est donc pas :

> **« la facture électronique contrôle déjà tout ».**

Le point documenté est :

```
ACTIVITÉ ÉCONOMIQUE
   ↓
DONNÉES STRUCTURÉES
   ↓
TRANSMISSION
   ↓
TRAITEMENT À GRANDE ÉCHELLE
   ↓
CROISEMENT
   ↓
ANALYSE ALGORITHMIQUE
```

Cette chaîne existe désormais dans le domaine fiscal étudié [S37][S45].

**VULNÉRABILITÉ JURIDIQUE :**

> Plus une infrastructure transforme une activité économique diffuse en données structurées, standardisées et interopérables, plus l'évolution de ses finalités, de ses destinataires et de ses possibilités de rapprochement devient déterminante pour les libertés.

---

### La vulnérabilité fondamentale n'est donc pas une fonction cachée

Au terme de l'enquête, aucune source n'a révélé :

```
bouton secret
« contrôle total »
```

La vulnérabilité identifiée est plus structurelle.

```
NUMÉRISATION
   ↓
STRUCTURATION
   ↓
IDENTIFICATION
   ↓
INTEROPÉRABILITÉ
   ↓
CROISEMENT
   ↓
ANALYSE
   ↓
CONDITION / DÉCISION POSSIBLE
```

À chaque étape existent des garanties.

Mais chaque étape augmente également la capacité potentielle de l'étape suivante.

---

### La protection des libertés dépend donc moins de l'existence des capacités que des frontières imposées à leur usage

Cette enquête montre finalement que deux réalités peuvent être vraies simultanément.

Première réalité :

> **les infrastructures étudiées ne constituent pas aujourd'hui un système juridiquement autorisé de contrôle général des achats, de l'identité, de l'environnement et de la monnaie.**

Deuxième réalité :

> **elles augmentent objectivement les capacités techniques d'identification, de structuration, de rapprochement, de vérification et d'automatisation disponibles dans l'écosystème numérique européen.**

Il n'y a aucune contradiction entre ces deux constats.

C'est précisément l'espace situé entre eux que le droit doit protéger.

---

### Les lignes rouges deviennent alors identifiables

L'enquête permet désormais de définir des changements qui nécessiteraient une réévaluation particulièrement rigoureuse :

> **1. utilisation d'un identifiant commun permettant de relier systématiquement identité, achats, produits et paiements ;**

> **2. transformation des informations environnementales relatives aux produits en profil environnemental individuel ;**

> **3. utilisation de ce profil pour produire une conséquence sur un paiement, un service ou un droit ;**

> **4. transformation d'une aide algorithmique en mécanisme déterminant pratiquement la décision humaine ;**

> **5. disparition ou réduction substantielle de la possibilité d'utiliser un moyen de paiement non associé au même niveau de traçabilité ;**

> **6. extension des finalités permettant l'utilisation croisée de données initialement collectées dans des infrastructures distinctes ;**

> **7. impossibilité pratique pour une personne de connaître, corriger ou contester les données et résultats dérivés utilisés à son égard ;**

> **8. multiplication d'extensions séparément justifiées sans évaluation publique suffisante de leur effet cumulé.**

Aucun de ces points ne doit être présenté comme réalisé lorsqu'il ne l'est pas.

Ils constituent des critères de surveillance vérifiables.

---

### Ce que l'enquête ne permet pas d'affirmer

**NON ÉTABLI :**

> Il n'est pas établi que l'Union européenne ou la France mettent actuellement en place un système destiné à attribuer un score environnemental individuel aux citoyens.

**NON ÉTABLI :**

> Il n'est pas établi que les données du DPP seront utilisées pour déterminer l'autorisation ou le refus des achats d'une personne.

**NON ÉTABLI :**

> Il n'est pas établi que l'euro numérique permettra à la BCE d'autoriser ou d'interdire les achats d'une personne en fonction des produits qu'elle souhaite acheter.

**NON ÉTABLI :**

> Il n'est pas établi que la facturation électronique, le DPP, le portefeuille européen d'identité numérique et l'euro numérique seront réunis dans une infrastructure unique de contrôle.

**NON ÉTABLI :**

> Il n'est pas établi que les espèces seront supprimées lors de l'introduction éventuelle de l'euro numérique.

Ces limites ne diminuent pas l'enquête.

Elles en définissent la solidité.

---

### Ce qu'elle permet en revanche d'établir

**AVÉRÉ :**

> La facturation électronique transforme une partie importante de l'activité économique en données structurées pouvant être exploitées automatiquement.

**AVÉRÉ :**

> Certaines de ces données sont désormais destinées à alimenter CFVR et la plateforme sécurisée des données de la DGFiP [S37][S45].

**AVÉRÉ :**

> CFVR combine déjà de nombreuses sources et utilise des méthodes algorithmiques pour détecter des anomalies et orienter le contrôle fiscal [S37].

**AVÉRÉ :**

> Le DPP permet d'associer à des produits des informations structurées pouvant notamment inclure des informations environnementales [S56].

**AVÉRÉ :**

> Le portefeuille européen d'identité numérique permet la présentation et la vérification d'attributs électroniques selon le cadre étudié [S55].

**AVÉRÉ :**

> Le cadre proposé pour l'euro numérique distingue et interdit la monnaie programmable tout en permettant des services de paiement conditionnel [S57].

**AVÉRÉ :**

> Les finalités, sources et périmètres de certaines infrastructures publiques peuvent évoluer juridiquement dans le temps, comme l'historique de CFVR le démontre [S58].

**GARANTIE JURIDIQUE :**

> Ces capacités techniques ne peuvent pas être librement combinées pour produire n'importe quelle conséquence individuelle : leur utilisation demeure soumise aux bases juridiques, aux finalités autorisées, aux droits fondamentaux et aux exigences de nécessité et de proportionnalité.

---

### Conclusion de 6.9

Le résultat de l'enquête n'est donc ni :

```
« tout est déjà connecté »
```

ni :

```
« les garanties actuelles rendent
toute évolution impossible »
```

Le résultat est plus précis.

```
INFRASTRUCTURES DISTINCTES
   ↓
CAPACITÉS CROISSANTES
   ↓
INTEROPÉRABILITÉ CROISSANTE
   ↓
POSSIBILITÉS DE RAPPROCHEMENT
   ↓
USAGES LIMITÉS PAR
LE DROIT ACTUEL
   ↓
MAIS CADRE JURIDIQUE
SUSCEPTIBLE D'ÉVOLUER
   ↓
SOUS CONTRÔLE DES
DROITS FONDAMENTAUX
```

**VULNÉRABILITÉ JURIDIQUE :**

> Le principal risque identifié n'est pas l'existence démontrée d'un système unique de contrôle, mais la possibilité que des extensions successives de finalités, d'accès, d'interfaces ou de conséquences rapprochent progressivement des infrastructures initialement séparées.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques permettent généralement d'étudier chaque infrastructure et chaque modification juridique séparément, mais beaucoup moins facilement d'évaluer l'effet cumulé de l'ensemble de l'écosystème sur les capacités d'identification, de rapprochement et de décision.

**GARANTIE JURIDIQUE :**

> Même lorsqu'une évolution est décidée par le législateur, les limitations apportées aux droits fondamentaux demeurent soumises aux exigences de légalité, de respect du contenu essentiel des droits, de nécessité et de proportionnalité.

**NON ÉTABLI :**

> L'enquête ne démontre actuellement ni l'existence d'un « pass environnemental » individuel, ni l'utilisation d'un profil environnemental pour contrôler les paiements, ni une architecture unique reliant automatiquement facturation électronique, identité numérique, DPP et euro numérique afin de restreindre les droits ou achats des citoyens.

**CONCLUSION :**

> **La question déterminante n'est donc pas de savoir si l'infrastructure permet déjà un contrôle généralisé. Elle est de savoir si les frontières juridiques qui séparent aujourd'hui collecte, information, identification, rapprochement, profilage et décision continueront à évoluer au même rythme que les capacités techniques qui permettent de les franchir.**

Et c'est précisément pour cette raison que l'analyse doit rester évolutive :

> **chaque nouvelle source de données, chaque nouvel identifiant, chaque nouvelle interface, chaque nouvelle finalité et chaque nouvelle conséquence attachée à ces infrastructures doit être examinée non seulement isolément, mais également pour ce qu'elle permet lorsqu'elle est combinée avec ce qui existe déjà.**
