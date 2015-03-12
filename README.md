## Installation

copy `bump` file in one of the $PATH folder:

```
cp bump /usr/local/bin/
chmod +x /usr/local/bin/bump
```

## Usage

Show all the version for each file:
```bump```


According to [semver](http://semver.org/):

increment *patch* part of the version number:
```
bump patch [message]
```

increment *minor* part of the version number:
```
bump minor [message]
```

increment *major* part of the version number:
```
bump major [message]
```

set a defined version number:
```
bump 0.0.0 [message]
```


For each of these options, you can define a ```message```, in this case, it would ```git commit``` the updated files and create the tag corresponding to this new version
