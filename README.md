# npm-package

See discussion on [how to install an npm package from GitHub directly](https://stackoverflow.com/a/21918559/639133): *""possible since version 1.1.65 and works for github.com only""*

Install this package directly from github
```bash
git clone https://github.com/mozey/npm-package.git
cd npm-package
mkdir -p _excluded/test && cd _excluded/test
npm install mozey/npm-package
```

With an empty repo `npm install` will fail with
```
no such file or directory, open '...package.json'
```

Follow the instructions to [create a package](https://docs.npmjs.com/creating-a-package-json-file)
```bash
npm init
```

Selected all defaults, except for *"description"*. It added a bunch of field, according to [creating a package.json file](https://docs.npmjs.com/creating-a-package-json-file), only the *"name"* and *"version"* fields are required. Adding *"author"* also seems appropriate, the other fields are not necessary
