# Tur – Activity Tracker for Android

[Norsk](README.nb.md) | [English](README.md)

**Gjeldende stabile Android-utgave: 0.21, publisert 17.11.2026.** Den separate Home Assistant-integrasjonen er fortsatt beta (0.20.2b3). Homey 0.1.1 er en lokal testpakke.

Tur registrerer hverdagsaktivitet og turer på Android, hjelper deg å følge utviklingen din og lar deg velge hva du deler.

## Installasjon og oppdatering

**[Last ned Tur 0.21 APK](https://tur.fjernkontroll.eu/Tur.apk)** · [Last ned fra Google Disk](https://drive.google.com/file/d/1vfG6mN2VA35m9yOT5zL-tuLASahVqNlX/view)

Installer **Tur.apk** over eksisterende app. Ikke avinstaller først: lokale registreringer og innstillinger skal beholdes. 0.21 (Android-versjonskode 37) oppgraderer både stabil 0.20 og beta B10. **Tur-beta.apk er fortsatt forrige 0.20 B10**, ikke gjeldende hovedversjon.

Du kan også bruke **Innstillinger → Se etter appoppdatering** i Tur. Appoppdatering krever ikke PC. Serveradministrator kan velge den signerte **tur-oppdater.py** under **Administrasjon → Serveroppdatering** i telefonappen, eller bruke **LastOpp-Tur.ps1** fra sin synkroniserte Drive-mappe. Serveradministrasjon krever administratornøkkel; vanlige brukere trenger ikke oppdatere serveren.

## Nytt i 0.21

- Huset øverst til venstre åpner hovedmenyen. Menysøk ligger øverst til høyre, finner undermenyer som Ris og ros og viser hele menystien.
- Avansert visning aktiveres med ti trykk på **Tur**-overskriften inne i den åpne hovedmenyen. Vent deretter på spørsmålet.
- Alle 56 funksjonstips har menysti. **Vis mer / Vis mindre** viser utvidet forklaring og en enkel illustrasjon av stien. Lest-tidspunkt og skjulte tips beholdes ved innholdsendringer.
- Turdetaljer har **Til turlisten** og puddelknappen **Uten hund / Med hund**. Samme puddel brukes i tips og ved turer med hund i listen. Hundemerket beholdes under registrering og endrer ikke poeng eller målinger.
- Pågående bevegelse under 500 meter ligger under **Bevegelse**, ikke blant siste turer.
- Home Assistant-deling støtter valgte tall, gruppenavn fra appen og nøkler som kan trekkes tilbake. Forventet avvisning av ugyldig eller tilbakekalt nøkkel lager ikke lenger en programfeilrapport på serveren.

## Aktivitet, turer og reiser

- Automatisk registrering med telefonens sensorer. Bakgrunnsregistrering avhenger av Android-tillatelser og batteribegrensninger.
- Skritt og dagstotaler, aktivitetsdistanse, kjent stigning, treningsminutter, mål og beregnede poeng.
- GPS-ruter, fart og høydeinformasjon der data finnes; historikk etter dag, uke, måned og år.
- Manuell treningsregistrering med redigering og sletting.
- Transportetapper for bil, tog, båt og buss beholder reiseinformasjon uten aktivitetskreditt.
- Samle passende aktivitets- og transportetapper til en reise. Originalene beholdes og telles én gang i aktivitetssummene.
- Aktivitetsfordeling per halvtime følger eksisterende delingsvalg og krever kompatible klienter og ferske, innsendte data.

## Grupper og frivillig deling

Opprett grupper, inviter andre og sammenlign delt målt aktivitet og måloppnåelse hver for seg. Appens installasjonslenker og gruppeinvitasjoner er separate funksjoner.

Del utvalgte turer eller perioder med visningslenker som kan trekkes tilbake. Personlige lenker krever ikke gruppemedlemskap. Navnevisning og GPS krever separate tillatelser; gruppelenker viser Anonym uten godkjent navnevisning. Maskering av start/slutt reduserer eksponering av steder, men garanterer ikke anonymitet. Tilbakekall henter ikke tilbake en kopi mottakeren allerede har lagret.

## Home Assistant og Homey

I Tur: **Grupper og deling → Home Assistant**. Velg egne tall, opprett en lesetilgangsnøkkel og lim den inn i integrasjonen. Valgfri egen lederstatus dekker i dag, siste 7 og siste 30 dager. Andres navn og tall eksporteres ikke.

[Oppsett for Home Assistant og gjeldende teststatus](https://github.com/trondtorsoe/Tur---HA-integrasjon/blob/main/README.nb.md). Krever Home Assistant 2026.11 eller nyere. Tur legges foreløpig til fra repo-lenken, og er ikke i Markedsplassens standardkatalog. Integrasjon 0.20.2b3 er kontrollert mot app/server 0.21; integrasjonen og Android-appen har uavhengige versjonsnumre.

Homey 0.1.1 er en separat lokal testpakke med installasjonsveiledning, ikke en publisert app i Homey App Store. Fysisk Homey-test gjenstår. Delingsoppsettet for HA/Homey og HA-integrasjonen støtter norsk og engelsk; Android-appen er ikke fullstendig oversatt.

## Kontroller og begrensninger

Utgave 0.21 bestod 217 servertester, 14 Android database-/menytester, Android Java-regresjoner med 129 søkeoppføringer og alle 56 tips, 11 tester mot ekte Home Assistant 2026.11 over lokal TLS og 17 Homey-tester mot 0.21-serveren. APK-signatur, filjustering, signert serverpakke og bevaring ved oppgradering er kontrollert.

Brukerbekreftet i HA: samsvar med tallene i Tur, endrede delingsvalg, gruppenavn og ikon, nøkkelbytte og tilbakekall, og ingen nye tomme sensorer med ukjente verdier. Manuell kontroll av 7/30-dagers sammenligninger, senere automatisk sensoroppretting, bevaring ved omstart/navneendring og lokale gruppenavn gjenstår. Dette er ikke fysisk test av alle Android-skjermer eller Homey-maskinvare.

## Personvern og dette repoet

Repoet inneholder offentlig dokumentasjon og nedlastingslenker. App- og serverkildekode holdes privat. Ikke publiser personlige aktivitetstall, GPS-spor, innlogging, nøkler, databaser eller produksjonslogger, heller ikke i offentlige feilrapporter.
