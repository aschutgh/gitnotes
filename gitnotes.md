% Git aantekeningen
% Arthur Schut
% 2018-08-27

# Some git resources
- https://maryrosecook.com/blog/post/git-from-the-inside-out
- https://jwiegley.github.io/git-from-the-bottom-up/
- https://git-scm.com/book/en/v2

# Git global config
Instellingen voor alle repositories op je systeem.

~~~~ {#bash1 .bash .numberLines}
git config --global user.name "voornaam achternaam"
git config --global user.email naam@domeinnaam.nl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Initializing a repository in an existing directory

~~~~ {#bash2 .bash .numberLines}
git init
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Adding untracked files
~~~~ {#bash3 .bash .numberLines}
git add filename
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Adding multiple untracked files
~~~~ {#bash4 .bash .numberLines}
git add .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Committing files
~~~~ {#bash5 .bash .numberLines}
git commit -m "beschrijving van je wijzigingen"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Make and checkout new branch
~~~~ {#bash6 .bash .numberLines}
git checkout -b nameofnewbranch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Checkout master branch
~~~~ {#bash7 .bash .numberLines}
git checkout master
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Merge somebranch into master branch
Branch master moet hiervoor wel je huidige branch zijn.

~~~~ {#bash8 .bash .numberLines}
git merge somebranch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Connect to github
## Connect local repository to github repository
Maak op github een nieuwe repository. Idealiter met dezelfde naam als je lokale
repository. Kopieer de github link van je repository. Geef het volgende
commando met achter origin de link van je github repository:

~~~~ {#bash9 .bash .numberLines}
git remote add origin https://github.com/accountnaamopgithub/naamvanjegithubrepo.git
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

## Push local master to github
~~~~ {#bash10 .bash .numberLines}
git push origin master
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Over dit document
Dit document is opgemaakt in pandoc markdown.
