# Magyarországi szülészetek térképe 🏥

Interaktív térkép a jelenleg működő, valamint az utóbbi években bezárt vagy szünetelő szülészeti osztályokról Magyarországon.

![Készült Leaflet + OpenStreetMap segítségével](https://img.shields.io/badge/built%20with-Leaflet-199900?logo=leaflet&logoColor=white)
![Licenc](https://img.shields.io/badge/license-MIT-blue.svg)
![Adatok frissítve](https://img.shields.io/badge/data-2026--06-green.svg)

## 🗺️ Mit tartalmaz?

- **46 működő állami szülészet** (Budapest + vidéki vármegyei és egyetemi központok)
- **3 nagy budapesti magánszülészet** (TritonLife Róbert, Maternity, Duna Medical Center)
- **8 bezárt vagy szünetelő szülészet** kontextusként

Minden jelölő tartalmazza az intézmény nevét, helyét és (ha releváns) a státuszára vonatkozó megjegyzést – például, hogy melyik kórház vette át a betegellátást.

## 🚀 Demó

Nyisd meg az `index.html`-t bármilyen modern böngészőben, vagy hostold ingyen GitHub Pages segítségével:

1. Forkold ezt a repót
2. Menj a `Settings → Pages` menübe
3. Source: `Deploy from a branch`, Branch: `main`, mappa: `/ (root)`
4. Mentsd, és a térképed pár perc múlva elérhető lesz a `https://<felhasznalonev>.github.io/<repo-nev>/` címen

## ✨ Funkciók

- 📍 Színkódolt jelölők (állami / magán / bezárt)
- 🔳 Teljes képernyős mód (gombbal vagy `Esc`-kel kiléphető)
- 📱 Reszponzív – mobilon és asztalon is jól néz ki
- 🗒️ Kattintható pop-upok részletekkel
- 🌍 OpenStreetMap alaptérkép – ingyenes, API-kulcs nem kell

## 📁 Fájlszerkezet

```
szuleszetek-terkep/
├── index.html      # Önálló térkép, beágyazott adatokkal
├── data.json       # Külön adatfájl (referenciaként, frissítéshez)
├── README.md       # Ez a fájl
└── LICENSE         # MIT licenc
```

A térkép **önálló**: az `index.html` mindent tartalmaz, ami a futáshoz kell. A `data.json` ennek a tükörmása – ha hozzá akarsz írni vagy módosítani szeretnél, a legegyszerűbb mindkét helyen frissíteni. (Vagy átírhatod az `index.html`-t, hogy `fetch()`-csel olvassa a JSON-t, ha GitHub Pages-en hostolod.)

## 📊 Adatforrások

Az adatok 2024–2026-os sajtóhírek és kórházi weboldalak alapján készültek:

- [Telex](https://telex.hu) – szülészeti ellátás cikkek
- [Népszava](https://nepszava.hu) – mezőtúri, sátoraljaújhelyi cikkek (2026)
- [HVG](https://hvg.hu) – egészségügyi átalakítás cikkek
- [mfor.hu](https://mfor.hu) – szülészetek térképe (2024)
- [EgészségKalauz](https://egeszsegkalauz.hu) – sátoraljaújhelyi cikk
- [Borsod24](https://borsod24.hu) – sátoraljaújhelyi cikkek
- [Pénzcentrum](https://penzcentrum.hu) – keszthelyi cikk
- [Válasz Online](https://valaszonline.hu) – kórházi leépítés (2024)
- Kórházi weboldalak: szszbvk.hu, oroshazikorhaz.hu, ujhelykorhaz.hu, csfk.hu, szlmk.hu, stb.

## 🔄 Legutóbbi adatfrissítés: 2026. június

Fontosabb státuszváltozások az előző verzió óta:

- **Sátoraljaújhely** – 2025. augusztus 1-jén újranyitott (egy hónap szünet után); jelenleg rezidens-rotációval, hétvégén készenléti ügyelettel működik (Forrás: Népszava, 2026. június)
- **Mezőtúr** – a 2025 márciusi szünet *továbbra is tart*, a 2026. májusi sajtóhír megerősítette
- **Mátészalka** – 2026. június 15. – augusztus 31. között ideiglenes ellátási rend (a kórház hivatalos közleménye)
- **Orosháza** – hozzáadva (működik, műtőfelújítás 2025-2026)

## 🤝 Hozzájárulás

Találtál hibát vagy elavult adatot? Köszi, hogy szólsz!

1. Nyiss egy [issue-t](../../issues), vagy
2. Csinálj pull requestet a `data.json` és `index.html` módosításával

Kérlek, **mindig adj meg forrást** (sajtóhír linket vagy kórház hivatalos közleményét), ha státuszt változtatsz.

## ⚠️ Disclaimer

Az itt szereplő információk tájékoztató jellegűek. Az ellátás megkezdése előtt kérlek mindig **ellenőrizd a kórház hivatalos weboldalán**, hogy a szülészet éppen működik-e – a státusz hetente változhat. Sürgős esetben hívd a **112**-t.

## 📜 Licenc

MIT – használd szabadon. Lásd a [LICENSE](LICENSE) fájlt.

A térkép adatait az [OpenStreetMap](https://www.openstreetmap.org/) közreműködői biztosítják, [ODbL](https://www.openstreetmap.org/copyright) licenc alatt.
