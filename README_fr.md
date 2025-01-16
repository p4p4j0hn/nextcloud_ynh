<!--
Nota bene : ce README est automatiquement généré par <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
Il NE doit PAS être modifié à la main.
-->

# Nextcloud pour YunoHost

[![Niveau d’intégration](https://apps.yunohost.org/badge/integration/nextcloud)](https://ci-apps.yunohost.org/ci/apps/nextcloud/)
![Statut du fonctionnement](https://apps.yunohost.org/badge/state/nextcloud)
![Statut de maintenance](https://apps.yunohost.org/badge/maintained/nextcloud)

[![Installer Nextcloud avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=nextcloud)

_[Lire le README dans d'autres langues.](./ALL_README.md)_

> _Ce package vous permet d’installer Nextcloud rapidement et simplement sur un serveur YunoHost._  
> _Si vous n’avez pas YunoHost, consultez [ce guide](https://yunohost.org/install) pour savoir comment l’installer et en profiter._

## Vue d’ensemble

Nextcloud permet de rendre accessible et de synchroniser ses données, fichiers, contacts, agendas entre différents appareils (ordinateurs ou mobiles), ou de les partager avec d'autres personnes (avec ou sans comptes), et propose également des fonctionnalités avancées de communication et de travail collaboratif. Nextcloud dispose de son propre mécanisme d'applications (voir aussi [le store d'apps de Nextcloud](https://apps.nextcloud.com/)) pour disposer des fonctionnalités spécifiques.

Dans le cadre de YunoHost, Nextcloud s'intègre avec le SSO/portail utilisateur (les comptes YunoHost sont automatiquements connectés à Nextcloud).

L'adresse `/.well-known` sera automatiquement configuré pour la synchronisation CalDAV et CardDAV si aucun autre service tel que Baïkal ne l'utilise déjà.

- Intégration avec les utilisateurs YunoHost et le SSO - exemple, le bouton de déconnexion
- Permet à un utilisateur d'être l'administrateur (choisi à l'installation)
- Permet de multiples instances de cette application
- Accès optionnel au répertoire home depuis les fichiers Nextcloud (à activer à l'installation, le partage étant activé par défaut)
- Utilise l'adresse `/.well-known` pour la synchronisation CalDAV et CardDAV du domaine si aucun autre service ne l'utilise déjà - par exemple, Baïkal
-

## Branche olstable

Cette branche suit une ancienne version stable, car souvent les premières versions de nextcloud ne sont pas totalement stables.

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/nextcloud_ynh/tree/testing).

Pour essayer la branche oldstable, procédez comme suit.

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/nextcloud_ynh/tree/oldstable --debug
ou
sudo yunohost app upgrade nextcloud -u https://github.com/YunoHost-Apps/nextcloud_ynh/tree/oldstable --debug
```

**Version incluse :** 29.0.10~ynh1

**Démo :** <https://demo.nextcloud.com/>

## Captures d’écran

![Capture d’écran de Nextcloud](./doc/screenshots/screenshot.png)

## Documentations et ressources

- Site officiel de l’app : <https://nextcloud.com>
- Documentation officielle utilisateur : <https://docs.nextcloud.com/server/latest/user_manual/en/>
- Documentation officielle de l’admin : <https://docs.nextcloud.com/server/stable/admin_manual/>
- Dépôt de code officiel de l’app : <https://github.com/nextcloud/server>
- YunoHost Store : <https://apps.yunohost.org/app/nextcloud>
- Signaler un bug : <https://github.com/YunoHost-Apps/nextcloud_ynh/issues>

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche `testing`](https://github.com/YunoHost-Apps/nextcloud_ynh/tree/testing).

Pour essayer la branche `testing`, procédez comme suit :

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/nextcloud_ynh/tree/testing --debug
ou
sudo yunohost app upgrade nextcloud -u https://github.com/YunoHost-Apps/nextcloud_ynh/tree/testing --debug
```

**Plus d’infos sur le packaging d’applications :** <https://yunohost.org/packaging_apps>
