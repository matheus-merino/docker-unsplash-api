# Docker Project

This project is part of Bogdan Stashchuk's O'reilly Docker course (learn more at https://learning.oreilly.com). The objective of the course project is to dockerize a full-stack application that allows users to search for Unsplash photos and save them to a personal gallery. For that, we are using both **Dockerfiles** and **Docker Compose**.

To see the original instructors' repository (including the feature for storing photos in MongoDB), follow this [link](https://github.com/bstashchuk/images-gallery).

## Initial configuration

- Create account at the https://unsplash.com
- At the https://unsplash.com/oauth/applications create new **demo** application with title **"Images Gallery"**.
  Demo applications are limited to 50 requests per hour
- In the newly created application find section **"Keys"** and copy **Access Key**
- In the **api** folder create file **.env.local** and add there following line:

```
UNSPLASH_KEY=<Paste copied Access Key here>
```

**EXAMPLE** with fake code(don't try to use it in your app):

```
UNSPLASH_KEY=2MJvApIkV13hfg2LmQlneILfHoJ2ttlzSdPKefGOyKM
```

- Save modified **.env.local** file
