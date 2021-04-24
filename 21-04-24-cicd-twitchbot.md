# SRE Live! CI/CD for python twitchbot (pt2)

## Today's plan
* Create a fluxcd deploy
* Build container in CI

## Recap
Check [last week streaming](21-04-17-cicd-twitchbot.md) to get where we are starting from.
We create a `kustomizer` deployment folder in the lerrigattobot repo.
We deployed that folder and the container published on dockerhub on the k3s cluster using fluxcd.

The fluxcd deployment was fine but we need to find a better way.

## Links
* https://github.com/lerrigatto/lerrigattobot
* https://github.com/fluxcd/flux2-kustomize-helm-example
