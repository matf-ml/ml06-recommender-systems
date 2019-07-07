# ml06-recommender-systems
Andrijana Marjanović

Repozitorijum sadrzi razlicite pristupe implementaciji sistema za preporuku filmova. Prikazane preporuke filmova iz baze podataka 
(http://files.grouplens.org/datasets/movielens/ml-latest-small-README.html) baziraju se na razlicitim idejama kao sto su najpopularniji 
filmovi u pogledu broja dobijenih ocjena ili najvise prosjecne ocjene, uopstene preporuke koje se daju svim korisnicima, slicnost po 
sadrzaju, kao i kolaborativno filtriranje. U slucaju metoda preporucivanja na osnovu sadrzaja, ne uzima se u obzir interesovanje korisnika, 
kao ni njegova povezanost sa drugim korisnicima, za razliku od kolaborativnog filtriranja.

U slucaju kolaborativnog filtriranja filmovi se preporucuje pronalazenjem slicnosti izmedju filmova koje je korisnik ocjenio, kao i 
slicnosti izmedju korisnika koji su ocjenili iste filmove.
Definisana je funkcija za podjelu skupa podataka na skup za obucavanje i validaciju, pomocu kojih je data ocjena Root Mean Square Error
i Mean Absolute Error.

Za predvidjanje najvisih ocjena na osnovu kojih se preporucuju razliciti filmovi razlicitim korisnicima, koristena je SVD dekompozicija.

Za implementaciju metoda latentnih faktora za CF koristen je Stohasticki gradijentni spust.
