To tylko takie drobne uwagi, załozenia i instrukcje ;D


Ten projekt miał na celu wykonanie programu umożliwiającego pisanie/grawerowanie/wycinanie
na wybranym elemencie w zależności od wybranego narzędzia. W moim przypadku są to płyty o wymiarach 1400x800x40. Program został
napisany tak, aby była szybka możliwość zmiany parametrów np. prędkości pisania lub też ruchu
między kolejnymi literami. 

Zdaje sobie sprawę, że pewne rzeczy można było by zrobić inaczej, być może szybciej i lepiej,
ale miałem za mało czasu, żeby zagłębiać się we wszystkich dostępnych funkcjach.




Informacje odnośnie pliku config.txt:

*Aby program mogł prawidłowo działać należy zmienić 4 linijke kodu (ścieżke dostępu do pliku konfiguracyjnego
 w konrolerze M_Gieraa, tak aby wskazywała ona plik config.txt

-nieparzyste linijki musza mieć wpisane wymiary elementu po którym chcemy pisać w formacie np. 1400x800
- możliwa jest zmiana wielkości elementu, tylko w pewnych granicach, tak aby robot mógł wszędzie dosięgnąć
- zmiana wielkości elementu wpłynie na ilość liter, które można zapisać a także długość tekstu w kazdej linijce
  adekwatnie do rozmiaru elementu, który chcemy np. grawerować
- parzyste linijki dotyczą tekstu jaki chcemy, żeby robot dla nas napisał
- nalezy pamiętać o tym, że gdy napis się nie zmieści w jednej linijce to automatycznie zostanie podzielony (można
  odpowiednio manipulować spacjami, żeby wykonać napis tak jak chcemy.
- każda para linijek (wymiary elementów i tekst) odpowiada za każdą nową płyte. Na palecie maksymalnie mieści się 24 płyty,
  ale nic nie stoi na przeszkodzie, aby 



Pomysły, które można wdrożyć:
- dodanie wiecej liter, liczb, znaków specjalnych
- zmiana odczytywania z pliku tak, aby w przyopadku gdy będzie jakiś znak np. '|' na końcu wyrazu to program automatycznie przejdzie
  do nowej lini, bez konieczności robienia spacji.
- zapytanie do operatora czy ma byc jeden napis na wszystkich plytach i wtedy zczytuje tylko ta pierwsza i ewentualnie pyta ile plyt takich wykonac