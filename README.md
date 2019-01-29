# pipenv

https://realpython.com/pipenv-guide/

`Pipfile` intends to replace `requirements.txt`.

It’s worth noting again that you should never change `Pifile.lock` by hand. It is meant to be generated with `pipenv lock`.

## Installation
pip install pipenv

## Usage

`pipenv shell`
`pipenv install flask==0.12.1`
`pipenv install numpy`
`pipenv install -e git+https://github.com/requests/requests.git#egg=requests`

**install as DEV package**
`pipenv install pytest --dev`

** show a dependency graph**
`pipenv graph`


**happy with your setting??? LOCK your environment**
** which creates/updates your Pipfile.lock**
`pipenv lock`

**You can install more things afterward**
**but to go back to your CLEAN last-locked environment...**
`pipenv install --ignore-pipfile`
**this gnores Pipfile and use pipfile.lock instead**


