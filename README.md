# Obraz systemu plików do pracowni „System plików” (SO)

Repozytorium przechowuje – jako zasób wydania (Release) `v1` – obraz
systemu plików ext2 używany w pracowni nr 2 z Systemów operacyjnych
(Instytut Informatyki Uniwersytetu Wrocławskiego). Obraz jest za duży, żeby
trzymać go w repozytoriach studentów.

| Plik | Rozmiar | SHA-256 |
|---|---|---|
| `debian9-ext2.img.xz` | 126 MiB | `5406fbfacf290bb81b241667a0c0b61d3238e516bdbccf40ddf9047379b4e710` |
| `debian9-ext2.img` (po rozpakowaniu) | 510 MiB | `87ce8bb717741c9e4bc56fba987a0001d0dce58b20035ed92634d943f1163875` |

Studenci nie muszą pobierać obrazu ręcznie – robi to `make obraz`
(i `make test`) w repozytorium z rozwiązaniem. Ręcznie:

```bash
curl -fLO https://github.com/ii-prac/so-ext2-obraz/releases/download/v1/debian9-ext2.img.xz
sha256sum debian9-ext2.img.xz
xz -d debian9-ext2.img.xz
```

Obraz zawiera minimalną instalację systemu Debian 9 („stretch”), czyli
oprogramowanie na licencjach wolnego oprogramowania (szczegóły w katalogu
`/usr/share/doc` obrazu).
