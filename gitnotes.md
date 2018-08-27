% Git aantekeningen
% Arthur Schut
% 2018-08-27

# Git global config
Instellingen voor alle repositories op je systeem.

- git config --global user.name "voornaam achternaam"
- git config --global user.email naam@domeinnaam.nl

# Adding untracked files
- git add filename

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
repository. Kopiëer de github link van je repository. Geef het volgende
commando met achter origin de link van je github repository:

- git remote add origin https://github.com/accountnaamopgithub/naamvanjegithubrepo.git

## Push local master to github
- git push origin master
