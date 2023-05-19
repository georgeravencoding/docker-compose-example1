
# docker-compose Traefik & Ghost

> Just a simple docker-compose with [Traefik](https://traefik.io/), [Ghost](https://ghost.org/) (CMS) and MariaDB for SQL server.

A fast and prod oriented stack to have your own and easy hackable CMS with Ghost. Was used before on [my personnal website](https://j.hommet.net).

## :factory: Requirements

* linux host (tested successfully on Ubuntu 20.04, Debian 10 & 11)
* docker >= 18.x
* docker-compose >= 1.26

## :rocket: How to use

Clone this repo where you want with this line :

```bash
git clone https://github.com/Mettmett/docker-compose.git:traefik-ghost-sql/
```

You need to edit the file `.env` at the source folder to modify the values of some vars.

**Important !!** You have to "`sudo chmod 600`" the file "acme.json", otherwise you won't be able to pull Let's Encrypt certificates.

After that when you're all set, press the red button to initiate :fire: !

```bash
docker-compose pull; docker-compose up -d; docker-compose logs -f
```

## :star: Author

Made by Julien HOMMET :fr: for [my personnal website](https://j.hommet.net)

* Twitter: [@_ComputerZ](https://twitter.com/_ComputerZ)
* GitHub: [Mettmett](https://github.com/Mettmett)

## :wrench: Support & Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## :moneybag: Licence

[CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0)

## :anchor: Misc

More infos at [https://computerz.solutions/docker-ghost-traefik-tls/](https://computerz.solutions/docker-ghost-traefik-tls/)
