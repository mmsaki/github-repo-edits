# github-cleanup

1. Setup environment

   ```sh
   uv venv --python 3.12
   ```

1. Install packages

   ```sh
   uv pip install ipython ipykernel pytz
   ```

## Get repo

Save repos to `repos.json`

```
gh repo list --limit 200 --json "name,openGraphImageUrl,owner,pushedAt,createdAt,url,visibility,isPrivate,isFork,watchers,stargazerCount,isEmpty,forkCount" > repos.json
```

## Edit repo

Making repos private

```
gh repo edit mmsaki/reponame --visibility private
```

## Programmable Edits

Make other edits in bulks inside [`repos.ipynb`](./repos.ipynb)

Thanks!
