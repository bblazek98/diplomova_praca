# Odkaz na stiahnutie hry a popis spustenia

## Stiahnutie hry
Hra doposiaľ nebola poblikovaná pre verejnosť


## Spustenie
Spúštanie je prevedené v dvoch krokoch
1. Spustenie priloženého programu "main.py"
2. Spustenie hry samotnej

### Spustenie 
Pre spustenie priloženého programu je potrebné mať nainštalovaný python s verziou 3.9 alebo vyššou. Pre správne fungovanie je potrebné nainštalovať knižnice pmocou príkazu uvedeného nižšie, na čo je využítý manažér Python balíčkov PIP.
```
pip install websockets asyncio termcolor
```
Balíček threading nie je potrebné inštalovať, keďže od verzie Python 3.7 patrí medzi základné. Pre spustenie bota je volaný príkaz:
```
python -u [cesta]
```
V tomto príkaze je potrebne vloženie cesty k lokácii súboru main.py priloženého k projektu.
Pri správnom spustení by mal program v konzole vypísať nasledujúci riadok a čakať na spustenie inštancie hry:
```
Waiting for client connection
```

### Spustenie hry
Po tom ako sa nám podarilo spustiť program pre ovládanie bota je potrebné spustenie hry samotnej. Po stiahnutí hry z odkazu uvedeného v prvej časti tejto príručky je potrebné rozbalenie tohot priečinku.
Spustiteľný súbor hry sa nachádza na tejto ceste:
```
.../TUKE_AI_Client/Windows/DFC.exe
```

Po spustení by sme sa mali dostať na nasledujúcu obrazovku:
![img1](https://github.com/bblazek98/diplomova_praca/blob/main/img/img1.png)

V tomto výbere zvolíme možnosť SOLO GAME pre testovanie.

Pri správnom spustení a postupe by mala začať hra. 
![img2](https://github.com/bblazek98/diplomova_praca/blob/main/img/img2.png)

V konzole spusteného bota sa nachádza pravidelný výpis akcií zoradený podľa úžitku a výpis príkazu prislúchajúceho zvolenej najlepšej akcii, ktorý bol odoslaný na vykonanie.
Vybratá akcia je zvýraznená v konzole zelenou farbou

```
Action Utility Values:
['activate_sentinel', 1.0]
['pickup_bomb', 0.8]
['attack_base', 0.47872000000000003]
['idle', 0.4]
['pickup_health_orb', 0.2]
['deploy_bomb', 0]
['deploy_health_orb', 0]
=============
Command sent:  ['-109246.995999', '114078.190728', '21795.15', 'False', 'False', '5']
```
