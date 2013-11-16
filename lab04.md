###Laboratorium 4

1\. Wyświetl listę plików z aktualnego katalogu, zamieniając wszystkie małe litery na duże.

```sh

ls | tr 'a-z' 'A-Z'

```

2\. Wyświetl listę praw dostępu do plików w aktualnym katalogu, ich rozmiar i nazwę.

```sh

ls -lk

```

3\. Wyświetl listę plików w aktualnym katalogu, posortowaną według rozmiaru pliku.

```sh

ls -S

```

4\.Wyświetl zawartość pliku /etc/passwd posortowaną według numerów UID w kolejności od największego do najmniejszego.

```sh

sort -t : -n -k3 -r /etc/passwd

```

5\. Wyświetl zawartość pliku /etc/passwd posortowaną najpierw według numerów GID w kolejności od największego 
do najmniejszego, a następnie UID

```sh 

sort -t : -k4 -r /etc/passwd | sort -t : -k3 

```


