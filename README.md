# Personal-Cloud

> [!IMPORTANT]
> In the latest versions of `docker compose`, I have noticed that every single docker compose creates it's own docker network which I find to be a waste of resources so I created a docker network and then added that network to all the services in my homelab.
> Here is the command:
> ```bash
> docker network create \
> --attachable \
> --driver=bridge \
> --ipv4 \
> --ipv6 \
> docker-vnet
> ```

## Services

- [Arcane](./arcane/README.md)
