# myVideoPlayer

![](https://github.com/froldev/symfony-myvideoplayer/blob/master/myvideoplayer.png)

## Getting Started for Projects

### Requirements

- Php ^7.2
- Symfony 5.2
- Composer

### Installation

1. Clone the current repository.

```bash
$ git clone https://github.com/froldev/symfony-myVideoPlayer.git
```

2. Move into the directory and create an `.env.local` file.
   **This one is not committed to the shared repository.**
   Modify `db_name` by the name you want.

3. Execute the following commands in your working folder to install the project:

```bash
$ composer install
$ bin/console doctrine:database:create
$ bin/console doctrine:migrations:migrate
$ bin/console doctrine:fixtures:load
```

> Reminder: Don't use composer update to avoid problem

> Assets are directly into _public/_ directory

### Working

Launch the server with the command below;

```bash
$ symfony server:start
```

### Built With

- [Symfony](https://github.com/symfony/symfony)
- [Twig](https://twig.symfony.com)
- [Axios](https://github.com/axios/axios)
- [Bootstrap](https://getbootstrap.com)
- [Copadia - Php Video Url Parser](https://github.com/Copadia-team/php-video-url-parser)
- [FOS CKEditor Bundle](https://symfony.com/doc/current/bundles/FOSCKEditorBundle/index.html)
- [StofDoctrine Extension Bundle](https://symfony.com/doc/current/bundles/StofDoctrineExtensionsBundle/index.html)
- [Vich Uploader](https://symfony.com/doc/2.x/bundles/EasyAdminBundle/integration/vichuploaderbundle.html)
- [Knp Paginator Bundle](https://github.com/KnpLabs/KnpPaginatorBundle)
- [Font Awesome](https://fontawesome.com/)

## User interface

---

    * homepage with banner, search and best videos
    * pages by category with videos

## Admin interface (**with connexion**)

---

    * page connexion
    * homepage with several elements (number of categories, number of videos and number of users)
    * page category with list, create, update, delete and search a category
    * page video with list, create, update, delete and search a video
    * page user with list create, update, delete and search a user

## Connexion to Admin Interface

---

```bash
login : admin@admin.fr
password : password
```

## **Remember to change the password to secure access to the adminsitrator area**

### Constant location in this project

#### Controller/HomeController.php

In order to change the number of categories in the navbar
The others will be in a drop-down list

```
    const MAX_LINKS_NAV = 6;
```

### Technology framework and library used in this project

`PHP 7.2`, `Symfony 5.2`, `JavaScript`, `Axios`, `Html5`, `Twig`, `Bootstrap`, `fortawesome/fontawesome`, `Copadia - Php Video Url Parser`, `FOS CKEditor Bundle`, `StofDoctrine Extension Bundle`, `Vich Uploader`, `Knp Paginator Bundle`

### About database `MySQL`

List of tables :

- category
- video
- user

##### projet réalisé février 2021 - mars 2021.
