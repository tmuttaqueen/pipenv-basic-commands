# pipenv-basic-commands
Basic commands when creating python environment using pipenv

Pipenv is best for managing dependencies. It has a Pipfile which spcifies the version user gave when install a package. It has Pipfile.lock file which specifies the exact version of that package installed after resolving dependencies. So to create an exact environment in development and production environment we can use the Pipfile.lock file which is very handy.

#### Installing pipenv ubuntu
```
pip3 install pipenv
```

#### Installing pipenv windows
```
pip3 install pipenv
```

#### Creating an environment inside a project folder with python version specified
```
pipenv --python 3.6
```

#### Removing an existing environment in a project folder ( pwd is the project folder )
```
pipenv --rm
```

#### Installing a package
```
pipenv install numpy
pipenv install numpy==1.19.5
```

#### Installing package from requirements.txt file
```
pipenv install -r requirements.txt
```

#### See the dependency graph of each package
```
pipenv graph
```

