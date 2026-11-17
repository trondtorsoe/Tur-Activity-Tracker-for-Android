# Tur – Activity Tracker for Android

[Norsk](README.nb.md) | [English](README.md)

> **BETA — under aktiv utvikling. Dette er ikke et gjennomtestet produkt. Feil, uferdige funksjoner og endringer må forventes.**

Tur registrerer hverdagsaktivitet og turer på Android, hjelper deg å følge utviklingen din og lar deg velge hva du vil dele med andre.

## Aktivitet og turer

- Automatisk aktivitetsregistrering med telefonens sensorer. Bakgrunnsregistrering avhenger av Android-tillatelser og batteribegrensninger.
- Skritt og dagstotaler, aktivitetsdistanse, høydemeter og treningsminutter.
- Registrerte turer med GPS-kart, fart og høydeinformasjon der data er tilgjengelige.
- Aktivitetsmål, beregnede aktivitetspoeng og utvikling over tid.
- Historikk organisert etter dag, uke, måned og år, med summer og grafer.
- Manuell registrering av trening uten telefon, med redigering og sletting.

## Grupper og frivillig deling

- Opprett grupper, inviter andre og sammenlign delt aktivitet og måloppnåelse.
- Del utvalgte turer og aktivitetsperioder. Deling av appens installasjonslenke og gruppeinvitasjoner er separate funksjoner.
- Personlige visningslenker fungerer uten gruppemedlemskap. Velg utløp, navnevisning og eventuell GPS-deling.
- Gruppelenker viser medlemmer som Anonym med mindre navnevisning er godkjent. GPS har en separat tillatelse.
- Visningslenker kan trekkes tilbake. En kopi mottakeren allerede har lagret, kan ikke hentes tilbake.
- Maskering av GPS-start og -slutt reduserer eksponering av steder, men garanterer ikke anonymitet.

## Betafunksjoner i B7

Disse funksjonene er beskrevet i gjeldende B7-kildepakke. Det betyr ikke at pakken er installert på produksjonsserveren eller testet på fysisk telefon.

- Aktivitetsfordeling per halvtime følger eksisterende valg om aktivitetsdeling. Krever kompatibel app og server; stabil 0.20 sender ikke halvtimer.
- Transportetapper for bil, tog, båt og buss beholder rute og reiseinformasjon uten å gi aktivitetskreditt.
- Samle passende lagrede etapper til en reise med ulike aktiviteter og transport. Originaletappene beholdes og telles én gang i aktivitetssummene.
- Egen inngang for Del min aktivitet og separat samtykke til navn og GPS på visningslenker.

## B8: Home Assistant og menysøk

- **Meny → Søk** finner funksjoner mens du skriver, viser menyplassering og følger brukernivået ditt. Du velger gruppe eller tur der det er nødvendig.
- **Grupper og deling → Home Assistant** deler valgte egne dagstall med en egen nøkkel som kan trekkes tilbake.
- Valgfri egen lederstatus dekker i dag, siste 7 og siste 30 dager, med målt aktivitet og måloppnåelse hver for seg. Andres navn og tall eksporteres ikke.
- Nytt delingsoppsett og Home Assistant-integrasjonen støtter norsk og engelsk. Resten av Android-appen er ikke fullstendig oversatt.
- [Oppsett for Home Assistant og begrensninger i betaen](https://github.com/trondtorsoe/Tur---HA-integrasjon/blob/main/README.nb.md).

B8 er en frivillig beta. Serveren må oppdateres med tilhørende pakke før den nye Home Assistant-koblingen virker. Stabile 0.20-brukere tvinges ikke til å oppdatere.

## Installasjon og oppdateringer

**[Last ned Tur 0.20 B8 APK](https://drive.google.com/file/d/1XXxspnAR8W0Kc5zFWoHol59_F2ru-6PH/view).** APK-filen ligger på Google Disk. Administrator må installere tilhørende B8-serverpakke før Home Assistant-delingen virker. Installer over eksisterende app, ikke avinstaller først.

## Personvern og dette repoet

Repoet brukes til offentlig dokumentasjon, versjonsnotater og distribusjon av APK-filer. App- og serverkildekode holdes privat. Ikke last opp personlige aktivitetstall, GPS-spor, innlogging, nøkler, databaser eller produksjonslogger her, heller ikke i offentlige feilrapporter.
