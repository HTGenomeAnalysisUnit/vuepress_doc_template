# vuepress_doc_template

## Configuration

This template assumes the default folder setup

```bash
├─ docs
│  ├─ .vuepress
│  │  └─ config.js
│  └─ README.md
├─ .gitignore
└─ package.json
```

Then you need to create a personal access token and store it in the repository encrypted secret named ACCESS_TOKEN.

Finally, configure the base value in `docs/.vuepress/config.js` and the TARGET_REPO value in the workflow .yml file to match your repository. 

## Automatic deploy

The GitHub action configured in `.github/workflows` will automatically build and deploy the documentation to github pages.

## Deploy from local folder

```bash
#requires npm/pnpm
#install locally in folder
pnpm i vuepress-theme-vt vuepress -D
#then deploy
./deploy.sh
```

