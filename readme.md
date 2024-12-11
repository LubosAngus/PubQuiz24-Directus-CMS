> [!NOTE]
> I was deciding between [strapi](https://strapi.io/) and [directus](https://directus.io/) for this CMS.\
> I went with directus, because I wanted to try it out. Turns out, it wasn't such a good choice.\
> Building up database from schema is pain in the ass. Not everything is exported to schema.\
> So in the next update I'm going to rewrite this to strapi.

# PubQuiz24 Directus CMS

To learn more about Directus [follow this link](https://docs.directus.io/self-hosted/cli.html).

## Bootstrap this CMS

For some reason, directus needs node.js in version 18

```sh
nvm use 18
```

Clone your `.env` file from `.env.example`. You don't event need to edit anything.

After the file is created, we can initialize directus CMS.

```sh
npm run initialize
```

## Run admin

```sh
npm run start
```

Go to [localhost:8055/admin/login](http://localhost:8055/admin/login), login with credentials in .env _(only creating user when initializing)_.\
Default are:

```
admin@quiz.app
1234567890
```

## Create data

After all this is done, you need one final step and to create quiz, topics and questions.

Quizes are intended to have 2 topics in one round on frontend, so keep that in mind.
