% Git aantekeningen
% Arthur Schut
% 2018-08-27
# FIXME
- alle commando's in bash codeblocks zetten
- aantekening schrijven dat dit document is opgemaakt in pandoc markdown

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
- git add filename

# Adding multiple untracked files
- git add .

# Committing files
- git commit -m "beschrijving van je wijzigingen"

# Make and checkout new branch
- git checkout -b nameofnewbranch

# Checkout master branch
- git checkout master

# Merge somebranch into master branch
Branch master moet hiervoor wel je huidige branch zijn.

- git merge somebranch

# Connect to github
## Connect local repository to github repository
Maak op github een nieuwe repository. Idealiter met dezelfde naam als je lokale
repository. Kopieer de github link van je repository. Geef het volgende
commando met achter origin de link van je github repository:

- git remote add origin https://github.com/accountnaamopgithub/naamvanjegithubrepo.git

## Push local master to github
- git push origin master
