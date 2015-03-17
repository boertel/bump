Bump version number for `bower.json` and `package.json` according to [semver](http://semver.org/).

## Installation

copy `bump` file in one of the `$PATH` folder, example:

```
git clone git@github.com:boertel/bump.git
cp ./bump/bump /usr/local/bin/
chmod +x /usr/local/bin/bump
```

## Usage

Show all the version for each file:
```
bump
```


According to [semver](http://semver.org/) which defines version number as follow: MAJOR.MINOR.PATCH:

increment *patch*:
```
bump patch [message]
```

increment *minor*:
```
bump minor [message]
```

increment *major*:
```
bump major [message]
```

set a defined version number:
```
bump 0.0.0 [message]
```


If ```message``` is defined, it will ```git commit``` the updated files and create the tag corresponding to the new version.

If your version is a single commit, you can do the following:
```
git add my-broken-file
git commit "fix my-broken-file"
bump patch !$
```
(`!$` = last argument of the last command, in our case: "fix my-broken-file")
