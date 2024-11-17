# PubQuiz24 Directus CMS

To learn more about Directus [follow this link](https://docs.directus.io/self-hosted/cli.html) to learn more.

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

## Create data

After all this is done, you need one final step and to create quiz, topics and questions.

Quizes are intended to have 2 topics in one round on frontend, so keep that in mind.