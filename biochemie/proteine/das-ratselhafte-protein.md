# Das rätselhafte Protein

## Das rätselhafte Protein: Eine Bioinformatik-Expedition

Quelle: [https://www.embl.org/](https://www.embl.org/)

{% tabs %}
{% tab title="ÜBERSICHT" %}
Gemeinsam werden wir in die faszinierende Welt der Bioinformatik eintauchen, um die Geheimnisse von Proteinen zu entschlüsseln, einem der grundlegenden Bausteine der Molekularbiologie. Anhand einer Reihe von interaktiven Übungen werden wir untersuchen, wie Proteine hergestellt werden, wie sie aussehen und wie sie sich über die verschiedenen Arten hinweg entwickelt haben. Begleite uns auf diesem fiktiven wissenschaftlichen Abenteuer, das mit realen Forschungsaktivitäten am EMBL verwoben ist, und gewinne dabei Einblicke in moderne Forschungsmethoden.

Ziel dieser Aktivität ist es, unser Verständnis von Proteinen und ihrer Evolution zu vertiefen und gleichzeitig wertvolle Einblicke in die praktischen Anwendungen der Bioinformatik in der wissenschaftlichen Forschung zu geben.
{% endtab %}

{% tab title="IHRE AUFGABE" %}
Während der[ TREC-Expedition](https://www.embl.org/about/info/trec/) (Traversing European Coastlines) sammeln Forscher\*innen zahlreiche biologische Proben von der europäischen Küste, um diese Ökosysteme zu untersuchen. Diese Proben werden aus dem Boden, Sedimenten, Aerosol, Flachwasser und dem Meer gewonnen und mit wissenschaftlichen Techniken wie Mikroskopie oder DNA-Sequenzierung sorgfältig analysiert.

Kürzlich stieß das TREC-Team auf eine verblüffende Entdeckung in einer ihrer Proben aus dem flachen Wasser – eine DNA-Sequenz, die mit keiner bekannten Sequenz übereinstimmt. Die Forscher\*innen sind von diesem Fund fasziniert und haben eine Aufgabe für dich: Kannst du ihnen helfen, das von dieser Sequenz kodierte Protein zu identifizieren und die biologische Funktion des Proteins zu entschlüsseln? Kannst du außerdem dabei helfen, die Spezies zu identifizieren, von der die Sequenz stammt und die evolutionären Beziehungen zu anderen Organismen zu erforschen?
{% endtab %}

{% tab title="BIOINFORMATISCHE METHODEN" %}
Die meisten der Methoden, die wir im Rahmen dieser Aktivität einsetzen werden, wurden vom EMBL-EBI entwickelt und Wissenschaftler\*innen in aller Welt **kostenlos** zur Verfügung gestellt.

**EMBOSS Transeq**\
Link:[ https://www.ebi.ac.uk/Tools/st/emboss\_transeq/](https://www.ebi.ac.uk/Tools/st/emboss_transeq/)\
Eine Methode zur Übersetzung von Nukleinsäuresequenzen (DNA oder RNA) in ihre entsprechenden Aminosäuresequenzen.

**NCBI BLAST+ (Basic Local Alignment Search Tool)**\
Link:[ http://www.ebi.ac.uk/Tools/sss/ncbiblast/](http://www.ebi.ac.uk/Tools/sss/ncbiblast/%0B)   \
Eine Methode zur Identifizierung und zum Vergleich biologischer Sequenzinformationen, wie z. B. Aminosäuresequenzen. Es ermöglicht Forscher\*innen ein bestimmtes Protein mit einer Datenbank von Sequenzen zu vergleichen. Dies ermöglicht die Identifizierung unbekannter Proteine.

**Clustal Omega**\
Link:[ https://www.ebi.ac.uk/Tools/msa/clustalo/](https://www.ebi.ac.uk/Tools/msa/clustalo/)   \
Eine Methode für das Alignment und den Vergleich mehrerer Sequenzen, die speziell für Aminosäuresequenzen geeignet ist.

**Simple Phylogeny**\
Lin&#x6B;**:**[ https://www.ebi.ac.uk/Tools/phylogeny/simple\_phylogeny/](https://www.ebi.ac.uk/Tools/phylogeny/simple_phylogeny/)  \
Eine Methode zur Durchführung grundlegender phylogenetischer Analysen an einem multiplen Sequenzalignment.

**UniProt-Datenbank (Universal Protein Resource)**\
Link:[ ](http://www.uniprot.org/%0B)[http://www.uniprot.org/](http://www.uniprot.org/)\
Ein umfassender Katalog von Proteininformationen, einschließlich Proteinsequenzen und deren Funktionen.

**AlphaFold Datenbank**\
Link:[ https://alphafold.ebi.ac.uk/](https://alphafold.ebi.ac.uk/) \
Eine Datenbank für Proteinstrukturvorhersagen. AlphaFold ist ein künstliches Intelligenz (KI) System, das die 3D-Struktur eines Proteins auf der Grundlage seiner Aminosäuresequenz vorhersagen kann. Die AlphaFold-Datenbank ist auch in die UniProt-Datenbank integriert.

**Hinweis:** Die Methoden benötigen einige Zeit für die Berechnungen. Daher kann ein wenig Geduld erforderlich sein.
{% endtab %}
{% endtabs %}

### Teil 1: Von der DNA zum Protein

{% tabs %}
{% tab title="ÜBERSICHT" %}
Wir haben gerade eine E-Mail von den TREC-Forscher\*innen erhalten, die die DNA-Sequenz enthält. Um zu verstehen, für welches Protein diese Sequenz kodiert, müssen wir die DNA-Sequenz zunächst in eine Aminosäuresequenz umwandeln, die auch als Primärstruktur des Proteins bekannt ist.

Wir werden die Bioinformatik-Methode EMBOSS Transeq verwenden, um uns bei diesem Prozess zu unterstützen. EMBOSS Transeq ermöglicht es uns, die biologischen Prozesse Transkription (DNA zu RNA) und Translation (RNA zu Protein) zusammenzuführen und eine Aminosäuresequenz direkt aus der DNA-Sequenz zu erstellen.&#x20;

Beginne die Aktivität, indem du die Anweisungen auf der Registerkarte “Deine Aufgabe” befolgst und versuchst, die begleitenden Fragen zu beantworten.
{% endtab %}

{% tab title="IHRE AUFGABE" %}
**Bitte befolge die unten aufgeführten Schritte:**

**1.** Auf der Registerkarte “Sequenz” findest du die unbekannte DNA-Sequenz mit der Bezeichnung “Unbekannte DNA”.\
**2.** Kopiere die Sequenz und gehe zur Registerkarte “EMBOSS Transeq”, wo du Anweisungen findest, wie du die Aminosäuresequenz des unbekannten Proteins mit der EMBOSS Transeq-Methode identifizieren kannst.\
**3.** Versuche, die Fragen auf der Registerkarte “Fragen” zu beantworten.
{% endtab %}

{% tab title="SEQUENZ" %}
Unbekannte DNA:

```

>New species (Unknown) 
ATGAACGGCACCGAGGGCCCCTTCGGCTACATCCCCATGAGCAACGCCACCGGCCTGGTG
AGGAGCCCCTACGACTACCCCCAGTACTACCTGGTGCCCCCCTGGGGCTACGCCTGCCTG
GCCGCCTACATGTTCCTGCTGATCCTGACCGGCTTCCCCGTGAACTTCCTGACCCTGTAC
GTGACCATCGAGCACAAGAAGCTGAGGAGCCCCCTGAACTACATCCTGCTGAACCTGGCC
GTGGCCGACCTGTTCATGGTGATCGGCGGCTTCACCACCACCATGTGGACCAGCCTGGAC
GGCTACTTCGTGTTCGGCAGGATGGGCTGCAACATCGAGGGCTTCTTCGCCACCCTGGGC
GGCGAGATCGCCCTGTGGAGCCTGGTGGTGCTGAGCATGGAGAGGTGGATCGTGGTGTGC
AAGCCCATCAGCAACTTCAGGTTCGGCGAGAACCACGCCGTGATGGGCGTGGCCTTCAGC
TGGTTCATGGCCGCCGCCTGCGCCGTGCCCCCCCTGGTGGGCTGGAGCAGGTACATCCCC
GAGGGCATGCAGTGCAGCTGCGGCATCGACTACTACACCAGGGCCGAGGGCTTCAACAAC
GAGAGCTTCGTGATCTACATGTTCGTGGTGTTCTTCACCTGCCCCCTGACCATCATCACC
TTCTGCTACGGCAGGCTGGTGTGCACCGTGAAGGAGGCCGCCGCCCAGCAGCAGGAGAGC
GAGACCACCCAGAGGGCCGAGAGGGAGGTGACCAGGATGGTGATCATCACCTTCGTGGCC
TTCCTGGCCTGCTGGGTGCCCTACGCCAGCGTGGCCTGGTACATCTTCACCCACCAGGGC
AGCGAGTTCGGCCCCGTGTTCATGACCATCCCCGCCTTCTTCGCCAAGAGCAGCGCCGTG
TACAACCCCGTGATCTACATCTGCCTGAACAAGCAGTTCAGGCACTGCATGATCACCACC
CTGTGCTGCGGCAAGAACCCCTTCGAGGAGGAGGAGGGCAGCACCACCGCCAGCAAGACC
GAGGCCAGCAGCGTGTGCAGCGTGAGCCCCCACGCC
```
{% endtab %}

{% tab title="EMBOSS Transeq" %}
**1.** [Rufe die EMBOSS Transeq-Methode](https://www.ebi.ac.uk/jdispatcher/st/emboss_transeq) auf.\
**2.** Füge die DNA-Sequenz (einschließlich des Größer-als-Symbols (>) und des Sequenznamens) in das Abfragefeld ein (STEP 1). Stelle sicher, dass im Feld “Parameters” (STEP 2) “frame=1” und “Codon table=Standard codon” ausgewählt ist. Sende dann deine Anfrage ab, indem du auf “Submit” klickst. \
**3.** Sieh dir die angezeigte Datentabelle an und versuche, die mit der Aufgabe verbundenen Fragen zu beantworten. Für eine bessere Visualisierung kannst du auf “Show Colors” klicken.\
**4.** Speichere oder kopiere die Aminosäuresequenz für die nächste Aufgabe.

**Hinweis:** Die in den Ergebnissen verwendeten Farben entsprechen den spezifischen chemischen Eigenschaften der Aminosäuren. Die Aminosäuren werden in Klammern als Ein-Buchstaben-Code angezeigt:\
– Kleine + hydrophobe Aminosäuren (AVFPMILW): Rot \
– Saure Aminosäuren (DE): Blau\
– Basische Aminosäuren (RK): Magenta\
– Aminosäuren mit Hydroxyl-, Sulfhydryl- oder Amingruppen + Glycine (STYHCNGQ): Grün
{% endtab %}

{% tab title="FRAGE" %}
Welche Arten von Aminosäuren sind in der Proteinsequenz am häufigsten vertreten?

Du kannst auf “Show Colors” klicken, um Informationen über die chemischen Eigenschaften der einzelnen Aminosäuren zu erhalten.
{% endtab %}
{% endtabs %}

<details>

<summary>Antworten zu den Fragen</summary>

<mark style="color:green;">Wenn wir auf "Farben anzeigen" klicken, sehen wir, dass die meisten Aminosäuren entweder rot oder grün gefärbt sind.</mark>

<mark style="color:green;">Rot weist auf kleine und hydrophobe Aminosäuren hin, während Grün Aminosäuren mit entweder einer Hydroxyl-, Sulfhydryl- oder Aminogruppe anzeigt.</mark>

</details>

### Teil 2: Identität und Funktion von Proteinen

{% tabs %}
{% tab title="ÜBERSICHT" %}
In Teil 1 haben wir die unbekannte DNA-Sequenz erfolgreich in eine Aminosäuresequenz übersetzt. Unsere Expedition, um die Geheimnisse dieses unbekannten Proteins zu entschlüsseln, hat jedoch gerade erst begonnen. Zum jetzigen Zeitpunkt wissen wir noch nichts über die Funktion des Proteins. Um weitere Erkenntnisse zu gewinnen, werden wir eine umfassende Datenbank mit bekannten Proteinsequenzen durchsuchen, um ähnliche Sequenzen zu finden, die Aufschluss über die Funktion des Proteins geben könnten.

Wir werden die Bioinformatik-Methode NCBI BLAST+ verwenden, um uns bei diesem Prozess zu unterstützen. NCBI BLAST+ ermöglicht es, Aminosäuresequenzen zu identifizieren und zu vergleichen. Hier werden wir es verwenden, um bekannte Sequenzen zu identifizieren, die unserer unbekannten Sequenz ähnlich sind.
{% endtab %}

{% tab title="AUFGABE" %}
**Bitte befolge die unten aufgeführten Schritte:**\
**1.** Kopiere die Aminosäuresequenz, die du kürzlich übersetzt hast. Du findest sie in der vorangegangenen Aufgabe oder kannst sie über den angegebenen [Link hier](https://drive.google.com/file/d/1M-65TwCxZ_DPRwjGs9hHMjhUjA2lJwPz/view?usp=sharing) herunterladen. Verwende einen Texteditor (z.B. TextEdit und Notepad), um FASTA-Dateien zu öffnen.\
**2.** Gehe auf die Registerkarte “NCBI BLAST+” und befolge die Anweisungen, um mit der NCBI BLAST+ Methode nach der Identität des Proteins zu suchen.  \
**3.** Versuche, die Fragen auf der Registerkarte “Fragen” zu beantworten.
{% endtab %}

{% tab title="NCBI Blast +" %}
Greife auf die[ NCBI BLAST-Methode](https://www.ebi.ac.uk/jdispatcher/sss/ncbiblast) zu.\
**2.** Vergewissere dich in ‚STEP 1‘, dass die Datenbank “UniProtKB/Swiss-Prot” ausgewählt ist. \
**3.** Füge in ‚STEP 2‘ die Aminosäuresequenz in das Abfragefeld ein.\
**4.** Vergewissere dich in ‚STEP 3‘, dass das Programm “blastp” ausgewählt ist.      \
**5.** Führe die Methode aus, indem du auf “Submit” klickst.\
**6.** Prüfe die Datentabelle (“Summary Table”) und versuche, die mit der Aufgabe verbundenen Fragen zu beantworten.

**Hinweis:** In der Übersichtstabelle werden Sequenzen aus der Datenbank angezeigt, die nach ihrer Ähnlichkeit mit der eingefügten Sequenz aufgelistet sind. Die ähnlichste Sequenz, auch bekannt als bester Treffer, wird am Anfang der Liste angezeigt.
{% endtab %}

{% tab title="FRAGEN" %}
**1.** Welches Protein ist der beste Treffer in der Proteindatenbank und von welcher Art stammt es?\
**2.** Wie hoch ist der Prozentsatz der Identität zwischen dem unbekannten Protein und dem besten Treffer? \
**3.** Welche biologische Funktion ist für den besten Treffer bekannt? Um diese Informationen zu erhalten, klicke mit der rechten Maustaste auf die zweite Spalte der Ergebnistabelle (DB:ID) und öffne den Link in einer neuen Registerkarte.
{% endtab %}
{% endtabs %}

<details>

<summary>Antworten zu den Fragen</summary>

1. Welches Protein und welche Spezies erzielt den besten Treffer in der Protein-Datenbank?

<mark style="color:green;">Das Protein Rhodopsin der Spezies Sardina pilchardus liefert den besten Treffer. (Datenbank-ID:</mark>

<mark style="color:green;">SP:OPSD\_SARPI)</mark>

2. Wie hoch ist der Prozentsatz der Identität, die das "unbekannte Protein" und der beste Treffer teilen?

<mark style="color:green;">Das unbekannte Protein teilt eine Identität von 98,9 % mit dem besten Treffer, dem Rhodopsin von Sardina pilchardus.</mark>

3. Was ist die bekannte biologische Funktion des besten Treffers? Diese Information kann gefunden werden, indem man auf den Link in der zweiten Spalte der Ergebnistabelle (DB:ID) klickt.

<mark style="color:green;">Rhodopsin (der beste Treffer), auch bekannt als Sehpurpur, ist ein Protein, das für die Bildformation unter Bedingungen mit wenig Licht erforderlich ist. Es handelt sich um einen sensorischen Rezeptor, der in einer breiten Palette von Organismen vorhanden ist, von Wirbeltieren bis zu Bakterien.</mark>

</details>

### Teil 3: Multiples Sequenzalignment

{% tabs %}
{% tab title="ÜBERSICHT" %}
Sehr gut gemacht! In Teil 2 haben wir herausgefunden, dass unser unbekanntes Protein höchstwahrscheinlich Rhodopsin ist – das lichtempfindliche Protein der Netzhaut. Rhodopsine gehören zu einer Klasse von Proteinen, die Opsine genannt werden und meistens ein Chromophor namens Retinal binden.

Jetzt wollen wir mehr über Rhodopsine erfahren und Methoden der Bioinformatik nutzen, um ihre evolutionären Veränderungen zu untersuchen. Dies wird uns dabei helfen, die Entwicklung der neuen Art zu verstehen und eng verwandten Arten zu identifizieren. Zu diesem Zweck führen wir ein sogenanntes multiples Sequenzalignment durch. Dies ist eine Technik, bei der zahlreiche Rhodopsin-Aminosäuresequenzen aus verschiedenen Arten übereinander angeordnet werden. Das Alignment stellt sicher, dass ähnliche Aminosäuren möglichst konsistent übereinander angeordnet sind. Wenn dies bei einem großen Teil der Aminosäuren der Fall ist, bedeutet es, dass die Sequenzen eng miteinander verwandt sind.&#x20;

Eine Reihe von vorbereiteten Sequenzen findest du auf der Registerkarte “Sequenzen”. Die erste Sequenz (“>New species (Unknown)”) entspricht dem Rhodopsin, das du zuvor entschlüsselt hast. Die anderen Sequenzen entsprechen Rhodopsinen von 20 verschiedenen Organismen, darunter Rhodopsine vom Menschen und gängigen Forschungsorganismen wie Fruchtfliegen, Hausmäuse, Ratten und Zebrafische.
{% endtab %}

{% tab title="AUFGABE" %}
**1.** Verwende die auf der Registerkarte “Sequenzen” verfügbaren Rhodopsinesequenzen von 21 verschiedenen Arten und führe mit Hilfe der EMBL-EBI Clustal Omega Methode ein multiples Sequenzalignment durch.\
**2.** Befolge die Anweisungen auf der Registerkarte “Clustal Omega”.\
**3.** Versuche, die Fragen auf der Registerkarte “Fragen” zu beantworten.
{% endtab %}

{% tab title="SEQUENZEN" %}
Ihre Eingabesequenzen:

```

>New species (Unknown) 
MNGTEGPFGYIPMSNATGLVRSPYDYPQYYLVPPWGYACLAAYMFLLILTGFPVNFLTLY
VTIEHKKLRSPLNYILLNLAVADLFMVIGGFTTTMWTSLBGYFVFGRMGCNIEGFFATLG
GEIALWSLVVLSMERWIVVCKPISNFRFGENHAVMGVAFSWFMAAACAVPPLVGWSRYIP
EGMQCSCGIDYYTRAEGFNNESFVIYMFVVFFTCPLTIITFCYGRLVCTVKEAAAQQQES
ETTQRAEREVTRMVIITFVAFLACWVPYASVAWYIFTHQGSEFGPVFMTIPAFFAKSSAV
YNPVIYICLNKQFRHCMITTLCCGKNPFEEEEGSTTASKTEASSVCSVSPHA

>Drosophila melanogaster (Fruit fly)
MASLHPPSFAYMRDGRNLSLAESVPAEIMHMVDPYWYQWPPLEPMWFGIIGFVIAILGTM
SLAGNFIVMYIFTSSKGLRTPSNMFVVNLAFSDFMMMFTMFPPVVLNGFYGTWIMGPFLC
ELYGMFGSLFGCVSIWSMTLIAYDRYCVIVKGMARKPLTATAAVLRLMVVWTICGAWALM
PLFGWNRYVPEGNMTACGTDYFAKDWWNRSYIIVYSLWVYLTPLLTIIFSYWHIMKAVAA
HEKAMREQAKKMNVASLRNSEADKSKAIEIKLAKVALTTISLWFFAWTPYTIINYAGIFE
SMHLSPLSTICGSVFAKANAVCNPIVYGLSHPKYKQVLREKMPCLACGKDDLTSDSRTQA
TAEISESQA

>Sus scrofa (Wild boar)
MNGTEGPNFYVPFSNKTGVVRSPFEYPQYYLAEPWQFSMLAAYMFMLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGLALTWVMALACAAPPLVGWSRYIP
EGLQCSCGIDYYTLKPEVNNESFVIYMFVVHFSIPLVIIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVVAFLICWLPYASVAFYIFTHQGSDFGPIFMTIPAFFAKSASI
YNPVIYIMMNKQFRNCMLTTLCCGKNPLGDDEASTTTSKTETSQVAPA

>Bos taurus (Cattle)
MNGTEGPNFYVPFSNKTGVVRSPFEAPQYYLAEPWQFSMLAAYMFLLIMLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVAFTWVMALACAAPPLVGWSRYIP
EGMQCSCGIDYYTPHEETNNESFVIYMFVVHFIIPLIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIAFLICWLPYAGVAFYIFTHQGSDFGPIFMTIPAFFAKTSAV
YNPVIYIMMNKQFRNCMVTTLCCGKNPLGDDEASTTVSKTETSQVAPA

>Homo sapiens (Human)
MNGTEGPNFYVPFSNATGVVRSPFEYPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVLGGFTSTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVAFTWVMALACAAPPLAGWSRYIP
EGLQCSCGIDYYTLKPEVNNESFVIYMFVVHFTIPMIIIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIAFLICWVPYASVAFYIFTHQGSNFGPIFMTIPAFFAKSAAI
YNPVIYIMMNKQFRNCMLTTICCGKNPLGDDEASATVSKTETSQVAPA

>Mus musculus (House mouse) 
MNGTEGPNFYVPFSNVTGVVRSPFEQPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVVFTWIMALACAAPPLVGWSRYIP
EGMQCSCGIDYYTLKPEVNNESFVIYMFVVHFTIPMIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIFFLICWLPYASVAFYIFTHQGSNFGPIFMTLPAFFAKSSSI
YNPVIYIMLNKQFRNCMLTTLCCGKNPLGDDDASATASKTETSQVAPA

>Gallus gallus (Red junglefowl)
MNGTEGQDFYVPMSNKTGVVRSPFEYPQYYLAEPWKFSALAAYMFMLILLGFPVNFLTLY
VTIQHKKLRTPLNYILLNLVVADLFMVFGGFTTTMYTSMNGYFVFGVTGCYIEGFFATLG
GEIALWSLVVLAVERYVVVCKPMSNFRFGENHAIMGVAFSWIMAMACAAPPLFGWSRYIP
EGMQCSCGIDYYTLKPEINNESFVIYMFVVHFMIPLAVIFFCYGNLVCTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIAFLICWVPYASVAFYIFTNQGSDFGPIFMTIPAFFAKSSAI
YNPVIYIVMNKQFRNCMITTLCCGKNPLGDEDTSAGKTETSSVSTSQVSPA

>Cricetulus griseus (Chinese Hamster)
MNGTEGPNFYVPFSNATGVVRSPFEYPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVICKPMSNFRFGENHAIMGVVFTWIMALACAAPPLVGWSRYIP
EGMQCSCGVDYYTLKPEVNNESFVIYMFVVHFTIPLIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVILMVVFFLICWFPYAGVAFYIFTHQGSNFGPIFMTLPAFFAKSSSI
YNPVIYIMMNKQFRNCMLTTLCCGKNILGDDEASATASKTETSQVAPA

>Canis lupus familiaris (Dog)
MNGTEGPNFYVPFSNKTGVVRSPFEYPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNVEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVAFTWVMALACAAPPLAGWSRYIP
EGMQCSCGIDYYTLKPEINNESFVIYMFVVHFAIPMIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIAFLICWVPYASVAFYIFTHQGSDFGPIFMTLPAFFAKSSSI
YNPVIYIMMNKQFRNCMITTLCCGKNPLGDDEASASASKTETSQVAPA

>Danio rerio (Zebrafish)
MNGTEGPAFYVPMSNATGVVRSPYEYPQYYLVAPWAYGLLAAYMFFLIITGFPVNFLTLY
VTIEHKKLRTPLNYILLNLAIADLFMVFGGFTTTMYTSLHGYFVFGRLGCNLEGFFATLG
GEMGLWSLVVLAIERWMVVCKPVSNFRFGENHAIMGVAFTWVMACSCAVPPLVGWSRYIP
EGMQCSCGVDYYTRTPGVNNESFVIYMFIVHFFIPLIVIFFCYGRLVCTVKEAAAQQQES
ETTQRAEREVTRMVIIMVIAFLICWLPYAGVAWYIFTHQGSEFGPVFMTLPAFFAKTSAV
YNPCIYICMNKQFRHCMITTLCCGKNPFEEEEGASTTASKTEASSVSSSSVSPA

>Rattus norvegicus (Brown rat)
MNGTEGPNFYVPFSNITGVVRSPFEQPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIGLWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVAFTWVMALACAAPPLVGWSRYIP
EGMQCSCGIDYYTLKPEVNNESFVIYMFVVHFTIPMIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIFFLICWLPYASVAMYIFTHQGSNFGPIFMTLPAFFAKTASI
YNPIIYIMMNKQFRNCMLTSLCCGKNPLGDDEASATASKTETSQVAPA

>Delphinus delphis (Short-beaked common dolphin)
MNGTEGLNFYVPFSNKTGVVRSPFEYPQYYLAEPWQFSVLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVANLFMVFGGFTTTLYTSLHAYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGLALTWIMAMACAAPPLVGWSRYIP
EGMQCSCGIDYYTLSPEVNNESFVIYMFVVHFTIPLVIIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVVAFLICWVPYASVAFYIFTHQGSDFGPIFMTIPSFFAKSSSI
YNPVIYIMMNKQFRNCMLTTLCCGRNPLGDDEASTTASKTETSQVAPA

>Mesoplodon bidens (Sowerby's beaked whale)
MNGTEGLNFYVPFSNHTGVVRSPFEYPQYYLAEPWQFSVLAAYMFLLIMLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVANLFMVLGGFTTTLYTSMHAYFIFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGLALTWIMALACAAPPLVGWSRYIP
EGMQCSCGVDYYTPSPEVNNESFVVYMFVVHFSIPMVIIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVVIMVVAFLICWVPYASVAFYIFTHQGSNFGPIFMTIPSFFAKSSAI
YNPVIYIMMNKQFRNCMLTTLCCGRNPLGDDEVSTTASKTETSQVAPA

>Phoca vitulina (Harbor seal)
MNGTEGPNFYVPFSNKTGVVRSPFEFPQYYLAEPWQFSMLAAYMFLLIVLGFPINFLTLY
VTVQHKKLRTPLNYILLNLAVADLFMVFGGFTTTLYTSLHGYFVFGPTGCNLEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFGENHAIMGVGFTWVMALACAAPPLVGWSRYIP
EGMQCSCGIDYYTLKPEVNNESFVIYMFVVHFTIPMIVIFFCYGQLVFTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVIAFLICWVPYASVAFYIFTHQGSNFGPIFMTLPAFFAKAASI
YNPVIYIMMNKQFRTCMITTLCCGKNPLGDDEVSASASKTETSQVAPA

>Scyliorhinus canicula (Catshark)
MNGTEGENFYIPMSNKTGVVRSPFDYPQYYLAEPWKFSVLAAYMFFLIIAGFPVNFLTLY
VTIQHKKLRQPLNYILLNLAVADLFMIFGGFPSTMITSMNGYFVFGPSGCNFEGFFATLG
GEIGLWSLVVLAIERYVVVCKPMSNFRFGSQHAFMGVGLTWIMAMACAFPPLVGWSRYIP
EGMQCSCGIDYYTLKPEVNNESFVIYMFVVHFSIPLTIIFFCYGRLVCTVKEAAAQQQES
ETTQRAEREVTRMVIIMVIAFLICWLPYASVAFFIFCNQGSEFGPIFMTIPAFFAKAASL
YNPLIYILMNKQFRNCMITTICCGKNPFEEEESTSASASKTEASSVSSSQVAPA

>Carassius auratus (Goldfish)
MNGTEGDMFYVPMSNATGIVRSPYDYPQYYLVAPWAYACLAAYMFFLIITGFPVNFLTLY
VTIEHKKLRTPLNYILLNLAISDLFMVFGGFTTTMYTSLHGYFVFGRVGCNPEGFFATLG
GEMGLWSLVVLAFERWMVVCKPVSNFRFGENHAIMGVVFTWFMACTCAVPPLVGWSRYIP
EGMQCSCGVDYYTRPQAYNNESFVIYMFIVHFIIPLIVIFFCYGRLVCTVKEAAAQHEES
ETTQRAEREVTRMVVIMVIGFLICWIPYASVAWYIFTHQGSEFGPVFMTLPAFFAKTAAV
YNPCIYICMNKQFRHCMITTLCCGKNPFEEEEGASTTASKTEASSVSSSSVSPA

>Lithobates catesbeianus (American bullfrog)
MNGTEGPNFYVPMSNKTGIVRSPFEYPQYYLAEPWKYSVLAAYMFLLILLGLPINFMTLY
VTIQHKKLRTPLNYILLNLAFANHFMVLCGFTITMYTSLHGYFVFGQTGCYFEGFFATLG
GEIALWSLVVLAIERYIVVCKPMSNFRFGENHAMMGVAFTWIMALACAVPPLFGWSRYIP
EGMQCSCGVDYYTLKPEVNNESFVIYMFVVHFLIPLIIISFCYGRLVCTVKEAAAQQQES
ATTQKAEKEVTRMVVIMVIFFLICWVPYAYVAFYIFTHQGSEFGPIFMTVPAFFAKSSAI
YNPVIYIMLNKQFRNCMITTLCCGKNPFGDEDASSAATSKTEATSVSTSQVSPA

>Bufo bufo (Common toad)
MNGTEGPNFYIPMSNKTGVVRSPFEYPQYYLAEPWQYSILCAYMFLLILLGFPINFMTLY
VTIQHKKLRTPLNYILLNLAFANHFMVLCGFTVTMYSSMNGYFILGATGCYVEGFFATLG
GEIALWSLVVLAIERYVVVCKPMSNFRFSENHAVMGVAFTWIMALSCAVPPLLGWSRYIP
EGMQCSCGVDYYTLKPEVNNESFVIYMFVVHFTIPLIIIFFCYGRLVCTVKEAAAQQQES
ATTQKAEKEVTRMVIIMVVFFLICWVPYASVAFFIFSNQGSEFGPIFMTVPAFFAKSSSI
YNPVIYIMLNKQFRNCMITTLCCGKNPFGEDDASSAATSKTEASSVSSSQVSPA

>Oryzias latipes (Japanese rice fish)
MNGTEGPYFNVPMVNTTGIVRSPYEYPQYYLVSPAAYAALGAYMFFLILVGFPINFLTLY
VTLEHKKLRTPLNYILLNLAVADLFMVFGGFTTTMYTSMHGYFVLGRLGCNLEGFFATLG
GEIGLWSLVVLAIERWVVVCKPISNFRFGENHAIMGLVFTWIMAASCAVPPLVGWSRYIP
EGMQCSCGVDYYTRAEGFNNESFVVYMFVCHFLIPLIVVFFCYGRLLCAVKEAAAAQQES
ETTQRAEREVTRMVVIMVIGFLVCWLPYASVAWYIFTNQGSEFGPLFMTIPAFFAKSSSI
YNPAIYICMNKQFRNCMITTLCCGKNPFEEEEGASTTASKTEASSVSSSSVSPA

>Sardina pilchardus (Pilchard)
MNGTEGPFFYIPMSNATGLVRSPYDYPQYYLVPPWGYACLAAYMFLLILTGFPVNFLTLY
VTIEHKKLRSPLNYILLNLAVADLFMVIGGFTTTMWTSLNGYFVFGRMGCNIEGFFATLG
GEIALWSLVVLSMERWIVVCKPISNFRFGENHAVMGVAFSWFMAAACAVPPLVGWSRYIP
EGMQCSCGIDYYTRAEGFNNESFVIYMFVVHFTCPLTIITFCYGRLVCTVKEAAAQQQES
ETTQRAEREVTRMVIIMFVAFLACWVPYASVAWYIFTHQGSEFGPVFMTIPAFFAKSSAV
YNPVIYICLNKQFRHCMITTLCCGKNPFEEEEGSTTASKTEASSVCSVSPA

>Lacunicambarus ludovicianus (Painted devil crayfish)
LHMIHLHWYQYPPMNPMMYPLLLVFMLITGILCLAGNFVTIWVFMNTKSLRTPANLLVVN
LAMSDFLMMFTMFPPMMITCYYHTWTLGATFCEVYAFLGNLCGCASIWTMVFITFDRYNV
IVKGVAGEPLSTKKASLWILTVWVLSFTWCVAPFFGWNRYVPEGNLTGCGTDYLSEDILS
RSYLYIYSTWVYFLPLAITIYCYVFIIKAVAAHEKGMRDQAKKMGIKSLRNEEAQKTSAE
CRLAKIAMTTVALWFIAWTPYLLINWVGMFARSYLSPVYTIWGYVFAKANAVYNPIVYAI
S
```
{% endtab %}

{% tab title="CLUSTAL OMEGA" %}
**1.** Füge alle Aminosäuresequenzen, einschließlich der Größer-als-Symbole und den Artnamen, in das Eingabefeld [der EMBL Job Dispatcher - Seite](https://www.ebi.ac.uk/jdispatcher/) ein. (Alternativ kannst du auch [diese FASTA-Datei](https://drive.google.com/file/d/1KDqNuCz0dGR0WpanujVZ0HUd2xMJz0B2/view?usp=drive_link) mit den Sequenzen von deinem Computer hochladen).

**2.** Wähle “ClustalW with character counts” als Ausgabeformat.

**3.** Übermittle die Sequenzen zum Durchführen des Alignments.

**4.** Die verschiedenen Rhodopsin-Sequenzen sind nun in einem Alignment. Du kannst die Ergebnisse auf der Registerkarte “Alignment” einsehen und zur besseren Visualisierung auf “Show Colors” klicken.

**5.** Lade die Aminosäuresequenzen nach dem Alignment herunter oder kopiere sie für die nächste Aufgabe (einschließlich “CLUSTAL O(1.2.4) multiple sequence alignment”).

**Hinweis:** Die Ausgabe von multiplen Sequenzalignments enthält auch eine zusätzliche Zeile unterhalb der letzten Sequenz, die Auskunft darüber gibt, wie konserviert eine bestimmte Aminosäure ist. Dies ist folgendermaßen zu interpretieren:\
– Sternchen (**\***): vollständig konservierte Aminosäure (identisch in allen Sequenzen)\
– Doppelpunkt (**:**): stark konservierte Aminosäure \
– Punkt (**.**): schwach konservierte Aminosäure  \
– Leer (): nicht konservierte Aminosäure
{% endtab %}

{% tab title="FRAGEN" %}
**1.** Was kannst du aus dem Alignment ableiten? Gibt es bemerkenswerte Unterschiede in der Länge der einzelnen Sequenzen?\
**2.** Welche Art besitzt die längste Rhodopsin-Aminosäuresequenz?\
**3.** Gibt es konservierte Aminosäuren oder Teile der Sequenzen, die bei allen Arten vorhanden sind? Gibt es Teile, die nur bei einer oder wenigen Arten vorkommen?
{% endtab %}
{% endtabs %}

<details>

<summary>Antworten zu den Fragen</summary>

1. <mark style="color:green;">Aus der Ausrichtung kann man schließen, dass sich die Längen der Rhodopsin-Sequenzen der 21 ausgewählten Arten zwischen 301 und 369 Aminosäuren variieren. Die meisten Sequenzen haben eine Länge von entweder 348 oder 354 Aminosäuren und zeigen eine hohe Ähnlichkeit. Die auffälligsten Unterschiede finden sich bei den Sequenzen von Drosophila melanogaster und Lacunicambarus ludovicianus.</mark><br>
2. <mark style="color:green;">Die Rhodopsin-Sequenz von Drosophila melanogaster besitzt die längste Aminosäuresequenz mit insgesamt 369 Aminosäuren.</mark>
3. <mark style="color:green;">Es gibt konservierte Reste oder Sequenzteile, die in allen Arten vorhanden sind? Gibt es einige Teile, die nur in einer oder wenigen Arten gefunden werden?</mark>

</details>

### Teil 4: Phylogenetische Analyse

{% tabs %}
{% tab title="ÜBERSICHT" %}
Nach erfolgreichem Alignment der verschiedenen Rhodopsin-Aminosäurensequenzen werden wir nun einen phylogenetischen Baum der 21 Rhodopsine erstellen. Ein phylogenetischer Baum ist eine visuelle Darstellung, die die evolutionären Beziehungen zwischen verschiedenen Arten veranschaulicht. Dies geschieht durch die Analyse von Variationen in ihren genetischen Merkmalen, wie z. B. Unterschiede in den DNA- und Aminosäuresequenzen.

Um einen phylogenetischen Baum auf der Grundlage unseres Sequenzalignments zu erstellen, können wir die bioinformatische Methode Simple Phylogeny verwenden.
{% endtab %}

{% tab title="AUFGABE" %}
**Bitte befolge die unten aufgeführten Schritte:**

**1.** Folge den Anweisungen auf der Registerkarte “Simple Phylogeny”.

**2.** Versuche, die Fragen auf der Registerkarte “Fragen” zu beantworten.
{% endtab %}

{% tab title="SIMPLE PHYLOGENY" %}
**1.** Füge das Alignment der Aminosäuresequenzen, einschließlich “CLUSTAL O(1.2.4) multiple sequence alignment”, [in das Eingabefeld](https://www.ebi.ac.uk/jdispatcher/) ein. (Alternativ kannst du auch [diese FASTA-](https://drive.google.com/file/d/1_QwQ9w6LzBDceP2LvVcHTS9yYrUIKfiP/view?usp=drive_link)[Datei](https://drive.google.com/file/d/1_QwQ9w6LzBDceP2LvVcHTS9yYrUIKfiP/view?usp=drive_link) mit den Sequenzen von deinem Computer hochladen).

**2.** Behalte in ‘STEP 2’ die Standardeinstellungen bei.

**3.** Bestätige deine Eingaben und erstelle den phylogenetischen Baum.

**4.** Klicke auf die Registerkarte “Phylogenetic Tree”. Die Ergebnisse werden standardmäßig in Form eines “Cladograms” angezeigt. Kladogramme stellen die Verzweigungsmuster der Arten dar, geben aber keinen Aufschluss über die evolutionären Zeitunterschiede zwischen den Gruppen. Wenn du die Zweiglänge als “Real” auswählst, erhältst du Informationen über die Zeitspannen zwischen den Verzweigungspunkte.

**5.** Analysiere die phylogenetische Baumstruktur und versuche, einige der Fragen auf der Grundlage deiner Beobachtungen zu beantworten.
{% endtab %}

{% tab title="FRAGEN" %}
**1**. Untersuche die “Real” phylogenetische Baumstruktur. Beachte die beiden Sequenzen, die als Ausreißer zu sehen sind. Zu welcher Art gehören diese Rhodopsin-Sequenzen und welche Merkmale machen sie deiner Meinung nach zu Ausreißern?

**2.** Beobachte die Struktur des “Cladograms”. Der Baum teilt die Sequenzen zunächst in drei Hauptgruppen auf. Spiegelt diese Aufteilung im Allgemeinen die evolutionären Beziehungen zwischen den Arten wider? Gibt es irgendwelche Ausnahmen oder Unstimmigkeiten?
{% endtab %}
{% endtabs %}

<details>

<summary>Antworten zu den Fragen </summary>

1. <mark style="color:green;">Die zwei abweichenden Sequenzen gehören zu</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Drosophila melanogaster</mark>_ <mark style="color:green;"></mark><mark style="color:green;">und</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Lacunicambarus ludovicianus</mark>_<mark style="color:green;">. Diese Sequenzen unterscheiden sich in der Anzahl der Aminosäuren im Vergleich zu den anderen Sequenzen aufgrund zusätzlicher Einfügungen oder Deletionen.</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Lacunicambarus ludovicianus</mark>_ <mark style="color:green;"></mark><mark style="color:green;">fehlen mehrere Aminosäuren am Anfang und am Ende seiner Sequenz. In der Mitte weist es dieselbe Einfügung wie</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Drosophila melanogaster</mark>_ <mark style="color:green;"></mark><mark style="color:green;">auf, die zusätzlich weitere Aminosäureeinfügungen besitzt.</mark>
2. <mark style="color:green;">Im Großen und Ganzen reflektiert der auf den Rhodopsin-Sequenzen basierende phylogenetische Baum die evolutionären Beziehungen zwischen den Arten. Die anfängliche Teilung resultiert in einer Gruppe, die nur Arten aus der Klasse der Säugetiere (Mammalia) enthält. In dieser Gruppe werden</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Rattus norvegicus</mark>_<mark style="color:green;">,</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Mus musculus</mark>_ <mark style="color:green;"></mark><mark style="color:green;">und</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Cricetulus griseus</mark>_ <mark style="color:green;"></mark><mark style="color:green;">(alle Mitglieder der Ordnung Rodentia) zusammengefasst, und die zwei Carnivora-Arten</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Canis lupus familiaris</mark>_ <mark style="color:green;"></mark><mark style="color:green;">und</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Phoca vitulina</mark>_ <mark style="color:green;"></mark><mark style="color:green;">werden ebenfalls zusammengefasst.</mark> <mark style="color:green;"></mark>_<mark style="color:green;">Bos taurus</mark>_ <mark style="color:green;"></mark><mark style="color:green;">wird jedoch nicht mit den anderen Säugetierarten gruppiert und bildet eine separate Gruppe. Die letzte große Gruppe umfasst 14 Arten, einschließlich der neu entdeckten Arten.</mark>

</details>

### Teil 5: Strukturanalyse

{% tabs %}
{% tab title="ÜBERSICHT" %}
Herzlichen Glückwunsch zum Erreichen des letzten Teils unseres Bioinformatik-Abenteuers! Dank deiner Hilfe wissen wir jetzt, dass das Rhodopsin von einer neuen Art stammt, die eng mit _Sardina pilchardus_ verwandt ist; einem Fisch, der an der europäischen Küste lebt. Die TREC-Forscher\*innen sind von deinen Fähigkeiten sehr beeindruckt und haben eine letzte Bitte. Im Rahmen ihrer Forschung möchten sie mehr über die Struktur dieses Rhodopsins erfahren.

In diesem Teil der Aktivität werden wir die strukturellen Aspekte von Proteinen anhand einer Proteindatenbank untersuchen. Die Rhodopsinstruktur dieses neu entdeckten Rhodopsins ist noch nicht verfügbar. Wir können jedoch die Struktur des eng verwandten Rhodopsins von _Sardina pilchardus_ untersuchen, das eine sehr ähnliche Struktur aufweisen sollte. Wir werden uns auf das Rhodopsin der _Sardina_ konzentrieren und die UniProt-Datenbank nutzen, um die Sekundärstruktur dieses Proteins zu untersuchen, insbesondere dessen Alpha-Helices und Beta-Faltblätter. Darüber hinaus werden wir die dreidimensionale Struktur des Sardina-Rhodopsins mit Hilfe der in UniProt integrierten AlphaFold Datenbank untersuchen. Dies wird es uns ermöglichen, vernünftige Schlussfolgerungen über die Struktur des neuen Rhodopsins zu treffen.
{% endtab %}

{% tab title="AUFGABE" %}
**Bitte befolge die unten aufgeführten Schritte:**

**1.** Suche nach dem _Sardina_ Rhodopsin in der UniProt-Datenbank, um die Sekundärstruktur des Proteins zu finden.

**2**. Untersuche die dreidimensionale Struktur des _Sardina_ Rhodopsins, die von AlphaFold erstellt und in der UniProt-Datenbank angezeigt wird.

**3.** Versuche, die Fragen auf der Registerkarte “Fragen” zu beantworten.
{% endtab %}

{% tab title="UniProt und AlphaFold" %}
**1.** Greife auf die [UniProt-Datenbank](https://www.uniprot.org/)  zu.

**2.** Suchen nach dem _Sardina_ Rhodopsin mit Hilfe des UniProt-Namens (OPSD\_SARPI) oder der Hinterlegungsnummer (Q9YGZ0).

**3.** Auf der Ergebnisseite findest du eine Zusammenfassung aller wissenschaftlichen Informationen, die über das _Sardina_ Rhodopsin verfügbar sind. Untersuche die in der UniProt-Datenbank bereitgestellten Informationen und versuche, einige der Fragen zu beantworten. &#x20;

**4.** Scrolle im Fenster der UniProt-Datenbank nach unten zu “Struktur”. Wenn die Struktur nicht angezeigt wird, klicke auf “Click on load the structure viewer”. Du siehst nun eine dreidimensionale Struktur des _Sardina_ Rhodopsins, auch bekannt als Protein-Tertiärstruktur, die von AlphaFold erstellt wurde. Du kannst deinen Mauszeiger benutzen, um die Struktur zu drehen. Außerdem kannst du auf einzelne Aminosäuren innerhalb der Struktur klicken, um weitere Informationen zu erhalten.

**5.** Schaue dir die dreidimensionale Struktur an und versuche, einige der Fragen zu beantworten.
{% endtab %}

{% tab title="FRAGEN" %}
Kannst du auf der Grundlage der Informationen aus der UniProt-Datenbank die folgenden Fragen beantworten?

1. Wie viele Transmembrandomänen hat das Rhodopsin der _Sardina pilchardus_ und wie sind sie über das Protein verteilt? Diese Informationen finden Sie im Abschnitt “Subcellular Location”.
2. Kannst du ausgehend von der vorhergehenden Antwort auf die größere Gruppe der evolutionär verwandten Proteine schließen, zu der unser Rhodopsin gehört?
3. Was sind Beispiele für posttranslationale Modifikationen (PTM) des Rhodopsins von _Sardina pilchardus_? Diese Informationen findest du im Abschnitt “PTM/Processing”.

Kannst du auf der Grundlage der von AlphaFold vorhergesagten dreidimensionalen Struktur einige der folgenden Fragen beantworten?

1. Welche Form hat das Rhodopsin von _Sardina pilchardus_ im Allgemeinen?
2. Versuche, die einzelnen Alpha-Helices und Beta-Faltblätter in der Struktur zu identifizieren. Die Beta-Faltblätter sind wichtig für die Bindung von Retinal. Wo genau befinden sich diese beiden Beta-Faltblätter?
{% endtab %}

{% tab title="ZUSAMMENFASSUNG" %}
Dank deiner Hilfe konnte das TREC-Team die Funktion und die evolutionären Ursprünge des unbekannten Proteins ermitteln. Außerdem deuten deine Ergebnisse darauf hin, dass dieses Rhodopsin zu einer neuen Art gehören könnte, die eng mit _Sardina pilchardus_ verwandt ist und an der europäischen Küste lebt.

Es sind einige Monate vergangen, seit du dem TREC-Team geholfen hast, und jetzt hat das Team dir überraschenderweise eine weitere E-Mail geschickt! Darin erklären dir die Forscher\*innen, dass sie ihre Forschung an diesem neuen Rhodopsin fortgesetzt haben und mit Hilfe des Imaging Centre am EMBL die Proteinstruktur des Rhodopsins dieser neuen Art identifizieren konnten. Dabei verwendeten sie eine Methode namens Kryoelektronenmikroskopie (Kryo-EM) und möchten, dass du der erste bist, der die Rhodopsinstruktur sieht. Hier ist sie:

{% embed url="https://www.embl.org/ells/wp-content/uploads/2023/07/Rhodopsin-Movie.mp4" %}
{% endtab %}
{% endtabs %}

<details>

<summary>Antworten zu den Fragen</summary>

1. Das Rhodopsin der Sardina pilchardus hat 7 Transmembrandomänen, die regelmäßig über das Protein verteilt sind. Diese Domänen sind durch topologische Domänen getrennt, die zwischen extrazellulären und zytoplasmatischen Regionen wechseln.&#x20;
2. Aufgrund des Vorhandenseins von 7 Transmembrandomänen können wir davon ausgehen, dass Rhodopsin zur Gruppe der 7-Transmembrandomänen-Rezeptoren gehört, die auch als G-Protein-gekoppelte Rezeptoren (GPCRs) bezeichnet werden.&#x20;
3. Zu den üblichen posttranslationalen Modifikationen (PTM) des Sardina pilchardus-Rhodopsins gehören Glykosylierung, Lipidierung und die Bildung von Disulfidbindungen.
4. Die Struktur des Rhodopsins von Sardina pilchardus ähnelt einer Röhre oder einem Fass. Die Struktur des Rhodopsins von Sardina pilchardus zeigt deutlich das Vorhandensein von sieben transmembranen Alpha-Helices, die zusammen die tonnenförmige Struktur bilden.&#x20;
5. Die beiden Beta-Folien befinden sich am oberen Ende der tonnenförmigen Struktur und sind auf beiden Seiten mit zwei Alpha-Helices verbunden.

</details>
