# Rebasing

---

## Lernziele

```
    rebase / rebase --interactive
```

 * Rebasing **dupliziert Commits**
 * **Risiken** und Nebenwirkungen
 * **Interaktives Rebasing**

---

### Rebase und Merge sind verwandt

![Rebasing und Merging](rebasing-and-merging.png)


---

### Rebase Beispiel 1

![Rebasing Beispiel vorher](abb-branches-beispiel-rebase-vorher.png)


---

### Rebase Beispiel 2

![Rebasing Beispiel nachher](abb-branches-beispiel-rebase-nachher.png)


---

### Rebase - Anwendung

    git rebase newbase

Welche Commits? Wohin?

 * Die neuen Commits entstehen auf `newbase`
 * Dupliziert werden
   - HEAD..newbase
   - Alle Commits in HEAD, die noch
     nicht in newbase enthalten sind

Ohne Parameter: Upstream Branch.

    git rebase

---

### Rebase - Konflikte

 * theirs vs. ours

---

### Übung 08: Rebasing

Starten sie im *Übungsverzeichnis* (wo sie das Zip-Archiv mit den
Übungen entpackt haben).
Öffnen sie die Anleitung im *Browser* (mit dem Kommando `start` auf
Windows, `xdg-open` auf Ubuntu,`open` auf MacOs).
**Achtung!** Es ist wichtig, die Übungen im *angegebenen
Startverzeichnis* zu beginnen. Achten Sie auf die Beschreibung:

    $ cd git-uebungen-<Zeitstempel z. B. 202005252000>
    $ start xdg-open aufgaben/08-rebasing-rebasing/index.html
    $ cd aufgaben/<angegebenes Startverzeichnis>

Folgen Sie dann den weiteren Anweisungen.


---


## Risiken und Nebenwirkungen

### Probleme mit duplizierten Commits

### (Un-)sichtbarkeit von Integrationen

---


### Verwandte Befehle

 * `commit --amend`
 * `reset HEAD~1`
 * `cherry-pick`
 * `filter-branch`


---


### Anwendung auf **Workflows**

---


![Feature Branching mit Rebasing](feature-branching-with-rebasing.png)
