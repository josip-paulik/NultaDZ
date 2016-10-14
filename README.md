# 0036492647

#1.
Dodani su ClassLibrary1.dll i ClassLibrary1.pdb. Javlja UnhandledException zato što nije nađen ClassLibrary1.dll u istoj datoteci kao i izvršna datoteka(KonzolnaAplikacija.exe). Kad bih Vam slao aplikaciju, poslao bih ClassLibrary.dll i KonzolnaAplikacija.exe.
#2.
Kada se pokrene KonzolnaAplikacija.exe onda se koristi stari string, zato što nismo "dodali nove informacije" u ClassLibrary1.dll odnosno sve dok se ne prevede source kod(Class1.cs), neće se promijeniti ClassLibrary1.dll(odakle konzolna aplikacija vadi podatke o metodi PrintHelloWorld).
#3
Pero: Hello World
#4
Sadržaj datoteke se nije promijenio.
#5
PeroClassLibrary.dll se stvorio u bin/debug direkotoriju, gdje je Visual Studio počeo tražiti nakon brisanja, zato se može buildati i pokrenuti.
#6
Prva linija u Output prozoru prikazuje liniju "Restoring NuGet packages...".  Packages direktorij se vratio u izvornom stanju

