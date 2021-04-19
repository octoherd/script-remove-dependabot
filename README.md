# remove dependabot

> An [octoherd](https://github.com/octoherd) script to delete the `.github/dependabot.yml` file

## Usage

```
$ npx @octoherd/script-remove-dependabot
```

Pass all options as CLI flags to avoid user prompts

```
$ npx @octoherd/script-remove-dependabot \
  -T ghp_0123456789abcdefghjklmnopqrstuvwxyzA \
  -R "octoherd/repository-with-script-folders"
```

## Options

| option                       | type             | description                                                                                                                                                                                                                                 |
| ---------------------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `--octoherd-token`, `-T`     | string           | A personal access token ([create](https://github.com/settings/tokens/new?scopes=repo)). Script will create one if option is not set                                                                                                         |
| `--octoherd-repos`, `-R`     | array of strings | One or multiple space-separated repositories in the form of `repo-owner/repo-name`. `repo-owner/*` will find all repositories for one owner. `*` will find all repositories the user has access to. Will prompt for repositories if not set |
| `--octoherd-bypass-confirms` | boolean          | Bypass prompts to confirm mutating requests                                                                                                                                                                                                 |

## Licenses

[ISC](LICENSE.md)
