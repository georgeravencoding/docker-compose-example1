# docker-compose Traefik & multiple Wordpress

> Docker stack to have some WordPress sites behind a Traefik reverse-proxy with Nginx, a SQL database and Redis objects cache.

This is a prod ready stack, but it needs some customization to be powerful. There is no usage of WordPress multisite, this is just a proof of concept to host multiple WordPress behind one traefik.

Only one redis server is used, it's not a good idea to have one redis server for each WordPress site.

## :factory: Requirements

* linux host (tested successfully on Ubuntu 20.04 && 22.04, Debian 10 & 11)
* docker >= 23.x
* docker compose (plugin) >= 2.17.x

## :rocket: How to use

Clone this repo where you want with this line :

```bash
git clone https://github.com/Mettmett/docker-compose.git:traefik-multiple-wordpress
```

You need to edit the file `.env` at the source folder to modify the values of some vars.

**Important !!** You have to "sudo chmod 600" the file "acme.json", otherwise you won't be able to pull Let's Encrypt certificates.

After that when you're all set, press the red button to initiate :fire: !

```bash
docker compose pull && docker compose up -d && docker compose logs -f
```

## :star: Author

Made by Julien HOMMET :fr: for [my personnal website](https://j.hommet.net)

* Twitter: [@mettmettz](https://twitter.com/mettmettz)
* GitHub: [Mettmett](https://github.com/Mettmett)

## :wrench: Support & Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## :moneybag: Licence

[CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0)

## :anchor: Misc
