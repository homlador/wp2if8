# Informatik WP II Stufe 8 - Schuljahr 2020/21

### Regeln

* Die Sitzordnung bleibt auch hier bestehen (Wegen Corona)
* Jedes Paar hat eine *Person A* (höhere Hausnummer) und eine *Person B*, der PC wird im __wöchentlichen Wechsel__ bedient, je nach Lernwoche.

Diese Woche, am <span id="curentDate">?</span>, ist <strong><span id="currentActive">?</span></strong> an der Reihe!

<script>
Date.prototype.getWeek = function() {
        var onejan = new Date(this.getFullYear(), 0, 1);
        return Math.ceil((((this - onejan) / 86400000) + onejan.getDay() + 1) / 7);
    }

    var now = new Date();
    var weekNumber = now.getWeek();
    var dayNames = ['Sonntag', 'Montag', 'Dienstag', 'Mittwoch', 'Donnerstag', 'Freitag', 'Samstag'];    
    //curentDate =  + " (" + weekNumber + ");
    curentDate = dayNames[now.getDay()] + " " + now.getDate() + "." + now.getMonth() + ".";
    var current = "?";
    if (weekNumber % 2 == 0) {
      currentActive = "A";
    } else {
      currentActive = "B";
    }
    document.getElementById("currentActive").innerHTML = currentActive;
    document.getElementById("curentDate").innerHTML = curentDate;
</script>

### Arbeitsmaterialien

Du brauchst...

* Deinen Benutzernamen und dein Passwort für die Schul-PCs
* Deinen Benutzernamen und dein Passwort für Teams
  * Apropos: Was ist ein [sicheres Passwort](https://checkdeinpasswort.de/)?
  * Tipp: Benutze einen Passwortmanager, z.B. [Bitwarden](https://bitwarden.com/)
* Einen Schnellhefter, falls es doch mal ausgedruckte Arbeitsmaterialien gibt
* Kopfhörer (werden wir manchmal brauchen)

Die Abgabe aller Arbeiten erfolgt über [Teams](https://teams.microsoft.com/). Dort könnt ihr auch jederzeit Fragen stellen.

### Welche Klassen- und Projektarbeiten gibt es?

| Thema                    | Form                                      | Wann                        |
| :----------------------- | ----------------------------------------- | --------------------------- |
| Recherche & Präsentation | Handout + Präsentation                    | Bis zu den Herbstferien     |
| Tabellenkalkulation      | Test + praktische Arbeit                  | Bis zu den Weihnachtsferien |
| Digitale Bilder + HTML   | praktische Arbeit + Kursarbeit auf Papier | Bis zu den Osterferien      |
| HTML + CSS               | Projektarbeit                             | Bis zu den Sommerferien     |

[//]: # (This syntax works like a comment, and won't appear in any output.)
[//]: # (It’s a little bizarre, but it works with MacDown and Pandoc.)
