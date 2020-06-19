# easypkg-repo
The main repository for EasyPack packages
## Adding your package
To add your package to the repo, add a line to `repo.epdata` with this format:
```
package <package name, no spaces> version <version, no spaces> url <url, no spaces>
```
The source code for this language is [here](https://github.com/munchkinhalfling/easypack-dsl).<br/>
Then, give GitHub Pages a moment to deploy, and run:
```bash
$ easypack install your-package-name
```
### Creating your own repo
Create a repo.epdata file with the following content: ("..." is a list of packages in the format described above)
```sdl
repo <your-repo-name>
...
```
Then, put it on the Internet and run `easypack addrepo <url of repo.epdata>`.
