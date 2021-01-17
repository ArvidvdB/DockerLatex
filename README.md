# LaTex docker image to build a PhD thesis
[![Build Status](https://travis-ci.com/arvidvdb/dockerlatex.svg?branch=master)](https://travis-ci.com/arvidvdb/dockerlatex)
[Thesis template of Jochem Rutgers](https://sites.google.com/site/jochemrutgers/publications/phd-thesis)
[Copy of thesis template of Jochem Rutgers](https://github.com/ArvidvdB/PhdThesisTemplate)

## Usage
Install [Docker](https://www.docker.com/)

### Linux
To view the possible commands of the themplate run:
```bash
docker run -it -v $(pwd):/data guusk/docker-latex-thesis make help
```
To build the template run:
```bash
docker run -it -v $(pwd):/data guusk/docker-latex-thesis make fonts all
```

### Windows PowerShell
To view the possible commands of the themplate run:
```pwsh
docker run -it -v ${PWD}:/data guusk/docker-latex-thesis make help
```
To build the template run:
```posh
docker run -it -v ${PWD}:/data guusk/docker-latex-thesis make fonts all
```

### Windows Commandline
To view the possible commands of the themplate run:
```winbatch
docker run -it -v %cd%:/data guusk/docker-latex-thesis make help
```
To build the template run:
```winbatch
docker run -it -v %cd%:/data guusk/docker-latex-thesis make fonts all
```


## LaTeX Docker Container

[![](https://dockerbuildbadges.quelltext.eu/status.svg?organization=brinkab&repository=dockerlatex&tag=latest&text=build)](https://hub.docker.com/r/brinkab/dockerlatex/)

Docker image use to build LaTeX document using TeX Live.
This image is based on [blang/latex](https://hub.docker.com/r/blang/latex/) and is extended with "make" and "git".
