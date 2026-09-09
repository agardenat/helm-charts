# helm-charts

Les charts Helm de [kdt](https://github.com/agardenat/kdt) et de
[kdt-identity](https://github.com/agardenat/kdt-identity), servis par GitHub Pages.

```sh
helm repo add kdt https://agardenat.github.io/helm-charts
helm repo update
helm search repo kdt
```

| Chart | Application | Source |
| --- | --- | --- |
| `kdt/kdt-web` | Interface web de kdt | https://github.com/agardenat/kdt |
| `kdt/kdt-identity` | Utilisateurs et groupes locaux pour Kubernetes | https://github.com/agardenat/kdt-identity |

Le contenu de ce dépôt est produit par la CI des deux projets : chaque tag `v*` y dépose l'archive
du chart et reconstruit `index.yaml`. Rien ne s'y édite à la main.

Les pré-versions y figurent aussi. `helm install` ne les retient pas de lui-même : il faut `--devel`
ou un `--version 2.0.0-rc.1` explicite pour en installer une.
