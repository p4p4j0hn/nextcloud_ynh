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
