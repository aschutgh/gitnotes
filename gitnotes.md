% Git aantekeningen
% Arthur Schut
% 2018-08-27

# Some git resources
- https://maryrosecook.com/blog/post/git-from-the-inside-out
- https://jwiegley.github.io/git-from-the-bottom-up/
- https://git-scm.com/book/en/v2

# Git global config
Instellingen voor alle repositories op je systeem.

~~~~ {#globalconfig .bash .numberLines}
git config --global user.name "voornaam achternaam"
git config --global user.email naam@domeinnaam.nl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Initializing a repository in an existing directory

~~~~ {#gitinit .bash .numberLines}
git init
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Status
De status van je repository vraag je op met git status.

~~~~ {#gitstatus .bash .numberLines}
git status
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Adding untracked files
~~~~ {#gitadd .bash .numberLines}
git add filename
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Adding multiple untracked files
~~~~ {#gitaddmultiple .bash .numberLines}
git add .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Committing files
~~~~ {#gitcommit .bash .numberLines}
git commit -m "beschrijving van je wijzigingen"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Make and checkout new branch
~~~~ {#makebranch .bash .numberLines}
git checkout -b nameofnewbranch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Checkout master branch
~~~~ {#checkoutmaster .bash .numberLines}
git checkout master
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Merge somebranch into master branch
Branch master moet hiervoor wel je huidige branch zijn.

~~~~ {#gitmerge .bash .numberLines}
git merge somebranch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Delete local branch
~~~~ {#gitdelbranch .bash. numberLines}
git branch -d localbranchtodelete
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Connect to github
## Connect local repository to github repository
Maak op github een nieuwe repository. Idealiter met dezelfde naam als je lokale
repository. Kopieer de github link van je repository. Geef het volgende
commando met achter origin de link van je github repository:

~~~~ {#connectremote .bash .numberLines}
git remote add origin https://github.com/accountnaamopgithub/naamvanjegithubrepo.git
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

## Push local master to github
~~~~ {#pushtoremote .bash .numberLines}
git push origin master
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# About

Dit document is opgemaakt in pandoc markdown. Je kunt het met pandoc
converteren naar pdf. Voor conversie naar pdf moet je wel \LaTeX geïnstalleerd
hebben.

~~~~ {#pandocconvert .bash .numberLines}
pandoc -o gitnotes.pdf gitnotes.md
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
