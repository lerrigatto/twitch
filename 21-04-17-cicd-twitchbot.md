# SRE Live! CI/CD for python twitchbot

## Today's plan
* What is a twitch chat bot
* How does it works
* How do we build and package python
* Create a docker container
* Publish the container somewhere

## Missing...
* Create a fluxcd deploy
* Build container in CI

## Recap
We checked the code of [lerrigattobot](https://github.com/lerrigatto/lerrigattobot) and the [twitchio](https://github.com/TwitchIO/TwitchIO) library.
The bot, right now, is fairly dumb, but enough to test the build and deployment.

We talked about [python-poetry](https://python-poetry.org/) and [pyproject.toml - PEP621](https://www.python.org/dev/peps/pep-0621/). The bot project is also using a bunch of other nice stuff like black, pre-commit, isort and sphinx, but we didn't really talk about them.

We created a docker multistage build and published the container to [dockerhub](https://hub.docker.com/r/lerrigatto/lerrigattobot).

We talked a lot about how cool docker multistage is.

## Links
* https://github.com/lerrigatto/lerrigattobot
* https://github.com/TwitchIO/TwitchIO
* https://www.docker.com/blog/containerized-python-development-part-1/
* https://docs.docker.com/develop/develop-images/multistage-build/
