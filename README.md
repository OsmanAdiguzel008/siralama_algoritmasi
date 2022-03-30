# siralama_algoritmasi
Siralama, artan veya azalan olacak sekilde duzenlenebiliyor.
Python liste uzerinde yapilan siralama .sort()fonksiyonu ile kiyaslandi. Sonuclar asagidaki gibidir:

%%timeit
yeni_liste = siralama(liste,False)
# 297 ns ± 13.1 ns per loop (mean ± std. dev. of 7 runs, 1000000 loops each)   1000 value
# 743 ns ± 759 ns per loop (mean ± std. dev. of 7 runs, 1 loop each)           10000 value
# 714 ns ± 569 ns per loop (mean ± std. dev. of 7 runs, 1 loop each)           100000 value

%%timeit
liste.sort()
# 4.74 µs ± 251 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)    1000 value
# 43 µs ± 761 ns per loop (mean ± std. dev. of 7 runs, 10000 loops each)       10000 value
# 419 µs ± 6.36 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)      100000 value
