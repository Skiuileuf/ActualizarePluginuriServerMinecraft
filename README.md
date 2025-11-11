# Proiect RPA 2025
Master Informatica de Gestiune, Facultatea de Contabilitate si Informatica de Gestiune, Academia de Studii Economice din Bucuresti

Viziteu Mihai

UIPath Studio 2023.10.4

### Descriere program
Program care primeste un excel cu linkuri pentru pluginuri pentru un server de minecraft si o versiune tinta si descarca pluginurile pentru versiunea selectata (daca exista) sau genereaza un excel cu pluginurile pentru care nu a fost gasita o versiune

Cum functioneaza?
Are un fisier "plugins.xlsx", unde fiecare sheet reprezinta un set de pluginuri pentru un server.
Daca exista mai multe sheet-uri, utilizatorul trebuie sa selecteze una dintre configuratii. 
Sunt descarcate si deserializate date dintr-un JSON, reprezentand toate versiunile de minecraft stabile (type = "release").
Doar pluginuri pentru Spigot/PaperMC vor fi luate in vedere. Nu intentionez sa implementez alte "plugin loaders"

Fiecare sheet contine date de forma (Nume,Link,Tip) ⚠️⚠️[WORK IN PROGRESS]⚠️⚠️
Tip reprezinta tipul site-ului de unde va fi descarcat pluginul. Probabil poate sa fie calculat in functie de link, dar exista si exceptii. 

Exemple de tipuri de pluginuri (practic tip = sursa):
Generice (mai multe pluginuri pot fi descarcate de pe acelasi site)
- Spigot
- Modrinth
- Hangar
Speciale
- Squaremap_Addons (necesita download de pe github)
- Luckperms (au site-ul lor)
