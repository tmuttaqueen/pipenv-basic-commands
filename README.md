# pipenv-basic-commands
Basic commands when creating python environment using pipenv

Pipenv is best for managing dependencies. It has a Pipfile which spcifies the version user gave when install a package. It has Pipfile.lock file which specifies the exact version of that package installed after resolving dependencies. So to create an exact environment in development and production environment we can use the Pipfile.lock file which is very handy.

#### Installing pipenv ubuntu
```
pip3 install pipenv
```

#### Installing pipenv windows
```
pip install pipenv
```

#### Creating an environment and installing packages when Pipfile already exists ( pwd is the project folder )
```
pipenv install
```

#### Creating an environment for a project with python version specified ( pwd is the project folder )
```
pipenv --python 3.6
```

#### Activate an environment ( pwd is the project folder )
```
pipenv shell
```

#### Removing an existing environment in a project folder ( pwd is the project folder )
```
pipenv --rm
```

### After activating a environment

#### Installing/Uninstalling a package
```
pipenv install numpy
pipenv install numpy==1.19.5
pipenv install numpy~=1.19    // pipenv will install the latest version of 1.*
pipenv install --dev numpy    // only install in development
pipenv uninstall numpy        // uninstall any version of numpy 
pipenv uninstall --dev numpy  // uninstall from development 
pipenv uninstall --all        // uninstall all packages
pipenv uninstall --all-dev    // uninstall all package from development
```

#### Installing package from requirements.txt file
```
pipenv install -r requirements.txt
```

#### See the dependency graph of each package
```
pipenv graph
```

