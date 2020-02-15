# BME Számítógépes Grafika házi szkeleton Linux-CMakere
Készítette: Magyar Máté
--

## 1.Szükséges csomagok
Debian/Ubuntu (valaki ellenőrizze):  
```libgl1-mesa-dev freeglut3-dev libglew-dev```  

Fedora  
```freeglut-devel glew-devel mesa-libGL-devel```

## 2.Módosítások
A forrásban módosításokat kellett végrehajtani a sikeres fordítás érdekében. 
_**A módosítások nem folyásolják be a program működését!**_

* byte típus definiálása a _framework.h_-ban (A használt byte típus
a Win32 SDK része, a definicíó onnan lett másolva)
* A szkeleton onIdle fv.-ben az elkért eltelt időt nem használjuk, a sikeres
fordítás miatt ki van kommentelve. Ha hasznélni szeretnéd, vedd ki a kommentet előle :D

## 3.Fordítás
A fordító a -Werror -Wall flagekkel fordít, ezek jelentése, hogy minden Warning hibának számít
Mivel a házi beadó fordítási paraméterei (egyelőre) nem ismertek számomra, 
ezért a legszigorúbb beállítást használom itt.
Ha erre nincs igény, a CMakeList.txt-ben az ezt bellító sort el lehet távolítani.

## 4.Hibák, észrevételek
A projekt Fedora Linux lett tesztelve, ha más disztron hiba lép fel, 
kérlek jelezd.
Bármi hibát, megjegyzést a https://github.com/barrow099/graf-linux/issues oldalon tedd kérlek.
