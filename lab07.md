###Laboratorium 7


1\.W bieżącym katalogu zamienić rozszerzenia wszystkich plików z rozszerzeniem htm na html. Jeżeli w nazwie pliku istnieje spacja, to należy zamienić ją na znak podkreślenia.

```sh

#!/bin/bash

     for plik1 in *.htm
     do
       plik2=`echo "$plik1"l | tr " " "_"`
       mv "$plik1"  "$plik2"

     done
     exit 0
     
```


2\. Napisać skrypt zawierający funkcję obliczającą silnię. Następnie należy obliczyć silnię z liczby, która jest argumentem skryptu. W przypadku niepoprawnego argumentu należy wypisać odpowiedni komunikat.

```sh


```
