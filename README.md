# neovia/.github

Fichiers par défaut de l'organisation.

- `pull_request_template.md` — modèle de PR par défaut pour tout dépôt sans
  template propre (structure GIT-009 + attestation IA GIT-021, charte IA
  Annexe B.5). Source de vérité :
  [neovia-quality/ci](https://github.com/neovia/neovia-quality/tree/main/ci)
  (dépôt privé) — modifier là-bas, recopier ici.

## Ce dépôt doit rester public

GitHub n'utilise les fichiers par défaut d'une organisation que si le dépôt
`.github` est **public** ([doc](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)).
Ils s'appliquent ensuite à tous les dépôts de l'org, quelle que soit leur
visibilité. Le passer en privé désactiverait donc le template de PR par défaut
(et l'attestation IA qui va avec) sur tout le parc, silencieusement, sans
erreur ni avertissement. La visibilité `internal`, qui serait l'entre-deux,
n'est pas disponible sur le plan Team.

Conséquence : **rien de sensible ici**. Pas de workflow CI, pas d'URL ou d'IP
d'infrastructure interne, pas de nom de secret, pas de référence à un outil
non public. Les workflows d'organisation n'ont de toute façon pas leur place
dans ce dépôt : un workflow placé ici ne s'exécute que sur les PR de ce dépôt,
il ne se propage pas aux autres (seul un *reusable workflow* appelé
explicitement, ou un *required workflow* de ruleset, se partage).
