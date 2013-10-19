### Labolatorium 1

1\. Używając linii poleceń stwórz strukturę katalogów:

'''sh

 mkdir -p dom nauka/{c,logo,pascal} praca/{dokumenty,zlecenia/{niezrealizowane,zrealizowane}}

2\. Przejdź do katalogu dom i utwórz katalog wazne-sprawy.

'''sh

cd dom

touch wazne-sprawy

3\. Wejdź do katalogu wazne-sprawy i utwórz tam pusty plik rachunki.txt.

'''sh

temp/dom/wazne-sprawy$ touch rachunki.txt

4\. Będąc w katalogu wazne-sprawy skopiuj plik rachunki.txt do katalogu zrealizowane.

'''sh

cp ./rachunki.txt ~/temp/praca/zlecenia/zrealizowane

5\. Przejdź do katalogu zrealizowane i zmień nazwę pliku rachunki.txt na wykonano.txt.

'''sh

cd ../../
cd praca/zlecenia/zrealizowane
mv rachunki.txt wykonano.txt

6\. Utwórz plik wykonano.txt wielkości 11 bajtów, następnie podziel go pliki wielkości 5 bajtów. W ten sposób otrzymasz 3 pliki. (split)

'''sh

cat > wykonano.txt

1234567890

split -b5 wykonano.txt

7\. Będąc w katalogu logo skopiuj powyżej otrzymane 3 pliki do katalogu dokumenty.

'''sh

cd ../../..

cd nauka/logo

cp ~temp/praca/zlecenia/zrealizowane/{xaa,xab,xac} ~/temp/praca/dokumenty/

8\. Będąc w katalogu dokumenty połącz skopiowane 3 pliki w plik odtworzono.txt, tak aby otrzymać plik o zawartości identycznej z wykonano.txt. Następnie plik odtworzono.txt skopiuj do katalogu wazne-sprawy.

'''sh







