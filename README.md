
# AutoInstall-Winget

Ez a projekt egy egyszerű telepítő scriptet és futtatható fájlt tartalmaz, ami Windows 11-en a winget segítségével automatikusan telepíti a megadott programokat.

## Fájlok

- **AutoInstall.exe** — futtatható telepítő (PowerShell script csomagolva)
- **Install-Apps.ps1** — a PowerShell script forrása
- **README.md** — ez a dokumentáció

## Használat

### PowerShell script futtatása

1. Nyisd meg a PowerShellt rendszergazdaként.
2. Navigálj abba a mappába, ahol az `Install-Apps.ps1` található.
3. Futtasd ezt a parancsot:

```powershell
.\Install-Apps.ps1
```
```powershell
irm "https://raw.githubusercontent.com/gabywap/AutoInstall-Winget/refs/heads/main/Install-Apps.ps1" | iex

Vagy futtasd ezt:
```CMD
.\SetupComplete.cmd
```

Ha hiba van a futtatási engedéllyel, akkor először engedélyezd a script futtatást ezzel:

```powershell
Set-ExecutionPolicy RemoteSigned
```

Majd próbáld újra.

---

### AutoInstall.exe futtatása

Egyszerűen kattints duplán az `AutoInstall.exe` fájlra, és a telepítés automatikusan elindul. Látható PowerShell ablakban követheted a folyamatot.

---

## Programok listája

- Microsoft.DirectX
- IrfanSkiljan.IrfanView
- IrfanSkiljan.IrfanView.PlugIns
- Google.Chrome
- Daum.PotPlayer
- VideoLAN.VLC
- Opera.Opera
- Mozilla.Firefox.hu
- 7zip.7zip
- Brave.Brave
- Ghisler.TotalCommander
- MathiasSvensson.MultiCommander
- Piriform.CCleaner
- Notepad++.Notepad++
- Winamp.Winamp
- AIMP.AIMP

---

## Megjegyzés

Ez a script csendes telepítést végez, és folytatja akkor is, ha egy program telepítése hibába ütközik.
