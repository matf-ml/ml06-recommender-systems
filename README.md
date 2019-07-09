# ml06-recommender-systems
Andrijana Marjanović

Repozitorijum za projekat na kursku Mašinsko učenje sadrži različite pristupe implementaciji sistema za preporuku filmova. 

Prikazane preporuke filmova iz baze podataka (http://files.grouplens.org/datasets/movielens/ml-latest-small-README.html) dobijaju se na osnovu različitih ideja kao sto su najpopularniji filmovi u pogledu broja dobijenih ocjena ili na osnovu najviše prosječne ocjene, zatim uopštene preporuke koje se daju svim korisnicima, kao i sličnost po sadržaju (Content-based Filtering) i kolaborativno filtriranje (Collaborative Filtering). U slučaju metoda preporučivanja na osnovu sadržaja, ne uzima se u obzir interesovanje korisnika, ni njegova povezanost sa drugim korisnicima, za razliku od CF u čemu se i ogleda prednost CF pristupa.

U slučaju CF pristupa, filmovi se preporučuju pronalaženjem sličnosti između filmova koje je korisnik ocjenio, kao i 
sličnosti između korisnika koji su ocjenili iste filmove.
Definisana je funkcija za podjelu skupa podataka koji sadrži relaciju korisnik-film u smislu ocjene, na skup za obučavanje i skup za validaciju, pomoću kojih je data ocjena Root Mean Square Error i Mean Absolute Error.

Za predviđanje kojim filmovima bi korisnik dao najviše ocjene i na osnovu toga bi ti filmovi bili preporučeni korisniku, korištena je i SVD dekompozicija.

Za implementaciju metoda latentnih faktora za CF korišten je Stohastički gradijentni spust.
