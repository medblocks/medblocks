# Medblocks
Your stack for building modern healthcare applications

[Documentation](https://docs.medblocks.org/medblocks/quick-start)

## Usage:

### Local Development
```sh
docker-compose up
```

### Deployment
- Set `DOMAIN_NAME` environment variable to your full URL: `https://domain.example.com`
- Also set `HTTPS` to `true`
- Change the `serve.tls.allow_termination_from` in the `hydra/hydra.yml` file to the IP address range of the reverse proxy/load balancer according to [CIDR Notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)
- Change the insecure example value to secure randomly generated values in all configuration files - including passwords in `init.sql`.