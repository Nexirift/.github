<p align="center">
<img src="https://raw.githubusercontent.com/Nexirift/.github/main/banner.svg" width="400" />
</p>

# Nexirift Open Source

Welcome to the Nexirift organization on GitHub!

We are an upcoming social networking platform, dedicated to connecting people and fostering meaningful interactions. Our open-source projects are designed to empower developers like you to contribute and shape the future of our platform.

Whether you're a seasoned developer or just starting out, we invite you to explore our repositories, join our community, and make a positive impact on the Nexirift platform.

Happy coding!

## Repositories

As part of our dedication to transparency, most of our repositories are open source. Feel free to browse through the code, contribute, and help us improve!

### API Servers

The reason why the API servers are split is for reliability. If needed, we can move an API server off to a different provider without affecting the other ones. In addition, if a problem occurs in one API server, it shouldn't affect the others due to the servers being split across different containers.

#### User

Our user API server is called [Spark](https://github.com/Nexirift/spark)! Currently, we do not have the repository public as we are still developing it.

#### Admin

Our admin panel uses an extra API server called [Galaxy](https://github.com/Nexirift/galaxy). Similar to the Spark server, this is not public yet.

#### Developer

The developer management panel uses an API server called [Singularity](https://github.com/Nexirift/singularity). Similar to the Spark server, this is not public yet.

### Relays

We plan to have relays that connect to the Activitypub protocol (Mastodon, Pleroma, etc) and Atproto (Bluesky) instances. This has not been started yet.

### Authentication

We have made a GraphQL Yoga connector to authenticate users using the open source Keycloak authentication solution.

Visit the repository here: [plugin-keycloak](https://github.com/Nexirift/plugin-keycloak).

### Policies

We are still working on making internal policies public (such as the data breach policy), please check back later.

## Documentation

We are working on providing documentation for all of our open source repositories.

## Reporting a Security Vulnerability

To report a security vulnerability related to a specific repository, please create a new security advisory in the repository, do NOT use the issue tracker. You can find a list of our repositories [here](https://github.com/orgs/Nexirift/repositories).

If the vulnerability is not related to a specific repository or you cannot access the repository, please email us at [security@nexirift.com](security@nexirift.com). Please include detailed information about the vulnerability and any steps to reproduce it.

Please do NOT disclose the vulnerability to anyone else, as it could heavily impact our users. We appreciate your responsible disclosure and commitment to the security of our platform.

For example, to report a vulnerability in the GraphQL Yoga Keycloak plugin repository, you can visit [this link](https://github.com/Nexirift/plugin-keycloak/security/advisories/new).
