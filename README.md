# Model Picker

Quel modèle Claude pour ce prompt, et avec quel effort ?

**L'outil en ligne : [lilian-barty.fr/outils/model-picker](https://www.lilian-barty.fr/outils/model-picker/)**, gratuit, sans compte.

Vous décrivez votre tâche comme vous la diriez à l'IA. L'outil recommande le modèle (Haiku, Sonnet, Opus), le niveau d'effort, et estime le coût. Il accepte aussi une liste de tâches, une par ligne, pour comparer d'un coup.

## Comment il décide

Pas en comptant des mots-clés. Il repère les négations (« sans audit » ne compte pas comme un audit), classe la tâche par famille (mécanique, rédaction, analyse, conception), puis module selon la criticité, le volume et la longueur.

Surtout, il place la tâche sur un axe : exécution cadrée ou jugement. Le cadré (règles explicites, résultat vérifiable) se délègue à un modèle léger. Le jugement (stratégie, prix, angle éditorial, décision à conséquences) se garde sur le plus capable, parce que c'est là qu'un modèle trop léger rend un travail médiocre sans prévenir. C'est la règle que j'applique à mon propre assistant.

Fable 5.1 n'arrive jamais en tête : Anthropic conseille de commencer par Opus 5.5 et de ne passer à Fable qu'en recours.

## Ce qu'il ne fait pas

Il n'envoie rien. Toute l'analyse tourne dans votre navigateur, votre prompt ne part nulle part, et il n'appelle aucune IA : ce sont des règles écrites à la main, pas un modèle qui en juge un autre.

C'est donc une estimation, pas un verdict. Sur une tâche ambiguë, il peut se tromper d'un cran ; le texte de justification vous dit pourquoi il a choisi, pour que vous puissiez le contredire.

Les prix et la gamme suivent la documentation d'Anthropic de septembre 2026. Quand un modèle sort, l'outil en ligne est mis à jour d'abord, ce dépôt ensuite.

## Ce dépôt

Le code est ici pour être lu : `index.html` contient tout l'outil, règles de décision comprises. La version en ligne est la référence.

Une recommandation qui vous paraît fausse ? Ouvrez une issue avec le prompt testé, ou écrivez à lilianchristophe.pro@gmail.com.

## Qui l'a fait

Lilian Barty-Christophe, consultant freelance en IA à Paris ([lilian-barty.fr](https://www.lilian-barty.fr/)). J'installe chez des indépendants et des équipes des systèmes IA qui font ce genre d'arbitrage tout seuls.

## Licence

Code visible, tous droits réservés. Vous pouvez le lire et vous en inspirer, pas le republier tel quel. Pour un autre usage, écrivez-moi.

## In English

Describe a task, and Model Picker recommends which Claude model to use, at which effort level, with a cost estimate. It runs entirely in your browser with hand-written rules: no prompt is sent anywhere. French interface. Try it at [lilian-barty.fr/outils/model-picker](https://www.lilian-barty.fr/outils/model-picker/). Source visible, all rights reserved.
