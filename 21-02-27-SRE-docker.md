# SRE Live! Docker n stuff

1) Install docker on debian stable
  1.1) https://docs.docker.com/engine/install/debian/
  1.2) https://docs.docker.com/engine/install/linux-postinstall/
    1.2.1) Add docker group, add user to docker group
  1.3) How docker works? https://docs.docker.com/engine/images/architecture.svg
  1.3.1) Use stuff like cgroups, namespaces, overlayfs, CoW

2) Dockerize elixir!
  2.1) default image: https://hub.docker.com/_/elixir
  2.2) Install phoenix: https://hexdocs.pm/phoenix/installation.html#phoenix
  2.3) Install node: https://github.com/nodesource/distributions#deb

