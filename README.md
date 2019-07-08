# ml06-recommender-systems
Andrijana Marjanović

Repozitorijum sadrzi razlicite pristupe implementaciji sistema za preporuku filmova. 

Prikazane preporuke filmova iz baze podataka (http://files.grouplens.org/datasets/movielens/ml-latest-small-README.html) dobijaju se na osnovu razlicitih ideja kao sto su najpopularniji filmovi u pogledu broja dobijenih ocjena ili na osnovu najvise prosjecne ocjene, uopstene preporuke koje se daju svim korisnicima, slicnost po sadrzaju (Content-based), kao i kolaborativno filtriranje (Collaborative Filtering). U slucaju metoda preporucivanja na osnovu sadrzaja, ne uzima se u obzir interesovanje korisnika, ni njegova povezanost sa drugim korisnicima, za razliku od CF. U tome se ogleda prednost CF pristupa.

U slucaju CF pristupa, filmovi se preporucuju pronalazenjem slicnosti izmedju filmova koje je korisnik ocjenio, kao i 
slicnosti izmedju korisnika koji su ocjenili iste filmove.
Definisana je funkcija za podjelu skupa podataka na skup za obucavanje i skup za validaciju, pomocu kojih je data ocjena Root Mean Square Error i Mean Absolute Error.

Za predvidjanje najvisih ocjena na osnovu kojih se preporucuju razliciti filmovi razlicitim korisnicima, koristena je i SVD dekompozicija.

Za implementaciju metoda latentnih faktora za CF koristen je Stohasticki gradijentni spust.
