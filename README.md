# Bibliographischer Datenbankvergleich


Software und Daten zum Vergleich der bibliographischen Datenbanken Scopus und [OpenAlex](https://openalex.org/) für das Forschungsgebiet der [Atomlagenabscheidung (ALD)](https://de.wikipedia.org/wiki/Atomlagenabscheidung).


Die enthaltenen Jupyter-Notebooks wurden verwendet, um ein Sample aus den bibliographischen Datenbanken Scopus und OpenAlex zu erstellen, die Daten zu bereinigen, das Matching der Daten durchzuführen und die anschließende Datenvisualisierung zu erstellen. 

Es wurde Python 3.11.2 genutzt. Weitere Software-Spezifikationen sind in `requirements.txt` definiert.

Die Datenabfrage über die Scopus-API erfolgt mit der Python-Bibliothek [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/index.html).  
Die Datenabfrage über die OpenAlex-API erfolgt mit der Python-Bibliothek [pyalex](https://github.com/J535D165/pyalex).



## Inhalt

* `01_Exploration_Daten_Scopus_ALD.ipynb`: Jupyter-Notebook zur Exploration der Scopus-Daten 
* `02_Datenabfrage_Scopus_ALD.ipynb`: Jupyter-Notebook zur Datenabfrage in Scopus
* `03_Datenabfrage_OpenAlex_ALD.ipynb`: Jupyter-Notebook zur Datenabfrage in OpenAlex
* `04_Datenbereinigung.ipynb`: Jupyter-Notebook zur Datenbereinigung der Daten aus Scopus und OpenAlex
* `05_Matching_Scopus_OpenAlex.ipynb`: Jupyter-Notebook zum Matching der Daten aus Scopus und OpenAlex
* `06_Matching_Score.ipynb`: Jupyter-Notebook zur Exploration und Entwicklung des genutzten Scores zum Matching
* `07_Datenanalyse.ipynb`: Jupyter-Notebook zur Analyse und Visualisierung der Daten
* `/data`: Daten aus den bibliographischen Datenbanken Scopus und OpenAlex. Details enthält die `README.md` in diesem Ordner.
  * `/raw`: CSV-Dateien der abgerufenen Rohdaten
  * `/proccesed`: CSV-Dateien für die bereinigten Daten
  * `/diff`: CSV-Dateien mit den finalen Ergebnissen aus dem Matching von Scopus und OpenAlex 
* `/figures`: PNG-Dateien der erzeugten Datenvisualisierungen


## Lizenz

Der Quellcode ist gemäß GPL v3 lizenziert (siehe LICENSE).  
Die Daten in `/data` sind unter [CCO](https://creativecommons.org/public-domain/cc0/) lizenziert.
