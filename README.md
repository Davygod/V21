# FORR3CG Vor 2021 - Lokaverkefni (25%)

Áður en lengra er haldið skalt þú stofna nýtt **private** repo á github og bjóða *gestskoli* inn sem samstarfsaðila. Farðu svo inn á Innu og skila slóðinni að repo-inu í annaðhvort **Lokaverkefni** skilahólfið.


  - [Almennar reglur varðandi verkefnið](#almennar-reglur-varðandi-verkefnið)
    - [Skýrsla](#skýrsla)
  - [Verkefnið](#verkefnið)
    - [Ferðaskrifstofan Tskóla-ferðir](#ferðaskrifstofan-tskóla-ferðir)
    - [Grunnkröfur](#grunnkröfur)
    - [Dæmi um aukakröfur](#dæmi-um-aukakröfur)
    - [Námsmat](#námsmat)
  - [Skil verkefnisins](#skil-verkefnisins)
  - [Prófunargögn](#prófunargögn)
    - [Prófunargögn í svigum](#prófunargögn-í-svigum)

## Almennar reglur varðandi verkefnið

- Verkefnið er einstaklingsverkefni. Ef tveir eða fleiri nemendur skila sömu lausnunum er gefið 0 (núll) fyrir þær lausnir.
- Ef kóði er tekinn af netinu (eða öðrum álíka stöðum) skal taka það fram, benda á hvaðan hann kemur og skrifa skýringar (e. comment) við hverja línu kóðans. Almennt eru ekki gefin stig fyrir kóða sem tekinn er af netinu en hann getur samt gefið örfá stig ef hann er t.d. til að bæta útlit forritsins.
- Ekki er heimilt að nota tilbúnar lausnir fyrir listann. Notið ekki auto og allir bendar (e. pointer) skulu vera hráir (e. raw).
- Allur kóði skal skrifaður í C++. Skipta á hverjum klasa í cpp og h skrár (þarf ekki fyrir `node` klasa).
  
### Skýrsla

Halda skal utan um verkefnið á github. Þar á að vera allur kóði ásamt dagbók og skýrslu. Í dagbókinni á að halda utan um hvað er gert og hvenær (ef eitthvað er ekki í dagbókinni þá er það ekki í verkefninu). Skýrslan er svo stutt samantekt á dagbókinni á samt útskýringum á hvernig forritið ykkar vinnur. Þar eiga líka að vera leiðbeiningar fyrir viðmótið sem þið skrifið. Skilið einnig stuttu myndbandi (screen record) þar sem virkni forritsins er sýnd.

Ekki er gefin sérstök einkunn fyrir skýrsluna og það sem á að vera í henni en vanti eitthvað af því sem á að vera í skýrslunni eða það ekki vel unnið kemur það til lækkunar á einkunn verkefnisins.

Sniðmát fyrir skýrsluna má finna [hér](./skyrsluform.md).

## Verkefnið

### Ferðaskrifstofan Tskóla-ferðir

Nú þegar sér fyrir endann á Covid hefur ferðaskrifstofan Tskóla-ferðir beðið þig um að skrifa bókunarkerfi fyrir sig. Ferðaskrifstofan býður upp á þrjár mismunandi ferðir; flugferðir, hjólaferðir og bátsferðir. Fyrir allar ferðir þarf að skrá númer (id), hversu margir geti farið í ferðina og hversu margir eru bókaðir í ferðina. Fyrir flugferðir þarf að auki að skrá hvert er flogið, fyrir hjólaferðina hversu marga klukkutíma hún taki og fyrir bátsferðina hvort báturinn er yfirbyggður eða ekki.

Þegar ferð hefur verið stofnuð þarf svo að vera hægt að uppfæra fjölda farþega í ferðunum. 

### Grunnkröfur

Verkefnið er 100 stig. Fullkomin lausn á grunnkröfum gefur 60 - 80 stig eftir því hvaða leið er valin fyrir listann.

- Gerður klasa fyrir hverja gerð ferðar og svo einn yfirklasi sem heldur utan um gögn sem eru sameiginleg í hinum klösunum.
- Gerðu getters og setters fyrir allar gagnabreytur klasanna. Tryggðu jafnframt að ekki sé hægt að skrá fleiri farþega í ferð en pláss er fyrir.
- Klasarnir þurfa að geta prentað sjálfa sig á snyrtilega á skjáinn.
- Útfærðu þinn eigin listaklasa sem heldur utan um ferðir:
  - Kviklegt fylki (e. dynamic array), gefur engin aukastig ofan á grunnkröfur.
  - Tengdur listi (e. linked list), gefur 10 aukastig ofan á grunnkröfur.
  - Tætitafla (e. hash table, hash map, dictionary), gefur 20 aukastig ofan á grunnkröfur.
- Gerðu notendaviðmót þar sem hægt er að gera eftirfarandi:
  - Það þarf að vera hægt að skrá ferð í listann.
  - Það þarf að vera hægt að sækja ferð úr listanum (án þess að eyða ferðinni).
  - Það þarf að vera hægt að eyða ferð úr listanum.
  - Það þarf að vera hægt að uppfæra fjölda skráðra farþega í ferðum.
    - Viðmótið birtir villumeldingu ef reynt er að skrá fleiri farþega í ferð en pláss er fyrir.
  - það þarf að vera hægt að prenta á skjá lista með öllum ferðum.
  - Hafðu notendaviðmótið sem svipuðu sniði og sýnt verður í kennslustund 4. maí.

### Dæmi um aukakröfur

- Skráavinnsla, hægt er að skrifa listann í skrár og lesa í listann úr skrá. (10 stig)
  - Hér er þægilegast að hver klasi kunni að skrifa sig í skrá og listaklasinn geti lesið skrárnar.
- Gögnin eru röðuð í listanum. (5 stig)
- Litir í viðmóti, hér má nota tilbúna lausn t.d. [rlutil](https://github.com/tapio/rlutil). (5 stig)
- Annað sem ykkur dettur í hug í samráði við kennara.

### Námsmat

Við mat á verkefninu er horft til eftirfarandi (ekki tæmandi listi):
- Virkni
- Lýsandi nöfn á:
  - Breytum.
  - Föllum og færibreytum þeirra.
  - Klösum, gagnaklasar heiti eintöluorðum og byrji á stórum staf.
- Snyrtilega upp settur kóði.
- Skýringar (e. comment) notaðar þar sem það á við.
- Verkefnið unnið jafnt og þétt (commit á github).

## Skil verkefnisins

Skil verkefnisins eru í tvennu lagi:

- Hlutaskil, 30% af lokaeinkunn. Hér á að skila öllum íhluta klösunum þ.e.a.s. klösunum fyrir flugferð, hjólaferð, bátsferð og svo yfirklasanum. Skilist fyrir miðnætti miðvikudaginn 5. maí (ekki verður hægt að fá framlengdan frest). Einkunn fyrir þennan hluta verður gefin fyrir tímann fimmtudaginn 6. maí. Ef engu er skilað í þessum hluta eru 30% farin af lokaeinkunn.
- Lokaskil, 70% af lokaeinkunn. Skilist fyrir hádegi laugardaginn 15. maí. Ekki verður hægt að fá framlengingu á þessum tíma.

## Prófunargögn

Hafið þessi gögn harðkóðuð í forritinu sem þið skilið.

Ferð | Nr. | Fjöldi bókaðir | Heildarfjöldi | Hvert/Tími/Yfirbyggður
--- | --- | :-: | :-: | ---
Flugferð | 900 | 10 | 50 | Akureyri
Flugferð | 901 | 120 | 200 | Tenerife
Flugferð | 902 | 3 | 10 | Grímsey
Flugferð | 903 | 50 | 250 | Boston
Hjólaferð | 904 | 3 | 10 | 4
Hjólaferð | 905 | 0 | 20 | 10
Hjólaferð | 906 | 3 | 5 | 1
Bátsferð | 907 | 2 | 10 | Nei
Bátsferð | 908 | 20 | 100 | Já
Bátsferð | 909 | 6 | 8 | Nei

### Prófunargögn í svigum

```c++
Flugferd(900, 10, 50, "Akureyri");
Flugferd(901, 120, 200, "Tenerife");
Flugferd(902, 3, 10, "Grímsey");
Flugferd(903, 50, 250, "Boston");
Hjolaferd(904, 3, 10, 4);
Hjolaferd(905, 0, 20, 10);
Hjolaferd(906, 3, 5, 1);
Batsferd(907, 2, 10, false);
Batsferd(908, 20, 100, true);
Batsferd(909, 6, 8, false);
```

