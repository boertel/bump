Increment the version according to [semver](http://semver.org/).

## Installation

copy `bump` file in one of the `$PATH` folder, example:

```
git clone git@github.com:boertel/bump.git
cp ./bump/bump /usr/local/bin/
chmod +x /usr/local/bin/bump
```

## Usage
```
bump [patch|minor|major] x.x.x
```
where ```x.x.x``` is your version you want to increment.

## Examples
```
> bump patch 0.0.2
0.0.3
```

```
> bump minor 0.0.3
0.1.0
```
Note: it resets the *patch* value

```
> bump major 0.0.5
1.0.0
```

You can check out [git-release](boertel/git-extended/blob/master/git-release) git-release to compute next version of your git project according to your releases/tags.
