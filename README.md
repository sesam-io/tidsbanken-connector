# tidsbanken-connector

```
$ curl 'https://api.tidsbanken.net/ansatt/ansattgruppe' [..]
{
  "@odata.context": "https://api-ansatte.tidsbanken.net/$metadata#Ansattgruppe",
  "value": [
    {
      "Id": 2147400000,
      "Navn": "10 Fastlønn m/tidskonto"
    },
    {
      "Id": 2147400001,
      "Navn": "20 Timelønn m/overtid"
    },
    {
      "Id": 0,
      "Navn": "dummy-ansatt dummy-mal"
    }
  ]
}

$ curl 'https://api.tidsbanken.net/ansatt/ansatt?$select=*&$top=10' -H 'tb-key: 47130659-[..]' -H 'x-api-version: 3.0' -H 'Ocp-Apim-Subscription-Key: 491f[..]'

{
  "@odata.context": "https://api-ansatte.tidsbanken.net/$metadata#Ansatt(*)",
  "value": [
    {
      "Id": 100,
      "Fornavn": "Super",
      "Etternavn": "Bruker",
      "Adresse": "",
      "Postnummer": "",
      "Poststed": "",
      "TlfPrivat": "",
      "Mobil": "",
      "Epost": "",
      "Fodt": null,
      "Tittel": "",
      "Lonnskonto": "",
      "AnsattDato": null,
      "Personnummer": "",
      "Sluttet": false,
      "SluttetDato": null,
      "AvdelingId": "1",
      "Aktiv": true,
      "Identifikator": "1019",
      "AntallFerieDager": 25.0,
      "Notat": "",
      "ProsjektId": "0",
      "Stillingsprosent": 100,
      "Element1Id": "",
      "Element2Id": "",
      "Kjonn": "",
      "Kommune": 9999,
      "MalId": 2147400000,
      "Innleie": false,
      "Fastlonn": null,
      "IceNavn": "",
      "IceNr": "",
      "PersonaliaBekreftet": null,
      "AntallHalveFerieDager": 0.0,
      "SistEndretDato": "2023-12-06T09:27:57.713Z",
      "SistEndretAvId": 100,
      "OpprettetDato": "2005-11-07T18:59:56Z",
      "OpprettetAvId": null
    }
  ]
}
```
