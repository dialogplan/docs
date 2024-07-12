# [docs.dialogplan.com](http://docs.dialogplan.com)


"Plan" najlepiej oddaje ideę scenariusza wykonania projektu. Sugeruje strukturę, organizację i przewidywanie przyszłych działań.
Słowo "plan" kojarzy się z harmonogramem, co dobrze pasuje do określania czasu wykonania poszczególnych etapów.
"Plan" implikuje również ustalanie priorytetów i sekwencji działań, co odpowiada określaniu priorytetów i zależności między etapami.
"Dialog" w tym kontekście może sugerować interaktywność lub możliwość dostosowania planu, co jest przydatne w zarządzaniu projektami.
"Dialogplan" brzmi profesjonalnie i jest łatwe do zapamiętania, co jest ważne z marketingowego punktu widzenia.



## Dlaczego powstał ten projekt?

Terminologia związana ze zmianą statusu projektu może różnić się w zależności od organizacji i branży - różne firmy i zespoły mogą mieć własne, unikalne nazewnictwo dla tych etapów.

Fachowa nazwa oznaczająca zmianę statusu projektu zależy od kontekstu i może być różna w zależności od branży i metodyki zarządzania projektami. 
Niektóre z ogólnych terminów, które mogą być używane do opisania zmiany statusu projektu, to:

1. **Faza (Phase)** - Etap projektu, często stosowany termin w cyklu życia projektu, w którym przechodzi on przez różne etapy, od koncepcji do zakończenia. Każda faza to odrębny etap prac.

2. **Milestone (Kamień milowy)** - Znaczący punkt w projekcie, często wiążący się z ważnym osiągnięciem lub etapem gwarantującym przejście do następnego etapu prac.

3. **Etap (Stage)** - Podobnie jak faza, etap to określenie segmentu projektu, który charakteryzuje się określonym zestawem prac lub celem do osiągnięcia.

4. **Update statusu (Status update)** - Aktualizacja lub zmiana stanu projektu, gdy przechodzi on z jednego stanu do drugiego.

5. **Progression (Postęp)** - Termin opisujący proces przemieszczania się projektu do przodu w jego cyklu życia.

6. **Transition (Przejście)** - Konkretne przejście projektu z jednej fazy/części prac do kolejnej.

W metodykach zarządzania projektami, takich jak Agile, mogą być również używane specyficzne terminy, takie jak „Sprint Review” w Scrum, który oznacza przegląd prac wykonanych w danym sprincie, lub „Iteration” w innych metodykach Agile wskazujące na cykliczny okres rozwoju produktu.


## Jakie cele realizuje?

pozwala na generowanie zestawienia wielu projektów do strageii w postaci:
+ dokumentacji w tabeli
+ obrazu grafu
+ formatu mermaid

Dla celów monitorowania postępu w projekcie poprzez 

+ **Faza (Phase)**

+ **Milestone (Kamień milowy)**

+ **Etap (Stage)** SDLC


## Jak to działa

Skrypt PHP generuje odpowiedź na zapytanie dynamicznie w formacie:

schema API:
```
http://dialogplan.com/{provider}/{org}/{repo}/{format}
```

schema GET:
```
http://dialogplan.com/?in={yaml|json}&out={md|csv|html}&url={gitlab|github}
```

example

```
http://dialogplan.com/?in="yaml"&out="md"&url="https://github.com/dialogplan/docs/"
```

Do wygenerowania wielu na raz potrzebny jest request typu POST

```
http://dialogplan.com/?format="yaml"&out="md"&url[0]="https://github.com/dialogplan/docs/"&url[1]="https://github.com/dialogplan/docs/"&url[3]="https://github.com/dialogplan/docs/"
```


## Schema

+ apiMacro - Hi level operation
+ apiUnit - Organization
+ apiDSL - OPS
+ apiTee - SDLC, deployment




## Funkcje

Zbudowanie struktury na bazie text -> yaml
zapisanie per user
share do konkretnych userów na tej platformie
można stworzyć dedykowane url

+ Edycja plików yaml zdalnie na organizachach, serwerze przez API github / gitlab


