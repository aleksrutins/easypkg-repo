# easypkg-repo
The main repository for EasyPack packages
## Adding your package
To add your package to the repo, add a JSON object to the `packages` array in repo.json with the following schema:
```json
{
  "name": "your-package-name",
  "version": "your-package-version",
  "url": "https://host.com/your/package.easypack.tar.gz"
}
```
Then, give GitHub Pages a moment to deploy, and run:
```bash
$ easypack install your-package-name
```
### Creating your own repo
Create a repo.json file with the following content: ("..." is a list of packages in the format described above)
```json
{
  "packages": [
    ...
  ]
}
```
Then, put it on the Internet and run `easypack addrepo <url of repo.json>`.
