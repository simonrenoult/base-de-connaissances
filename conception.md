# 🧱 Conception


## Général

- [x] Quatre règles pour un design simple : https://blog.jbrains.ca/permalink/the-four-elements-of-simple-design
- https://tqdev.com/2018-the-boring-software-manifesto
- https://engagor.github.io/blog/2020/10/05/a-few-tips-for-making-your-code-easier-to-reason-about/
- https://www.deconstructconf.com/2019/hillel-wayne-what-we-can-learn-from-software-history
- https://cutlefish.substack.com/p/tbm-3553-basic-prioritization-questions
- http://www.laputan.org/mud/
- https://matthiasnoback.nl/2020/07/key-design-patterns/
- https://evelynvankelle.com/2020/06/29/if-something-is-too-complex-to-understand-it-must-be-wrong/
- https://www.lilobase.me/savoir-faire-des-choses-compliquees-ne-fait-pas-de-vous-un-bon-developpeur/
- https://jessitron.com/2020/05/08/one-secret-to-quality-software/
- https://github.com/devcrafting/architecture-styles
- https://sandimetz.com/blog/2016/1/20/the-wrong-abstraction
- https://simpleprogrammer.com/respecting-abstraction/



## Clean Archiecture

- [x] Clean Architecture vs DDD : https://khalilstemmler.com/articles/software-design-architecture/domain-driven-design-vs-clean-architecture/ 
- [x] Origine des termes de la Clean Architecture : https://blog.octo.com/application-domain-infrastructure-des-mots-de-la-layered-hexagonal-clean-architecture/
- [x] DDD, CQS et Clean Architecture en TypeScript : https://khalilstemmler.com/articles/enterprise-typescript-nodejs/application-layer-use-cases/
- https://herbertograca.com/2017/09/28/clean-architecture-standing-on-the-shoulders-of-giants/
- [x] Les mauvais côtés de la Clean Architecture : https://www.jamesmichaelhickey.com/clean-architecture/
- https://jimmybogard.com/vertical-slice-architecture/



## Couplage

### Pourquoi préférer un système faiblement couplé ("loose coupling") ?

> Plus petit est le système à maintenir plus rapides sont les développements.

> Plus petit est le système à maintenir plus rapide et simple sont la rédaction et l'exécution des tests.

> Des systèmes couplés sont plus complexes à maintenir car faire évoluer un sous-ensemble du système requiert de faire évoluer les autres sous-ensembles dépendants.

> Dans un système faiblement couplé, l'impact d'un défaut est plus limité.

> Plus petit est le système mieux il sera compris.

> Des systèmes couplés sont plus complexes à comprendre en raison du nombre d'élément à considérer.

> Un système couplé sera plus facile à migrer dans un autre système.

> Des systèmes couplés sont moins performants car leur performance est limité à celle du moins performant d'entre eux.

> Loi de Déméter (1987) : un objet A peut appeler une méthode d'un objet B, mais A ne peut pas utiliser B pour accéder à un troisième objet via B et requérir ses services. Le système est alors plus maintenable car A ne dépend pas de la structure interne de B. B peut alors faire évoluer sa structure interne indépendament de A.

### Ressources

- [x] The pragmatic programmer, Orthogonality : https://flylib.com/books/en/1.315.1.23/1
- [x] The pragmatic programmer, 
Decoupling and the Law of Demeter
 : https://flylib.com/books/en/1.315.1.52/1
- [ ]  Working Effectively with Legacy Code, Dependency-Breaking Techniques (chap 25)
- [ ]  Clean Architecture, Component Cohesion (chap 13)
- [ ]  Clean Architecture, Component Coupling (chap 14)
- [ ]  Clean Architecture, Independance (chap 16)
- [ ]  Refactoring, Divergent Change : https://martinfowler.com/books/refactoring.html
- [ ]  Refactoring, Shotgun Surgery : https://martinfowler.com/books/refactoring.html
- [ ]  Refactoring, Message Chain : https://martinfowler.com/books/refactoring.html
- [x] https://fr.wikipedia.org/wiki/Loi_de_D%C3%A9m%C3%A9ter
- [x] https://jonhilton.net/2016/03/09/why-coupling-will-destroy-your-application-and-how-to-avoid-it/
- [x] https://www.ben-morris.com/why-is-loose-coupling-between-services-so-important/
- [ ] https://www.lilobase.me/votre-application-a-besoin-de-son-jardin-secret-attention-a-la-localite-de-linformation/



## CQRS

### Pourquoi ?

> Dans un système complexe, le processus métier ne peut être connu de tous de manière exhaustive. 
> Dès lors, il convient d'encapsuler les différentes opérations au sein d'abstractions.
> On parle de **Commande** pour les ordres envoyés au système et de **Queries** pour les questions
> posées au système.

> Distinguer **Commandes** et **Queries** permet de faire émerger un système **CQS** et non **CQRS**.
> C'est la distinction de la localisation de la donnée et des modèles ainsi mis à jour qui donnent
> la lettre R au CQRS. 

### Références

- https://codeopinion.com/cqrs-without-multiple-data-sources/
- Keynote - Udi Dahan - DDD Europe 2020 : https://www.youtube.com/watch?v=-iuMjjKQnhg&feature=youtu.be
- Creating IDs with CQRS and Event Sourcing in Java and .NET : https://thomasjaeger.wordpress.com/2016/01/09/creating-ids-with-cqrs-and-event-sourcing-in-java-and-net/
- https://matthiasnoback.nl/2018/05/when-and-where-to-determine-the-id-of-an-entity/
- [x] CQRS, Fonctionnel, Event Sourcing & Domain Driven Design - Arnaud Lemaire - PHP Tour 2018 : https://www.youtube.com/watch?v=qBLtZN3p3FU&feature=youtu.be
- https://codeopinion.com/is-cqrs-complicated/
- https://blog.ploeh.dk/2014/08/11/cqs-versus-server-generated-ids/
- https://thinkbeforecoding.com/post/2013/07/28/Event-Sourcing-vs-Command-Sourcing
- [x] https://herbertograca.com/2017/10/19/from-cqs-to-cqrs/
- [x] https://matthiasnoback.nl/2017/03/bash-practices-cqs-and-return-values/
- Greg Young - CQRS and Event Sourcing - Code on the beach 2104 : https://www.youtube.com/watch?v=JHGkaShoyNs



## Dette technique

- https://jp-lambert.me/recenser-et-suivre-la-dette-technique-4146f1e5c7b9
- [x] https://www.lilobase.me/a-complexite-egale-des-realites-tres-differentes/
- https://blog.octo.com/la-fin-de-la-dette-technique-resoudre-les-conflits/



## Domain Driven Design

- [ ] Le DDD est-il adapté à tous vos projets ? https://www.lilobase.me/le-domain-driven-design-est-il-adapte-a-tous-vos-projets/amp/?__twitter_impression=true&s=09
- [x] DDD, CQS et Clean Architecture en TypeScript : https://khalilstemmler.com/articles/enterprise-typescript-nodejs/application-layer-use-cases/
- https://github.com/ardalis/DDD-NoDuplicates
- https://gojko.net/2010/06/11/udi-dahan-the-biggest-mistakes-teams-make-when-applying-ddd/
- https://blog.codecentric.de/en/2020/07/hexagon-schmexagon-1/
- https://enterprisecraftsmanship.com/posts/domain-model-purity-completeness/
- https://virtualddd.com/learning-ddd/
- [x] CQRS, Fonctionnel, Event Sourcing & Domain Driven Design - Arnaud Lemaire - PHP Tour 2018 https://www.youtube.com/watch?v=qBLtZN3p3FU&feature=youtu.be
- https://philippe.bourgau.net/how-to-use-event-storming-to-introduce-domain-driven-design/
- https://weronikalabaj.com/the-harsh-reality-of-a-domain-breakthrough/
- https://github.com/ddd-crew/ddd-starter-modelling-process
- https://www.jamesmichaelhickey.com/consistency-boundary/
- https://medium.com/nick-tune-tech-strategy-blog/strategic-ddd-remote-collaboration-toolkit-ab3176f878aa
- https://speakerdeck.com/mploed/aligning-organization-and-architecture-with-strategic-ddd
- LA STRATEGIE DERRIERE LE DOMAIN DRIVEN DESIGN (DDD) par Arnaud Lemaire : https://vimeo.com/420563208
- https://particular.net/blog/putting-your-events-on-a-diet
- https://blog.avanscoperta.it/2020/08/04/domain-driven-design-in-2020/
- https://blog.sapiensworks.com/post/2015/11/23/DDD-is-not-programming
- https://tpierrain.blogspot.com/2020/04/et-si-les-adaptateurs-faisaient-eux.html
- [x] https://enterprisecraftsmanship.com/posts/domain-model-purity-completeness/

### Aggregats

- https://github.com/ddd-crew/aggregate-design-canvas

#### FAQ

##### Comment gérer les dépendances entre agrégats ? 

Soient deux agrégats A et B où B possède une référence à A via l'id de ce dernier. Alors les commandes modifiant B peuvent s'assurer de l'existence de A (que A et B appartiennent au même BC ou non). 
Exemple : `ARepository.verifierExistence(commandeModifiantB.IdentifiantDeA)`

### Bounded contexts

- https://medium.com/nick-tune-tech-strategy-blog/bounded-context-canvas-recipe-use-case-swimlanes-11ca647175d3
- https://github.com/ddd-crew/bounded-context-canvas
- The Art of Discovering Bounded Contexts by Nick Tune : https://www.youtube.com/watch?v=ez9GWESKG4I&feature=youtu.be
- https://domaincentric.net/blog/bounded-context-patterns-fan-out-specification-context
- https://blog.onehundredacorns.com/2020/06/17/presentation-du-bounded-context-canvas/


### Context map 

- https://contextmapper.org/docs/context-map-generator/

### Domain events

- https://docs.microsoft.com/fr-fr/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/domain-events-design-implementation
- https://udidahan.com/2008/08/25/domain-events-take-2/
- https://lostechies.com/jimmybogard/2010/04/08/strengthening-your-domain-domain-events/
- https://lostechies.com/jimmybogard/2014/05/13/a-better-domain-events-pattern/
- https://martinfowler.com/articles/201701-event-driven.html
- https://martinfowler.com/eaaDev/EventNarrative.html#HandlingEvents
- https://udidahan.com/2008/08/25/domain-events-take-2/

### Implémentations

- https://github.com/kgrzybek/modular-monolith-with-ddd



## Event Sourcing

- https://www.continuousimprover.com/2020/06/guidelines-event-sourcing.html
- https://www.eventstore.com/blog/the-cost-of-creating-a-stream



## Event Storming

- Glossaire des termes d'eventstorming : https://github.com/ddd-crew/eventstorming-glossary-cheat-sheet
- https://zimarev.com/blog/event-sourcing/myth-busting/2020-07-09-overselling-event-sourcing/
- https://philippe.bourgau.net/how-to-use-event-storming-to-introduce-domain-driven-design/
- https://xebia.com/blog/eventstorming-core-concepts-glossary-and-legend/

### Que faire de la documentation écrite avant l'Event Storming ?

- Prendre connaissance de cette documentation par respect pour ceux qui l'ont écrite
- Elle reste majoritairement un [sunk cost](https://en.wikipedia.org/wiki/Sunk_cost)
- L'artefact nécessaire à la production logicielle est visuelle et évènementielle, pas "documentative"
- La documentation est utile pour rentrer dans les détails, pas pour une vue générale

### Comment découvrir les pivotal events ?

D'après les discussions entre participants quand deux participants sont en désaccords sur le contenu nécessaire au déclenchement d'un évènement.

Quand deux personnes modifient un même évènement.

Quand le pattern Draft/Executable émerge, c'est-à-dire d'un côté un métier dont le cycle de vie concerne un version "brouillon" et de l'autre un métier dont le cycle de vie concerne une version "publiée"

### Quand mettre à jour l'Event Storming

Le stocker pour ne pas frustrer les gens.

Redémarrer from scratch quand on fait une rétrospective du modèle.

En numérique, c'est très difficile de le finir mais facile à mettre à jour.


## Extreme Programming

- Extreme Programming 20 years later by Kent Beck : https://www.youtube.com/watch?v=cGuTmOUdFbo&feature=youtu.be



## Functional programming

- https://fsharpforfunandprofit.com/rop/



## Hexagonal Architecure

- https://netflixtechblog.com/ready-for-changes-with-hexagonal-architecture-b315ec967749
- https://blog.codecentric.de/en/2020/07/hexagon-schmexagon-1/
- https://tpierrain.blogspot.com/2020/03/architecture-hexagonale-ne-vous-perdez.html



## Microservices

- https://medium.com/transferwise-engineering/learnings-from-migrating-legacy-to-microservices-2ef4c0f6a766
- https://microservices.io/patterns/data/saga.html
- https://microservices.io/index.html



## Mob programming

- Woody Zuill "The Power of Mob Programming" (Avanscoperta Meetup) : https://www.youtube.com/watch?v=yu-Gvx__UmE
- https://proagile.se/blog/remote-mob-programming-insights-captured-during-a-webinar-with-woody-zuill
- GOTO 2019 • Mob Programming and the Power of Flow • Woody Zuill : https://www.youtube.com/watch?v=28S4CVkYhWA



## Modélisation

- Visual and Collaborative Modelling - Kenny Baas-Schwegler - DDD Europe 2020 : https://www.youtube.com/watch?v=5RrEzJM5bdw



## Monolithe

- [x] Comment découper un monolithe : https://engineering.gusto.com/chipping-away-at-a-monolith/
- GOTO 2019 • Monolith Decomposition Patterns • Sam Newman : https://www.youtube.com/watch?v=9I9GdSQ1bbM
- https://www.kamilgrzybek.com/design/modular-monolith-integration-styles/



## Refactoring et dette technique

- https://daedtech.com/refactoring-development-technique-not-project/
- https://understandlegacycode.com/blog/start-cleaning-legacy-with-daily-refactoring-hour/
- Llewellyn Falco - From 0% to Cleanly Refactored 100% tested code : https://www.youtube.com/watch?v=wp6oSVDdbXQ
- https://understandlegacycode.com/blog/convince-management-to-address-tech-debt-with-enclosure-diagrams/
- https://medium.com/@smnbss/conways-law-an-architecture-and-organization-journey-7eb974d3773d
- Improving Legacy by Carola Lilienthal : https://www.youtube.com/watch?v=icDjN3yv4C4
- Three Great Opportunities from Legacy Code by J.B. Rainsberger (https://www.youtube.com/watch?v=8e9a_b16e7o
- Refactoring: This class is too large : https://martinfowler.com/articles/class-too-large.html
- punkindev.fr/2020/03/le-refacto-quand-comment-et-pourquoi-en-faire.html
- https://verraes.net/2013/09/extract-till-you-drop/
- https://williamdurand.fr/2013/06/03/object-calisthenics/



## SOLID

- https://shadow-tech.fr/posts/apprenez-enfin-a-coder-proprement-le-principe-de-responsabilite-unique-%28solid-1-5%29
- https://shadow-tech.fr/posts/votre-product-owner-va-vous-adorer-le-principe-d-ouverture-fermeture-%28solid-2-5%29
- https://shadow-tech.fr/posts/arretez-de-faire-du-code-illisible
- https://shadow-tech.fr/posts/le-principe-de-separation-des-interfaces-va-vous-aider-a-mieux-coder-%28solid-4-5%29
- https://shadow-tech.fr/posts/voici-pourquoi-vous-devez-absolument-appliquer-le-principe-d-inversion-de-dependance-%28solid-5-5%29



## Tests 

### Pourquoi écrire des tests automatisés ?

> Permet de prévenir les régressions en cas de modification du code testé

> Permet de documenter la fonctionnalité testée

### Références

- https://mariocervera.com/non-obvious-benefits-automated-testing
- https://codemanship.wordpress.com/2020/09/26/readable-parameterized-tests/
- Rails Conf 2013 The Magic Tricks of Testing by Sandi Metz : https://www.youtube.com/watch?v=URSWYvyc42M
- http://xunitpatterns.com/Principles%20of%20Test%20Automation.html
- Pyramide des tests : https://martinfowler.com/articles/practical-test-pyramid.html
- https://medium.com/wealcomecompany/vous-ne-verrez-plus-les-tests-unitaires-de-la-m%C3%AAme-mani%C3%A8re-7b0f92c460cb
- https://twitter.com/michaelbolton/status/1261019115273232389
- https://blog.antoinechalifour.dev/post/tests-ui-ressemblent-utilisateurs
- https://kentcdodds.com/blog/avoid-nesting-when-youre-testing
- https://blog.thecodewhisperer.com/permalink/integrated-tests-are-a-scam
- https://testingjavascript.com/
- https://tyrrrz.me/blog/unit-testing-is-overrated
- https://outsidein.dev/

### Mocks

- https://github.com/testdouble/contributing-tests/wiki/Don%27t-mock-what-you-don%27t-own
- https://8thlight.com/blog/eric-smith/2011/10/27/thats-not-yours.html
- Les mocks c'est le mal : https://understandlegacycode.com/blog/if-you-mock-are-you-even-testing/
- Peut-être pas tant que ça ? https://blog.thecodewhisperer.com/permalink/you-dont-hate-mocks-you-hate-side-effects
- https://blog.frankdejonge.nl/testing-without-mocking-frameworks/
- https://isaiahperumalla.wordpress.com/2008/05/28/test-driven-design-using-mocks-lessons-learnt-part-2/
- https://martinfowler.com/articles/mocksArentStubs.html

### TDD

- [x] TDD version microtest en graybox : https://www.geepawhill.org/2020/07/24/microtest-tdd-is-gray-box/
- Why Research on Test-Driven Development is Inconclusive? https://arxiv.org/abs/2007.09863
- https://www.stefanhendriks.com/2012/03/31/the-difference-between-tdd-and-test-first-development/
- TDD,  where did it all go wrong : https://www.youtube.com/watch?v=HNjlJpuA5kQ&feature=youtu.be
- https://twitter.com/ygrenzinger/status/1263725481096089600?s=09
- https://www.geepawhill.org/2020/03/11/tdd-on-the-front-end/
- Outside In TDD part I : https://www.youtube.com/watch?v=XHnuMjah6ps
