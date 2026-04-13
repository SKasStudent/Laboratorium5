# Projekt Docker - Laboratorium 5

## Opis

Projekt zawiera Dockerfile tworzący obraz bazowy "scratch" alpine, który buduje prostą aplikacje webową, mającą za zadanie wyświetlać:
- Informacje o adresie ip serweru na którym jest uruchomiona
- Informacje o hostname'ie serweru na którym jest uruchomiona
- Wersję aplikacji

## Autor
Szymon Kasperczuk
Adres Email: s101587@pollub.edu.pl

## Polecenia użyte przy realizacji zadania

### Budowanie
```bash
docker build -t [nazwa_obrazu] --build-arg VERSION=[wersja] .
```
**Wynik działania polecenia:** 
<p align="center">
<img width="790" height="511" alt="Screenshot From 2026-04-13 18-20-54" src="https://github.com/user-attachments/assets/5971c7e1-f7a3-48ff-9abd-dc29665fc800" />
</p>

### Uruchamianie
```bash
docker run -d -p 8080:80 --name [nazwa_kontenera] [nazwa_obrazu]
```

**Wynik działania polecenia:** 
<p align="center">
<img width="714" height="35" alt="Screenshot From 2026-04-13 18-21-10" src="https://github.com/user-attachments/assets/05992f84-2fc8-46b1-ac9f-4eacf2f1d271" />
</p>

### Sprawdzenie poprawnosci działania

```bash
curl localhost:8080
```

**Wynik działania polecenia:** 
<p align="center">
<img width="536" height="93" alt="Screenshot From 2026-04-13 18-21-27" src="https://github.com/user-attachments/assets/a97de8e4-c3ba-4382-b085-eada78cb8a7e" />
</p>
