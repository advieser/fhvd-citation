# Zitationsstile für die FHVD
Dieses Repo enthält die folgenden Zitationsstile für die Fachhochschule für Verwaltung und Diensteleistung (FHVD):
- `fhvd.csl`: Standardstil, nach den **Methodischen Hinweisen**
- `vwr-fhvd.csl`: Stil für Verwaltungsrecht

## `fhvd.csl`
Dieser Stil definiert die Folgenden Eintragsarten:
- **Buch** für Kommentare und Lehrbücher
- **Buchteil** für Teile von Herausgeberwerken
- **Zeitschriftenartikel** (und Conference Proceedings)
- **Webseite**

Diese Implementation deckt folgende Punkte der eigentlichen Spezifikation NICHT ab:
1. Bei Journals soll die Heftnummer angegeben werden, wenn "die Seiten des Jahrgangs / des Bandes nicht durchnummeriert sind". Dies geschieht hier NICHT automatisch. Standardmäßig wird die Heftnummer ausgegeben. Um dies steuern zu können, kann das Feld in Zotero leer gelassen werden. Wenn verfügbar, wird immer Jahr anstatt Band ausgegeben.
2. Dieser Still sortiert mehrere Einträge in einer Fußnote NICHT automatisch danach, ob es sich um Rechtsquellen handelt, wie eigentlich gefordert. Dies lässt sich stattdessen in Zotero beim Einfügen der Quellen kontrollieren.
3. Beim Einfügen von Fußnoten via Zotero muss IMMER eine konkrete Fundstelle mitangegeben werden. Dies geschieht NICHT automatisch. Die Angabe erfolgt als "S. 30f." oder "S. 30ff."
4. Bei Quellen des gleichen Autors in einer Fußnote wird NICHT automatisch "ders." oder "dies." verwendet.
5. Die Abkürzung "a.a.O." wird NICHT verwendet. Dies wäre möglich bei Zitation der gleichen Quelle in untersch. Fußnoten auf der selben Seite.
6. Die Abkürzung "Ebd." wird NICHT verwendet. Dies wäre möglich, wenn zwei aufeinander folgende Fußnoten die genau gleiche Quelle (samt Fundstelle) hätten.
7. Die URL einer Webseite sollte in einer Fußnote abgekürzt werden. Dies geschieht NICHT automatisch (da zotero kein Feld short-url hat).
8. Die Quellentypen Loseblattsammlung und E-Book sind NICHT definiert.
Diese Implementation weicht vom Beispiel für Sammelbände ab, insofern als dass die Jahreszahl der Konsistenzhalber gleich wie bei anderen Einträgen formatiert wird, und nicht in Klammern.

## `vwr-fhvd.csl`
Dieser Stil baut auf dem `fhvd.csl`-Stil vom **11.04.2024** und implementiert Konkretisierungen durch die Aufgabenstellung.
Er definiert die folgenden Eintragsarten:
- **Buch** für Lehrbücher
- **Buchteil** für Teile von Sammelwerken
- **Enzyklopädieeintrag** für Teile von Kommentaren
- **Zeitschriftenartikel**
- **Fall** für Urteile und Beschlüsse
- **Webseite**

Eine Anleitung kann [hier](Anleitung_VwR-FHVD.pdf) gefunden werden.

# Ressourcen
- [CSL 1.0.2 specification](https://docs.citationstyles.org/en/stable/specification.html)
- [CSL validator](https://validator.citationstyles.org/)
- [Zotero to CSL fields mappings](https://rawcdn.githack.com/POBrien333/zot2csl/1ebc3b5199b4e256d86b8feaa068a51d710f9e88/zot2csl_html/zotero_schema_output.html)
