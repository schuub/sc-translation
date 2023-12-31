# Zur Übersetzung beitragen

## Programme und Tools
Wenn Du dich an der Übersetzung beteiligen möchtest, solltest Du einige Programme und Tools installieren.
### Git
Git benötigst Du, um deine Änderungen in unser Repository zu übertragen.

[GIt download Seite](https://git-scm.com/downloads)

Folge den Anweisungen des Installationsprogrammes. Es reicht, wenn Du alles auf den Standarteinstellungen belässt, sofern Du keine Erfahrung mit Git hast.
### Visual Studio Code
Ich empfehle hier das Programm Visual Studio Code. Es ist ein kostenloses Programm, mit dem Du alle möglichen Arten von Dateien bearbeiten kannst.

[VS-Code download](https://code.visualstudio.com/download)

Ausßerdem kannst Du den ganzen Ordner öffnen und siehst die Dateien links aufgelistet.

Wenn Du beide Dateien (global_de.ini und global_en.ini) markierst, einen Rechtsklick machst und dann "Compare Selected" auswählst, werden beide Dateien nebeneinander angezeigt. Zusätzlich siehst Du auch, welche Zeilen in der deutschen Übersetzung noch fehlen.

## Arbeiten mit Git
### Das Projekt klonen
Damit deine Änderungen auch bei uns ankommen, muss du zuerst das repository klonen. Öffne das "Git-Bash" programm. Es ist eine Kommandozeile.

Wenn das Projekt auf ein anderes Laufwerk als C: soll, dann kannst Du es wie folgt auswählen:
`cd e:`

Wenn die Dateien z.B. in das Verzeichnis `E:\projekt\translation` sollen, gehst Du wie folg vor:

- `cd e:` Enter
- `cd projekt/translation` Enter

Wenn Du im richtigen Verzeichnis angekommen bist, gibst Du folgendes ein:

```
git clone https://github.com/StarHeadSC/sc-translation.git
```

Als nächstes musst Du deine Logindaten von GitHub eingeben. Achtung: Wenn Du das Passwort eingibst, wird nichts von der Eingabe in dem Fenster angezeigt.

Die Dateien werden jetzt herunter geladen.

Nachdem alles herunter geladen wurde, wechselst Du in das Projektverzeichnis:

```
cd sc-translation
```

Als nächstes legen wir einen neuen Branch an, in den Du deine Änderungen übermittelst.

Dazu gibst Du folgendes in die Kommandozeile ein:

```
git checkout -b translation/<username>
```
Ersetze \<username> bitte mit deinem Nutzernamen von Github.

Jetzt kannst Du deine Übersetzungen in die global_de.ini einarbeiten.

Sobald Du mit deinen Änderungen an der deutschen Übersetzung fertig bist, musst Du erneut die Kommandozeile "Git Bash" öffnen.

Navigiere wieder zum Verzeichnis, in dem Du das Projekt geklont hast.

Deine Änderungen musst Du zuerst "commiten".

Gib dafür folgendes ein:

```
git commit -m "Zeile xxx bis Zeile xxx"
```

Gib bitte die Zeilennummern an, die Du übersetzt hast.

Als nächstes müssen die Änderungen "Gepushed" werden.

```
git push --set-upstream origin translation/<username>
```

Ersetzte hier wieder <username> mit deinem eigenen Nutzernamen.

Der Letzte Schritt ist die Erstellung eines Pull-Request. Dadurch werden wir darüber informiert, dass Du deine Änderungen abgeschlossen hast. Diese werden dann von uns geprüft und im Idealfall dann freigegeben und in die Eigentliche Übersetzung übernommen. Ganz automatisch.

Gehe dazu auf [https://github.com/StarHeadSC/sc-translation/branches](https://github.com/StarHeadSC/sc-translation/branches), suche deinen Branch und klicke auf `New pull request`.
Der titel sollte automatisch deiner letzten Commit-Nachricht entsprechen, Du kannst den titel aber auch anpassen. Optional kannst Du noch Hinweise oder Anmerkungen zu deinen Änderungen/Übersetzungen anfügen.
Mit einem Klick auf `Create pull request` wird dieser erstellt. Sobald wir diesen Freigegeben haben werden die Anpassungen übernommen.

Solltest Du noch weitere Fragen haben, kannst Du diese im Discord stellen.
