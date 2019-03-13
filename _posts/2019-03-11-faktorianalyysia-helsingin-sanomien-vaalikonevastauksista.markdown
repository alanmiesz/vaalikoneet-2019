---
layout: post
title:  "Faktorianalyysiä Helsingin Sanomien vaalikonevastauksista"
date:   2019-03-11 10:53:55 +0200
categories: hs
datatable: true
---

# Taustaa

Tässä kirjoituksessa tutkitaan Helsingin Sanomien vaalikoneen vastauksia [eksploratiivisen faktorianalyysin](https://en.wikipedia.org/wiki/Factor_analysis) avulla. Menetelmällä voidaan rakentaa jossakin määrin HS:n omaa "arvokarttaa" muistuttava nelikenttä ehdokkaiden vastauksista, samalla näyttäen puolueiden keskimääräisen sijainnin lisäksi karkeasti minkälaisissa kysymyksissä puolueiden sisällä esiintyy hajontaa. 

Faktorianalyysi on tilastollinen menetelmä, jossa muuttujien (tässä tapauksessa ehdokkaiden vaalikonevastausten) keskinäistä hajontaa yritetään kuvataan pienemmällä joukolla muuttujia eli faktoreita. Vaalikoneen tapauksessa voidaan ajatella, että ehdokkaiden vastaukset kysymyksiin heijastelevat esimerkiksi kahta piilevää piirrettä eli faktoria, jotka ovat kussakin ehdokkaassa eri vahvuisia. Toisaalta kysymyksille voidaan laskea *lataukset*, eli mitta sille kuinka paljon saman- tai erimielisyys kuhunkin kysymykseen on peräisin faktoreista. 

Alla näkyvässä kartassa on kuvattu HS:n vaalikonevastausaineisto kahden faktorin avulla ja sijoitettu kukin koneeseen vastannut ehdokas kartalle sen mukaan, kuinka voimakkaita faktorit ehdokkaassa vastausten perusteella ovat. Vastaukset (jotka sinänsä ovat [Likert-asteikollisia](https://en.wikipedia.org/wiki/Likert_scale) eivätkä jatkuvia muuttujia) on muutettu yksinkertaisuuden vuoksi tässä numeroarvoiksi. Tämä ei ole täysin perusteltu ratkaisu, mutta soveltuu tämänkokoisen aineiston laadulliseen ja "viihteelliseen" kuvaukseen. Rotaatiomenetelmänä on käytetty ns. [varimax-rotaatiota](https://en.wikipedia.org/wiki/Varimax_rotation). Faktorien kysymyskohtaiset lataukset ja niihin perustuva tulkinta on käsitelty kartan alapuolella. Eri puolueiden ehdokkaiden näkyvyyden voi kytkeä päälle ja pois klikkaamalla puolueen nimeä.

# "Arvokartta"

{% include visu.html %}

<br />
# Faktorien eli arvokartan akselien tulkinnasta

Vaalikonekysymysten lataukset on esitetty alla. Kysymyksen viereen piirretty nuoli ilmaisee, minkäsuuntaista ja -suuruista latausta kummankin faktorin (x- ja y-akseli) suhteen väitteen kanssa *samaa mieltä* oleminen merkitsee. Esimerkiksi kysymyksen 1 väitteen kanssa samaa mieltä oleminen ilmentää, että x-akselin kuvaama piirre on ehdokkaassa todennäköisesti negatiivinen (mikä sijoittaa ehdokkaan "vasemmalle") ja y-akselin kuvaama piirre hyvin lievästi positiivinen (mikä sijoittaa ehdokkaan "ylös"). Käytännössä lähelle nollaa (esimerkiksi +-0.3 tai vähemmän) alle jääviä latauksia on usein tapana pitää merkityksettöminä, jolloin esimerkiksi y-akselin kuvaama piirre ei juurikaan vaikuta kysymyksen 1 vastaukseen, eikä kummankaan akselin kuvaama piirre kysymyksen 2 vastaukseen. Tässä käytetty varimax-rotaatio pyrkii maksimoimaan faktorien riippumattomuutta, joten sitä käyttäen kysymyksillä on yleensä merkityksellinen lataus vain jommankumman faktorin suhteen.    

Eksploratiivisessa faktorianalyysissä faktoreilla ei ole periaatteessa ennakkoon määrättyä tulkintaa, mutta kysymysten perusteella esimerkiksi julkisten palveluiden yksityistämisen, tuloerojen ja vastikkeellisen sosiaaliturvan kannattaminen selittyvät voimakkaasti x-akselin kuvaamalla piirteellä, eli sitä voitaisiin kuvata jossakin mielessä "oikeistolaisuutena" kuten HS:n arvokartassakin. Toisaalta esitetyt kysymykset ja vastaajapopulaatio vaikuttavat latauksiin: myös esimerkiksi Nato-jäsenyyden valmistelun kannatuksella on vahva "oikealle" vievä lataus, vaikka sen ja yllämainittujen asioiden kannatus eivät välttämättä edellytä tai poissulje toisiaan.

<div class="datatable-begin"></div>

Lataukset                 | Kysymys                               | 
------------------------- | ------------------------------------- | 
<img src="/vaalikoneet-2019/assets/img/1.png" width="500" /> | 1. Terveyskeskuksen lääkäri- ja hoitajakäyntien tulisi olla asiakkaalle maksuttomia.           | 
<img src="/vaalikoneet-2019/assets/img/2.png" width="500" />  | 2. Nykyään vanhuksen tulot vaikuttavat laitoshoidon hoitomaksuihin. Jatkossa myös vanhuksen omaisuutta tulisi käyttää hoivamaksujen kattamiseen.   | 
<img src="/vaalikoneet-2019/assets/img/3.png" width="500" />  | 3. Suomen sosiaaliturvassa olisi syytä siirtyä kansalaispalkan eli vastikkeettoman sosiaaliturvan suuntaan.      | 
<img src="/vaalikoneet-2019/assets/img/4.png" width="500" />  | 4. Sosiaaliturvaa tulisi uudistaa siten, että vastikkeeksi tuesta täytyy tehdä nykyistä enemmän jotakin yhteiskunnallisesti hyödyllistä, kuten opintoja tai vapaaehtoistöitä.  | 
<img src="/vaalikoneet-2019/assets/img/5.png" width="500" />  | 5. Korkeakoulutusta on oltava tarjolla joka puolella Suomea.      | 
<img src="/vaalikoneet-2019/assets/img/6.png" width="500" />  | 6. Päiväkotien varhaiskasvatuksen tavoite on ensisijaisesti mahdollistaa vanhempien työssäkäynti.       | 
<img src="/vaalikoneet-2019/assets/img/7.png" width="500" />  | 7. Kun perhevapaita uudistetaan, tärkeä tavoite on kasvattaa vain isälle suunnattua kiintiötä.      | 
<img src="/vaalikoneet-2019/assets/img/8.png" width="500" />  | 8. Kotihoidon tukea ei saa lyhentää nykyisestä lapsen kolmesta ikävuodesta.      | 
<img src="/vaalikoneet-2019/assets/img/9.png" width="500" />  | 9. Suomessa tulee asettaa kansalaisille henkilökohtainen hiilibudjetti, jossa määritellään hiilijalanjäljelle enimmäisraja.      | 
<img src="/vaalikoneet-2019/assets/img/10.png" width="500" />  | 10. Eduskunnan pitäisi antaa lupia uusille ydinvoimaloille.     |
<img src="/vaalikoneet-2019/assets/img/11.png" width="500" />  | 11. Suomen pitää vähentää hakkuita ilmastonmuutoksen hillitsemiseksi.      | 
<img src="/vaalikoneet-2019/assets/img/12.png" width="500" />  | 12. Suomalaisia pitäisi ohjata vähäisempään lihansyöntiin, esimerkiksi verotuksen keinoin.       | 
<img src="/vaalikoneet-2019/assets/img/13.png" width="500" />  | 13. EU:sta on Suomelle enemmän hyötyä kuin haittaa.      | 
<img src="/vaalikoneet-2019/assets/img/14.png" width="500" />  | 14. Suomen muuttuminen aiempaa monikulttuurisemmaksi ja monimuotoisemmaksi on hyvä asia.      | 
<img src="/vaalikoneet-2019/assets/img/15.png" width="500" />  | 15. Ulkomailta tuleville opiskelijoille pitäisi myöntää oleskelulupa koko tutkinnon suorittamisen ajaksi.      | 
<img src="/vaalikoneet-2019/assets/img/16.png" width="500" />  | 16. Suomen tulisi tällä vaalikaudella ryhtyä valmistelemaan hakemista Natoon.      | 
<img src="/vaalikoneet-2019/assets/img/17.png" width="500" />  | 17. Eduskunnan pitäisi päättää työmarkkinoita koskevista uudistuksista myös vastoin työmarkkinajärjestöjen eli ammattiliittojen ja työnantajajärjestöjen tahtoa.      | 
<img src="/vaalikoneet-2019/assets/img/18.png" width="500" />  | 18. Autoilu on Suomessa jo liian kallista.      | 
<img src="/vaalikoneet-2019/assets/img/19.png" width="500" />  | 19. On oikein rajoittaa ihmisten autoilua, jos robottiautot ovat liikenteessä turvallisempia.      | 
<img src="/vaalikoneet-2019/assets/img/20.png" width="500" />  | 20. Päänsärkylääkkeitä ja vastaavia reseptittömiä itsehoitolääkkeitä pitäisi voida ostaa ruokakaupasta.      | 
<img src="/vaalikoneet-2019/assets/img/21.png" width="500" />  | 21. Homo- ja lesbopareilla pitää olla samat avioliitto- ja adoptio-oikeudet kuin heteropareilla.     | 
<img src="/vaalikoneet-2019/assets/img/22.png" width="500" />  | 22. Jos valtio tarjoaa turvapaikanhakijoiden vastaanottokeskuksen perustamista kotikuntaani, tarjous pitää hyväksyä.     | 
<img src="/vaalikoneet-2019/assets/img/23.png" width="500" />  | 23. Kouluissa kohdellaan koululaisia liian lepsusti. Tiukempi kuri tekisi kouluista parempia.      | 
<img src="/vaalikoneet-2019/assets/img/24.png" width="500" />  | 24. Perinteiset arvot — kuten koti, uskonto ja isänmaa — muodostavat hyvän arvopohjan politiikalle.      | 
<img src="/vaalikoneet-2019/assets/img/25.png" width="500" />  | 25. Julkisia palveluita tulisi ulkoistaa entistä enemmän yksityisten yritysten tuotettavaksi.      | 
<img src="/vaalikoneet-2019/assets/img/26.png" width="500" />  | 26. Jos tulee eteen tilanne, jossa on välttämätöntä joko leikata julkisia palveluita ja sosiaalietuuksia tai korottaa veroja, veronkorotukset ovat parempi vaihtoehto.      | 
<img src="/vaalikoneet-2019/assets/img/27.png" width="500" />  | 27. Suuret tuloerot ovat hyväksyttäviä, jotta erot ihmisten lahjakkuudessa ja ahkeruudessa voidaan palkita.    | 
<img src="/vaalikoneet-2019/assets/img/28.png" width="500" />  | 28. Nykyisen kaltaiset palvelut ja sosiaalietuudet ovat pitkällä aikavälillä liian raskaita julkiselle taloudelle.      | 
<img src="/vaalikoneet-2019/assets/img/29.png" width="500" />  | 29. Talouskasvu ja työpaikkojen luominen tulisi asettaa ympäristöasioiden edelle silloin, kun nämä kaksi ovat keskenään ristiriidassa.     | 
<img src="/vaalikoneet-2019/assets/img/30.png" width="500" />  | 30. Kaikessa päätöksenteossa pitäisi arvioida vaikutukset ympäristöön ja tarvittaessa luopua ympäristölle haitallisista hankkeista.      | 

<div class="datatable-end"></div>

# Aineistosta

Analyysissä käytetty aineisto on ladattu Helsingin Sanomien vaalikoneesta ohjelmallisesti vaalikoneen avauduttua maaliskuussa 2019. On mahdollista, että vaalikoneen näyttämä aineisto on täydentynyt latauksen jälkeen tai että siitä puuttuu yksittäisiä ehdokkaita tai pienpuolueita. 