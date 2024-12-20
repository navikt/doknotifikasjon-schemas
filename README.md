
# Doknotifikasjon-schemas

Unarchived 2024-12-20: 
Fremdeles i bruk, klienter må bes om å oppdatere til `teamdokumenthandtering-avro-schemas`
https://github.com/search?q=org%3Anavikt+%22doknotifikasjon-schemas%22+-is%3Aarchived&type=code

# Dette Github-prosjektet er deprekert
Doknotifikasjon-schemas er erstattet av [teamdokumenthandtering-avro-schemas](https://github.com/navikt/teamdokumenthandtering-avro-schemas), som har alle Avro-skjema for Team Dokumentløsninger.

# Funksjonalitet
Avro-skjemaer for doknotifikasjon, for mer info for felter se på [confluence](https://confluence.adeo.no/display/BOA/doknotifikasjon+-+Funksjonell+Beskrivelse)

Avro skjema blir brukt på denne [applikasjonen](https://github.com/navikt/doknotifikasjon).


# Teknisk

For å legge til Avro skjema til en applikasjon må du legge jitpack som repository til jito og dependency med pakken fra jitpack

``` 	
<repositories>
    <repository>
        <id>jitpack</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
```

``` 	
<dependency>
    <groupId>com.github.navikt</groupId>
    <artifactId>doknotifikasjon-schemas</artifactId>
    <version>${doknotifikasjon-schemas-version}</version>
    <scope>compile</scope>
</dependency>
```

## For å gjøre en release

Hver gang det merges til master blir det gjort en release på Jitpack. Se [her](https://jitpack.io/#navikt/doknotifikasjon-schemas) for alle releases.

## Henvendelser
Spørsmål om koden eller prosjekttet kan rettes til Team Dokumentløsninger på:
* [\#Team Dokumentløsninger](https://nav-it.slack.com/client/T5LNAMWNA/C6W9E5GPJ)
