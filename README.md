# MusilODD
This repository contains all MusilODD documents

Erläuterung des ODD, Katharina Godler

Musil-ODD/Schema für Mappe V/6

Folgende Module wurden für das Musilschema augewählt:
- core
- header
- textstructure
- msdescription
- transcr
- linking

Attribute/Werte
in alphabetischer Reihenfolge
@function (elementspezifische Änderungen)
Bei der Auszeichnung von Sonderzeichen wird innerhalb des Elements <metamark></metamark> mit dem Attribut @function die Funktion des Sonderzeichens beschrieben. In der Mappe V/6 kommen Deleaturzeichen, Zeichen, die einen Absatz aufheben und Schlaufen/Pfeile bei Wortumstellungen/Transpositionen vor.
Daher erhält das optionale Attribut @function die optionalen Werte „del“, „paragraph-remove“ und „transposition“.
@hand (Änderung der Attributklasse)
Musil korrigierte häufig mit schwarzer Tinte und zur Hervorhebung und Unterscheidung der Korrekturen setzte er folgende Farben ein: blau, braun, grün und rot. Für manche Korrekturen bzw. Notizen und Alternativvarianten verwendete er einen Bleistift.
Daher erhält das optionale Attribut @hand die optionalen Werte „#blue“, „#brown“, „#green“, „#pencil“ und „#red“.
@medium (elementspezifische Änderungen)
wird bei Musils Manuskripten auf der Objektebene (in der handNote) zur Beschreibung des Schreibmediums verwendet. Musil schrieb in der Mappe V/6 überwiegend mit schwarzer Tinte.
Daher erhält das optionale Attribut @medium den optionalen Wert „black_ink“.
@reason (elementspezifische Änderungen)
wird bei Musils Manuskripten auf der Textebene im Element <supplied></supplied> verwendet, wenn der Satz grammatikalisch unvollständig ist.
Daher erhält das optionale Attribut @reason den optionalen Wert „syntax“.
@rend (elementspezifische Änderungen)
wird bei Musils Manuskripten sowohl bei der Objektbeschreibung (1) als auch innerhalb der Textebene (2) verwendet.
Objektbeschreibung (im Header, bei Doppelblättern)
- Mit @rend wird innerhalb der Objektbeschreibung (<objectDesc></objectDesc> im <support></support>-Element) im Wert definiert, ob es sich um die Vorder- oder Rückseite 1/2 handelt – daher erhält das optionale Attribut @rend die optionalen Werte „recte“, „verso“, „recte_re_1“, „recte_re_2“ oder „verso_re_1“, „verso_re_2“ – „re“ steht hier für „regarding page“.
Textebene (Textausrichtung/-formatierung)
- Streichungen <del></del>, Ergänzungen <add></add>, Notizen <note></note> hat Musil häufig am Rand ausgeführt, einige wenige davon sind vertikal ausgerichtet. – daher erhält das optionale Attribut @rend den optionalen Wert „vertical“.
- Die Seitennummerierung am Beginn einer Seite erfolgt immer auf der rechten Seite des Manuskripts - daher erhält das optionale Attribut @rend den optionalen Wert „right“
- Sonderzeichen, die wieder gestrichen bzw. revidiert wurden - daher erhält das optionale Attribut @rend den optionalen Wert „strikethrough“.
- Revidierte Streichungen, die mit dem Element <restore></restore> wieder aufgehoben werden, wurden von Musil an einer Stelle in Mappe V/6 unterpunktet. - daher erhält das optionale Attribut @rend den optionalen Wert „dotted_underline“.
@rendition (elementspezifische Änderungen)
wird bei Musils Manuskripten bei der Beschreibung des Schreibprozesses einerseits auf Objektebene (im Header) zur Klassifizierung des Dokumenttyps (in der HandNote), andererseits auf der Textebene bei Wortumstellungen verwendet.
Objektbeschreibung
- Mit @rendition wird innerhalb der Objektbeschreibung (<physDesc></physDesc> innerhalb des <handNote></handNote>-Elements im Wert definiert, welchem Entwurftyp die Dokumente entsprechen. – hier haben wir Werte in deutscher Sprache zugelassen. – daher erhält das optionale Attribut @rendition den optionalen Wert „final_draft“ für Entwurfstyp 3
Textebene: Schreibprozess bei Wortumstellungen
- Mit @rendition mit dem Wert „before“ wird im Element <seg></seg> daraufhingewiesen, wie die Satzstellung vor der Wortumstellung ausgesehen hat. - daher erhält das optionale Attribut @rendition den optionalen Wert „before“.
@scribe (elementspezifische Änderungen)
wird bei Musils Manuskripten auf der Objektebene (in der handNote) zur Beschreibung der Schreiberhand verwendet. Der Schreiber ist hier Robert Musil.
Daher erhält das optionale Attribut @scribe den optionalen Wert „RMusil“.
@status (Änderung der Attributklasse)
Bei Streichungen in Streichungen wird zur Dokumentation des Schreibprozesses innerhalb des Elements <del></del> und im Element <add></add> mit dem Attribut @status die Ebene der Streichung/Ergänzung angegeben. In der Mappe V/6 konnten bis zu vier Korrekturschichten identifiziert werden.
Daher erhält das optionale Attribut @status die optionalen Werte „level2“, „level3“, „level4“.
@type (elementspezifische Änderungen)
wird bei Musils Manuskripten auf der Objektebene (in der idno/identifier) zur Objektidentifizierung verwendet. Dafür wird das Kürzel „sn“ für die Series-nova-Paginierung verwendet.
Daher erhält das optionale Attribut @type den optionalen Wert „sn“.
Zusatzinformationen zur Druckfahnen-Mappe
Problematik: Innerhalb des Elements <metamark> ist kein @hand-Attribut möglich, daher wird im Moment auf das @rend-Attribut zurückgegriffen.
Zusätzliche Werte bei der Druckfahnen-Mappe (diese wurden noch nicht im ODD beschrieben):
@function

Beim Element <metamark></metamark>
„hi“ – bei Erinnerungsstrichen am Rand
„compose“ – bei Zeichen zur Zusammensetzung zweier Wörter
„check“ – für Häkchen/Checkmarks
„insertion_space“ – für Trennzeichen
@rend

Beim Element <hi></hi>
„wavy_underline“ – bei gewellten Unterstreichungen
„erased“ – bei ausradierten (zurückgenommene/revidierte) Streichungen
@reason
Beim Element <supplied></supplied>
„erased“ – bei ausradierten Stellen am Rand
@type
Beim Element <note></note>
„scribal_abbreviation“ – bei Korrektorensiglen
