# SRE Live! CI/CD with FluxCD

## Recap
After a lot of trial and error, we find a way to deploy the [lerrigattobot](https://github.com/lerrigatto/lerrigattobot) twitch chatbot using FluxCD. We are fetching the default kustomize from the public repo and patching the configs in the fluxCD repo.

It took a long time to find a way to patch the configmap because I was using the configmap-generator from kustomize and that was adding a random hash, making the patch not matching with any existing resource.
The fix I applied was to remove the random hashing.

Then we had troubles locating the patch files because fluxcd was looking for it in the upstream lerrigattobot repo. We fix that using an inline patch.

Next time we will have to fix the secrets, that should work more or less in the same way, so _there will be no issues ™_.

## Links
https://github.com/fluxcd/flux2-kustomize-helm-example
