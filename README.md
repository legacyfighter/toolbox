# Skrzynka narzędziowa

Repozytorium dodatków do skrzynki narzędziowej LF. Znajdują się tu:

* [użyteczne one linery](#użyteczne-one-linery)
* [książki](#książki)
* [narzędzia](#narzędzia)


### Użyteczne one-linery
________________________

Uwaga! Korzystanie z poniższych skryptów może wymagać dopasowania do twojej technologii lub systemu operacyjnego...

##### Lista 10 najczęściej zmieniających się plików w repozytorium
```bash
git log --pretty=format: --name-only | sort | uniq -c | sort -rg | head -10
```

##### Korona Himalajów, 14 najdłuższych plików w projekcie
```bash
find . -name '*.java' -not -path "*/target/*" | xargs wc -l | sort -nr | head -n14
```

##### Lista wszystkich plików w projekcie, które mają więcej niż 500 linii
```bash
find . -name '*.java' -not -path "*/target/*" | xargs wc -l | sort -nr | awk '$1 > 500'
```

### Książki
___________

- [📕 Refactoring: Improving the Design of Existing Code - Martin Fowler, Kent Beck](https://www.goodreads.com/book/show/44936.Refactoring)
- [📕 Working Effectively with Legacy Code - Michael C. Feathers](https://www.goodreads.com/book/show/44919.Working_Effectively_with_Legacy_Code)

*linki powinny prowadzić do Goodreads*

### Narzędzia
_____________

To be introduced...