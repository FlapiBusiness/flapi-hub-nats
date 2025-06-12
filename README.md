# Crzgames - Nats Server
   
## 🛠 Tech Stack
- NATS (broker message)
- Kubernetes (Devops)
- CI / CD (Github actions)

<br /><br /><br /><br />


## 📦 Versionning
On utilise la convention SemVer : https://semver.org/lang/fr/ <br /><br />
Pour une Release classique : MAJOR.MINOR.PATCH <br />
Pour une Pre-Release, exemples : MAJOR.MINOR.PATCH-rc.0 OR MAJOR.MINOR.PATCH-beta.3 <br /><br />

Nous utilison release-please de Google pour versionner, via Github Actions. <br />
Pour que cela sois pris en compte il faut utiliser les conventionnal commits : https://www.conventionalcommits.org/en/v1.0.0/ <br />
Release Please crée une demande d'extraction de version après avoir remarqué que la branche par défaut contient des « unités publiables » depuis la dernière version. Une unité publiable est un commit sur la branche avec l'un des préfixes suivants : `feat` et `fix`. <br /><br />

La première Release que créer release-please automatiquement est la version : 1.0.0 <br />
Pour créer une Pre-Release faire un commit vide, par exemple si on'ai à la version 1.0.0, on peut faire : 
```bash
git commit --allow-empty -m "chore: release 1.1.0-rc.0" -m "Release-As: 1.1.0-rc.0"
```

<br /><br /><br /><br />

## Create NKEY Authentificator
Documentation official : [NATS NKey](https://docs.nats.io/using-nats/nats-tools/nk) <br />

1. Download and Install `Go` : https://go.dev/dl/
2. Download and Install `Nats NKey` :
```bash
go install github.com/nats-io/nkeys/nk@latest
```
3. `Generate NKey` for public key and private key (seed) :
```bash
nk -gen user -pubout
```

<br /><br /><br /><br />


## 🚀 Production

### ⚙️➡️ Automatic - Pipeline CI / CD :

<br />

### ✋ Manual :
