# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
```

For direnv (which I highly recommend as a general tool), you can setup it up using the following:

- Install direnv (e.g. `brew install direnv` on mac)
- Hook into your shell (e.g. add `eval "$(direnv hook zsh)"` to your `.zshrc` file)
- Reload your shell
- Create an .envrc file in the root of your backstage app with something like:

```
# .envrc
dotenv # this will load an `.env` file
```

- Create a standard `.env `file or use an existing one
- Run `direnv allow` to tell direnv to accept the .envrc file. Required anytime the file changes. This will also reload your shell with the .env variables in your shell
- Run `yarn dev` and with the environment variables ready.

NOTE: direnv is a directory switcher, so anytime you cd into a directory with a .envrc file in the directory structure it will find it and execute the commands automatically. It also has many other useful features beyond this which you can explore and use for other purposes.

### For develop

#### Create GithubApp

[Docs](https://backstage.io/docs/integrations/github/github-apps)

run this command and change permissions

```
yarn backstage-cli create-github-app <github org>
```
