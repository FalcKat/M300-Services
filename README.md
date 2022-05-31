# M300-Services

## Einleitung

## Inhaltsverzeichniss  

### [Theorie](M300/Theorie.md "Theorie")

### [Git](M300-Services/M300/Git.md "Git")

### [Vagrant](M300-Services/M300/Vagrant.md "Vagrant")

### [Docker](M300/Docker.md "Docker")

## Dokumentation
SSH-Key erstellen (lokal)

ACHTUNG: Auf Windows muss zuerst Git/Bash installiert werden. Anschliessend können die Befehle in der Git/Bash ausgeführt werden. Dabei handelt es sich nur um die Shell von Linux, die auf Windows ausgeführt wird. Alternativ können Sie für die meisten Befehle auch die PowerShell verwenden.

    Terminal (Bash) öffnen
    Folgenden Befehl mit der Account-E-Mail von GitHub einfügen:

      $  ssh-keygen -t rsa -b 4096 -C "beispiel@beispiel.com"

    Neuer SSH-Key wird erstellt:

      Generating public/private rsa key pair.

    Bei der Abfrage, unter welchem Namen der Schlüssel gespeichert werden soll, die Enter-Taste drücken (für Standard):

      Enter a file in which to save the key (~/.ssh/id_rsa): [Press enter]

    Nun kann ein Passwort für den Key festgelegt werden. Ich empfehle dieses zu setzen und anschliessend dem SSH-Agent zu hinterlegen, sodass keine erneute Eingabe (z.B. beim Pushen) notwendig ist:

      Enter passphrase (empty for no passphrase): [Passwort]
      Enter same passphrase again: [Passwort wiederholen]

SSH-Key dem SSH-Agent hinzufügen

Windows und Linux

Datei %HOME%/.ssh/id_rsa.pub oder $HOME/.ssh/id_rsa.pub in Zwischenablage kopieren.

macOS

    Terminal (Bash) öffnen
    SSH-Agent starten:

      $ eval "$(ssh-agent -s)"
      Agent pid 931

    Ab Version macOS High Sierra 10.12.2 muss das ~/.ssh/config File angepasst werden, damit SSH-Keys automatisch dem SSH-Agent hinzugefügt werden:

      $ sudo nano ~/.ssh/config
      
      Host *
      AddKeysToAgent yes
      UseKeychain yes
      IdentityFile ~/.ssh/id_rsa

    Nun muss der Schlüssel dem Agent nur noch hinzugefügt werden:

      $ ssh-add -k ~/.ssh/id_rsa

    Der SSH-Key muss nun nur noch kopiert und anschliessend dem GitHub-Account hinzugefügt werden (siehe "SSH-Key hinzufügen"):

      $ cat ~/.ssh/id_rsa.pub
      # Kopiert den Angezeiten Inhalt der id_rsa.pub Datei in die Zwischenablage
      
      
      ## Repository klonen

    Zu Testzwecken soll ein Repository geklont werden. Dazu sind folgende Befehle notwendig:
    Terminal (Bash) öffnen
    Repository klonen:

      $ git clone https://github.com/mc-b/M300

    In das M300-Verzeichnis wechseln:

      $ cd M300

    Repository aktualisieren und Status anzeigen:

      $ git pull

      Already up to date.

      $ git status

      Your branch is up to date with 'origin/master'.

    Die Statusmeldung soll dabei mitteilen, dass das lokale Repository mit dem Originalen übereinstimmt.

## Reflexion

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/ch/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/3.0/ch/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/ch/">Creative Commons Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 3.0 Schweiz Lizenz</a>
