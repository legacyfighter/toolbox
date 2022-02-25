# Skrzynka narzędziowa

Repozytorium dodatków do skrzynki narzędziowej LF. Znajdują się tu:

* [użyteczne one linery](#użyteczne-one-linery)
* [książki](#książki)
* [artykuły](#artykuły)
* [blogi](#blogi)
* [narzędzia](#narzędzia)
* [skróty](#skróty)


### Użyteczne one-linery
________________________

Uwaga! Korzystanie z poniższych skryptów może wymagać dopasowania do twojej technologii lub systemu operacyjnego...

##### Lista 10 najczęściej zmieniających się plików w repozytorium
```bash
git log --pretty=format: --name-only | sort | uniq -c | sort -rg | head -10
```

##### Korona Himalajów, 14 najdłuższych plików w projekcie
```bash
find . -name '*.java' -not -path "*/target/*" -not -path "*/build/*" | xargs wc -l | sort -nr | head -n14
```

##### Lista wszystkich plików w projekcie, które mają więcej niż 500 linii
```bash
find . -name '*.java' -not -path "*/target/*" -not -path "*/build/*" | xargs wc -l | sort -nr | awk '$1 > 500'
```

##### Liczba commitów w zadanym okresie z pominięciem merge commitów
```bash
git rev-list --count --since="Jan 31 2022"  --before="Feb 5 2022" --all --no-merges
```

### Książki
___________

- [📕 Refactoring: Improving the Design of Existing Code - Martin Fowler, Kent Beck](https://www.goodreads.com/book/show/44936.Refactoring)
- [📕 Working Effectively with Legacy Code - Michael C. Feathers](https://www.goodreads.com/book/show/44919.Working_Effectively_with_Legacy_Code)
- [📕 Your Code as a Crime Scene: Use Forensic Techniques to Arrest Defects ... - Adam Tornhill](https://www.goodreads.com/book/show/23627482-your-code-as-a-crime-scene)
- [📕 Software Design X-Rays: Fix Technical Debt with Behavioral Code Analysis - Adam Tornhill](https://www.goodreads.com/book/show/36517037-software-design-x-rays)
- [📕 The Mikado Method - Ola Ellnestam, Daniel Brolund](https://www.goodreads.com/book/show/17974534-the-mikado-method)
- [📕 xUnit Test Patterns: Refactoring Test Code - Gerard Meszaros](https://www.goodreads.com/book/show/337302.xUnit_Test_Patterns)
- [📕 Refactoring Databases: Evolutionary Database Design - Scott W. Ambler, Pramod J. Sadalage](https://www.goodreads.com/book/show/161302.Refactoring_Databases)
- [📕 Practical Guide to Large Database Migration - Preston Zhang](https://www.goodreads.com/book/show/42818341-practical-guide-to-large-database-migration)
- [📕 Practical Data Migration- Johny Morris](https://www.goodreads.com/book/show/16654923-practical-data-migration)

*linki powinny prowadzić do Goodreads*

### Artykuły
____________

- [Working Effectively With Legacy Code - Michael C. Feathers](https://debug.to/pdf/Michael%20Feathers%20-%20Working%20Effectively%20With%20Legacy%20Code.pdf)

### Blogi
_________

- [Understand Legacy Code](https://understandlegacycode.com/)

### Narzędzia
_____________

- [🛠 Code Maat - a command line tool used to mine and analyze data from version-control systems (VCS)](https://github.com/adamtornhill/code-maat#running-code-maat)

### Skróty

##### Wyświetlenie drzewa hierarchii wywołania

Idea: https://www.jetbrains.com/help/idea/viewing-structure-and-hierarchy-of-the-source-code.html

