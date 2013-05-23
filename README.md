digabi livecd
================================
Sähköisen ylioppilastutkinnon päätelaiteasennuksen testialusta.

(c) 2013 Ville Korhonen (ville@xd.fi)

## Vaatimukset
    apt-get install live-helper

Suositeltavaa käyttää esim. `apt-cacher-ng` -pakettivälimuistia, mikäli käännösoperaatioita on useita.

## Levyn kääntäminen
Versionumeron valintaan käytetään `git describe` -komentoa.
    make dist

Tällä hetkellä levy käyttää julkaisuversiona Debian Jessietä (testing), jolle ei löydy natiivia tukea debootstrapin nykyisestä versiosta.

    ln -s /usr/share/debootstrap/scripts/wheezy /usr/share/debootstrap/scripts/jessie


## Sekalaista
Tällä hetkellä rakennusympäristöstä on seuraavat oletukset:
 - virtuaalikone
 - isäntäkoneelta jaettu hakemisto johon voidaan kirjoittaa, on mountattu /public ; tämän alta löytyy alihakemisto www, joka julkaistaan www-palvelimella

## Lisenssitiedot
Toteutus pohjautuu Debianin pakettikirjastoon, ja sisällytetyt ohjelmat käyttävät lukuisia erilaisia lisenssejä. Kaikki lisenssitiedot löydät osoitteesta [Debianin kotisivuilta](http://www.debian.org/legal/licenses/).
