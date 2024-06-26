# Kassan palaute- ja inventaario laskusovellus

## Sovelluksen tämänketkiset ominaisuudet ja idea tähän sovellukseen
Sovellus otta vastaan ostojen kokonaissumman, käteisrahamäärän minkä asiakas sen maksamiseen antaa ja kassan inventaarion, eriteltynä kaikkiin seteleihin ja kolikoihin.
Näillä tiedoilla sovellus laskee minkän rahamäärän minkälaisilla seteleillä pitää palauttaa asiakaalle, niin että palautus tapahtuu mahdollisimman isoilla
saatavilla olevilla rahayksiköillä. Se näyttää myös tarkan kolikko- tai setelimäärän kukin rahayksikön kohdalla, minkä asiakaalle pitäisi palauttaa.
Se palauttaa myös uuden kassan inventarion palautuksen jälkeen. Lisäksi sovellus kertoo kassan statuksen 'OPEN' jos rahaa palautukseen riittää, ja ylimääräistä rahaa jää,
'CLOSED' jos palautus on juuri saman suuruinen kuin kassan varat tai 'INSUFFICIENT FUNDS', jos kassan varat ei riitä palautukseen.

Idean tähän sovellukseen sain Freecodecampin JavaScript kurssin loppuharjoituksesta. Siinä vaadittiin vain että sovellus palautta kassan statuksen ja rahamsumman joka yksiköstä
palautettavaksi. Siihen olen kähittänyt oman ratkaisun minkä palautin Freecodecampin ja sain kurssin sertifikaatin.
Sen jälkeen jatkokehitin sovelluksen niin että se näyttää myös setelien määrän minkä pitää palauttaa joka yksikön kohdalla ja uuden kassan inventaarion.

## Käytetyt kielet ja kirjastot
- Sovelluksen koodi toimii JavaScriptillä
- Sovelluksen funktiot on automaattitestattu Jest testauskirjaston kanssa. Myös Jestin liäosa on käytetty Visual Studio Codessa.

## Jatkokehityssuunnitelmat
- Tällä hetkellä sovellus ei huomioi transaktiossa saatun käteisen määrän uuden inventaarion laatimiseen. Se vain poistaa inventaariosta palautussumman.
Sitä korjaamiseen sovelluksen pitää muuttaa sillä tavalla, että myös asiakkaan maksun rahasumman pitää eritellä listalla rahayksikköttäin,
eikä pelkästään syöttää numeroarvolla.

- Sovelluksesta voisi kehittää 'Svelte Native' ja 'Android Studiolla' puheliinsovellus. Se olisi avuksi jos joutuisi työskentelemään
  vanhan kassan kanssa missä ei ole digitalisia apuvälineitä. 

