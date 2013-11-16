###Laboratorium 4

1\. Wyświetl listę plików z aktualnego katalogu, zamieniając wszystkie małe litery na duże.

```sh

ls | tr 'a-z' 'A-Z'

```

2\. Wyświetl listę praw dostępu do plików w aktualnym katalogu, ich rozmiar i nazwę.

```sh

 ls -l | tr -s " " | cut -f 1,5,9 -d " " |tr " " "\t"


```

3\. Wyświetl listę plików w aktualnym katalogu, posortowaną według rozmiaru pliku.

```sh

ls -S

```

4\.Wyświetl zawartość pliku /etc/passwd posortowaną według numerów UID w kolejności od największego do najmniejszego.

```sh

sort -n -k 3 -t : /etc/passwd | less

```

5\. Wyświetl zawartość pliku /etc/passwd posortowaną najpierw według numerów GID w kolejności od największego 
do najmniejszego, a następnie UID

```sh 

sort -n -k 3 -t : /etc/passwd | sort -ns -k 4 -t : | more

```


6\. Podaj liczbę plików każdego użytkownika.

```sh

find $HOME -not -type d| wc -l


```

7\. Sporządź statystykę praw dostępu (dla każdego z praw dostępu podaj ile razy zostało ono przydzielone).

```sh

ls -l | cut -f 1 -d " " | sort | uniq -c

```
