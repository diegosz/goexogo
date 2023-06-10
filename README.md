# goexogo

<p align="center">
<img src="assets/images/_4d9e52eb-551a-44c4-8f05-532d73cedb10.jpg" alt=“goexogo” title="goexogo" width="60%" height="60%">
</p>

## Add New Repo

1. Pull branches:

   ```sh
   sh pullall.sh
   ```

2. In `main` branch, add new repo to `vangen.json`:

3. Commit and push:

   ```sh
   git add .
   git commit -m "Add new repo"
   git push -u origin main
   ```

4. In Github, the `generate.yml` action, should run generating the files and pushing them to `publish` branch.

   > Only generates on changes of `vangen.json` file.

5. Github Pages should be updated: [goexogo](https://go.goexogo.com/)

> Remember to set `go.goexogo.com` in **Custom Domain** in [pages settings](https://github.com/diegosz/goexogo/settings/pages).

## Generate Manually

```sh
vangen -out docs
```
