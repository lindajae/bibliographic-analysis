# Daten

## /raw

Die abgefragten Rohdaten. Es wurden jeweils zwei Zeiträume betrachet (2010 - 2013 und 2020 - 2023). 


### Scopus

Die Daten aus Scopus unterliegen Lizenzbedingungen die eine Weitergabe nicht erlauben. Es ist daher nur die ID aus Scopus gespeichert.
Für das Ausführen des Juypter-Notebooks ist eine Lizenz für Scopus sowie ein API-Key notwendig.

* `data_scopus_2010_pub.csv`
Rohaten aus Scopus für die Suchabfrage zur Atomlagenabscheidung für den Zeitraum 2010 - 2013. Datenabfrage erfolgt mit `02_Datenabfrage_Scopus_ALD.ipynb`
* `data_scopus_2020_pub.csv`
Rohdaten aus Scopus für die Suchabfrage zur Atomlagenabscheidung für den Zeitraum 2020 - 2023. Datenabfrage erfolgt mit `02_Datenabfrage_Scopus_ALD.ipynb`


### OpenAlex

* `data_openalex_2010.csv`
Rohdaten aus OpenAlex für die Suchabfrage zur Atomlagenabscheidung für den Zeitraum 2010 - 2013. Datenabfrage erfolgt mit `03_Datenabfrage_OpenAlex_ALD.ipynb`
* `data_openalex_2020.csv`
Rohdaten aus OpenAlex für die Suchabfrage zur Atomlagenabscheidung für den Zeitraum 2020 - 2023. Datenabfrage erfolgt mit `03_Datenabfrage_OpenAlex_ALD.ipynb`



## /processed

Enthält die bereinigten Daten. Die Bereinigung erfolgt mit `04_Datenbereinigung.ipynb` und beinhaltet vorallem das Entfernen von Duplikation und die Bereinigung 
des Dokumententitels zur Vorbereitung des Matchings.

* `data_openalex_2010_cleaned.csv`
Bereinigte Daten aus OpenAlex für den Zeitraum 2010 - 2013. 
* `data_openalex_2020_cleaned.csv`
Bereinigte Daten aus OpenAlex für den Zeitraum 2020 - 2023. 

* `data_scopus_2010_cleaned_pub.csv`
Bereinigte Daten aus Scopus für den Zeitraum 2010 - 2013. Es ist nur die Scopus ID enthalten.
* `data_scopus_2020_cleaned_pub.csv`
Bereinigte Daten aus Scopus für den Zeitraum 2020 - 2023. Es ist nur die Scopus ID enthalten.


## /diff

Dieser Ordner enthält die Ergebnisse des Datenabgleichs. Das Matching erfolgt in `05_Matching_Scopus_OpenAlex.ipynb`

* `data_2010_matching_results.csv`
Ergebnis des Datenbankvergleichs für den Zeitraum 2010 - 2013. Es ist nur die DOI, Scopus ID und OpenAlex ID enthalten (sofern vorhanden).
* `data_2020_matching_results.csv`
Ergebnis des Datenbankvergleichs für den Zeitraum 2020 - 2023. Es ist nur die DOI, Scopus ID und OpenAlex ID enthalten (sofern vorhanden).


Im Rahmen der Datenanalyse in `07_Datenanalyse.ipynb` wurden für alle nicht gematchten Datensätze mit DOI eine zweite Abfrage in Scopus bzw. OpenAlex durchgeführt. 
Diese Daten sind auch in diesem Ordner enthalten. Für die Abfragen in Scopus ist eine Lizenz erfolderlich. 


* `data_2010_only_openalex_final.csv`
Finaler Datensatz der nach der zweiten Abfrage (via DOI in Scopus) nur in OpenAlex enthaltenen Daten für den Zeitraum 2010 - 2013. 
* `data_2020_only_openalex_final.csv`
Finaler Datensatz der nach der zweiten Abfrage (via DOI in Scopus) nur in OpenAlex enthaltenen Daten für den Zeitraum 2020 - 2023. 

* `data_2010_only_scopus_final_pub.csv`
Finaler Datensatz der nach der zweiten Abfrage (via DOI in OpenAlex) nur in Scopus enthaltenen Daten für den Zeitraum 2010 - 2013. 
Es ist nur die Scopus ID enthalten.
* `data_2020_only_scopus_final_pub.csv`
Finaler Datensatz der nach der zweiten Abfrage (via DOI in OpenAlex) nur in Scopus enthaltenen Daten für den Zeitraum 2020 - 2023. 
Es ist nur die Scopus ID enthalten.
