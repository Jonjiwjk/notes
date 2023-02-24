# Installazione Portable Git

1) Scarica il file:

[PortableGit](https://github.com/git-for-windows/git/releases/download/v2.39.1.windows.1/PortableGit-2.39.1-64-bit.7z.exe)

2) Estrai nella cartella:

```cmd
C:\Users\{matricola}\PortableGit
```

3) Esporta la variabile d'ambiente da cmd:

```cmd
set Path="C:\Users\{matricola}\PortableGit"
```

5) Avvia git-bash da cmd:

```cmd
Microsoft Windows [Versione 10.0.19045.2673]
(c) Microsoft Corporation. Tutti i diritti sono riservati.

C:\Users\marco>git-bash

C:\Users\marco>
```

6) Configura i parametri globali di git (solo in fase di installazione):

> Esegui:
```bash
git config --global user.name "matricola-CognomeNome"
```
> Output:
```bash
marco@DESKTOP-72VFU3G MINGW64 ~
$ git config --global user.name "matricola-CognomeNome"
```

> Esegui:

$ git config --global user.email "matricola@studenti.marconiverona.edu.it"

```bash
marco@DESKTOP-72VFU3G MINGW64 ~
$ git config --global user.email "matricola@studenti.marconiverona.edu.it"

marco@DESKTOP-72VFU3G MINGW64 ~
$
```

7) Controlla che i parametri globali siano stati creati (creera un file *.gitconfig*):

```bash
marco@DESKTOP-72VFU3G MINGW64 ~
$ git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.interactive=true
color.ui=auto
help.format=html
diff.astextplain.textconv=astextplain
rebase.autosquash=true
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=helper-selector
user.name=matricola-CognomeNome
user.email=matricola@studenti.marconiverona.edu.it

marco@DESKTOP-72VFU3G MINGW64 ~
$ ls -las .*
1 -rw-r--r-- 1 marco 197610  3 Feb 23 23:18 .bash_history
1 -rw-r--r-- 1 marco 197610 86 Feb 23 23:24 .gitconfig
1 -rw-r--r-- 1 marco 197610 20 Feb 23 23:27 .lesshst

marco@DESKTOP-72VFU3G MINGW64 ~
$
```

---

## Approfondimenti

**NB**:

- In *`windows`* le path hanno una sintassi del tipo:

> {drive:}/{literal<sub>1</sub>}/.../{literal<sub>n</sub>}

il separatore fra un livello e l'altro è il carattere **/**

- In *`Posix`* le path hanno una sintassi del tipo:

> {root}\\{literal<sub>1</sub>}\\...\\{literal<sub>n</sub>}

dove la root è il carattere **\\** ed i separatori fra un livello e l'altro è sempre il carattere **\\**
