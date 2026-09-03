---
layout: default
title: Personvernerklæring – FotballLoggen
permalink: /privacy/
---

# Personvernerklæring for FotballLoggen

**Sist oppdatert: 12. mai 2026**

FotballLoggen ("appen") er en mobilapp for å registrere og holde oversikt over treningsøkter og kamper for barn som spiller fotball. Denne personvernerklæringen forklarer hvilke personopplysninger appen behandler, hvordan de behandles, og hvilke rettigheter du har.

**Behandlingsansvarlig:** Ihne Skarbøvik, Norge. E-post: ihne@hotmail.com.

## Kort oppsummert

FotballLoggen krever at du logger inn med e-post + passord eller Apple ID. Data du legger inn – egne barn, lag, treningsøkter, kamper og skader – lagres i appens skytjeneste (Supabase) slik at flere foreldre kan dele samme husholdning. Appen samler ikke inn lokasjon, kontaktdata, helsedata eller bruksstatistikk. Det vises ingen reklame, og data deles ikke med tredjeparter for markedsføring eller analyse.

## Hvilke opplysninger behandles

**Konto og innlogging (du, som forelder):**
- E-postadresse
- Passord (lagret som hash, aldri i klartekst)
- Visningsnavn ("Forelder", e-postprefiks eller eget valg)
- Apple-bruker-ID dersom du logger inn via Apple Sign-in

**Husholdning og medlemskap:**
- Husholdningsnavn ("familie")
- Hvilke brukere som tilhører husholdningen, og rolle (forelder/barn)
- Invitasjonskoder (gyldige i 14 dager)

**Barn du registrerer:**
- Navn
- Eventuelt fødselsår og kjønn (J/G)
- Avatarfarge
- Skadeperioder (start, eventuelt slutt, fritekstnotat)

**Aktiviteter:**
- Type (styrke, fotballtrening, fotballkamp, cup)
- Dato, varighet, lag, aldersgruppe, notater
- Kampresultat, mål, assists, motstander (for kamper)
- Cup-detaljer (navn, sluttdato, sted, kampstadium)

**Barn-pålogging (valgfritt):**
- Hvis du oppretter konto til et barn genereres en intern e-postadresse på domenet `kids.fotballloggen.local`. Denne er kun et teknisk identifikasjonsnummer og brukes ikke til kommunikasjon. Barnet logger inn med brukernavn + passord.

## Hvorfor data behandles (rettslig grunnlag)

Behandlingen skjer på grunnlag av **avtale med deg som bruker** (GDPR art. 6 nr. 1 bokstav b) – appens kjernefunksjon krever at du kan logge inn og dele data mellom enheter og foreldre i samme husholdning. Uten innlogging og lagring kan appen ikke fungere.

Barnedata (navn, fødselsår, skader, treningsstatistikk) behandles på grunnlag av **samtykke fra forelder** som registrerer barnet (GDPR art. 6 nr. 1 bokstav a, sammenholdt med art. 8 om barn). Det er forelders ansvar å vurdere om barnet selv skal informeres, og fra en passende alder, samtykke.

## Hvor lagres data, og hvem har tilgang

Data lagres hos **Supabase Inc.** (datterselskap av Supabase Inc., USA), som er appens databehandler. Supabase drifter PostgreSQL-databasen der appens data ligger. Dataoverføring til USA skjer i henhold til EU-Kommisjonens standard contractual clauses (SCC) og EU–US Data Privacy Framework.

Apple Inc. behandler kun e-postadressen din og en Apple-bruker-ID dersom du logger inn via Apple Sign-in. Du kan velge "Hide My Email" hos Apple – da får appen kun en anonymisert relay-adresse.

**Ingen andre tredjeparter har tilgang.** Appen bruker ikke analyseverktøy, sporings-SDK-er, annonse-nettverk eller markedsføringsverktøy.

Innenfor appen kan andre medlemmer av din husholdning (medforeldre og eventuelt barn med egen konto) se data om barn og aktiviteter i samme husholdning. Du kontrollerer hvem som er medlem ved å sende eller trekke tilbake invitasjoner.

## Hvor lenge lagres data

Data lagres så lenge du har en aktiv konto. Når du sletter kontoen, slettes:
- Din forelder-konto og profil
- Husholdninger der du er eneste forelder, og alt innhold (barn, lag, aktiviteter)
- Husholdninger med andre foreldre består videre uten din konto

Sikkerhetslogger hos Supabase (innloggingstider, IP-adresser) lagres i opptil 30 dager før de slettes automatisk.

## Dine rettigheter (GDPR)

Du har rett til:

- **Innsyn** – be om kopi av alle data appen lagrer om deg og dine barn.
- **Retting** – endre feilaktige opplysninger direkte i appen, eller be om hjelp.
- **Sletting** – slette kontoen og tilhørende data permanent.
- **Begrensning** – be om at behandlingen pauses i en periode.
- **Dataportabilitet** – be om utlevering av data i et maskinlesbart format (JSON).
- **Innsigelse** – protestere mot behandling.
- **Klage** til Datatilsynet (datatilsynet.no) hvis du mener behandlingen er ulovlig.

For å utøve rettighetene: send e-post til **ihne@hotmail.com**. Forespørsler besvares innen 30 dager.

## Sletting av konto

Du sletter kontoen din ved å:
1. Sende e-post til ihne@hotmail.com med "Slett konto" som emne, eller
2. Bruke "Slett konto"-funksjonen i appens innstillinger (når implementert).

Sletting er permanent og kan ikke angres.

## Sikkerhet

Data overføres kryptert (TLS) mellom appen og Supabase. Passord lagres som hash (bcrypt). Tilgang til data internt i appen styres av Postgres Row Level Security, slik at brukere kun kan se data i husholdninger de er medlem av.

## Barn under 13

Appen er designet for å registreres og brukes av en voksen forelder eller foresatt. Barnedata legges inn av forelder. Hvis et barn under 13 år får egen innlogging, er det forelder som har ansvar for samtykke og for å forklare barnet hva som lagres.

Vi behandler ikke barnedata for markedsføring eller profilering.

## Endringer i personvernerklæringen

Hvis personvernerklæringen endres vesentlig vil oppdatert versjon publiseres her med ny dato, og du vil varsles i appen ved første oppstart etter endringen.

## Kontakt

Spørsmål om personvern eller forespørsler om rettigheter? Send e-post til **ihne@hotmail.com**.

---

# Privacy Policy – FotballLoggen (English)

**Last updated: May 12, 2026**

FotballLoggen ("the app") is a mobile app for tracking training sessions and matches for children who play football. This privacy policy explains what personal data the app processes, how it is processed, and your rights.

**Data controller:** Ihne Skarbøvik, Norway. Email: ihne@hotmail.com.

## Summary

FotballLoggen requires sign-in via email + password or Apple ID. Data you enter – your children, teams, training sessions, matches, and injuries – is stored in the app's cloud backend (Supabase) so that multiple parents can share the same household. The app does not collect location, contacts, health data, or usage analytics. No ads are shown, and data is not shared with third parties for marketing or analytics.

## What data is processed

**Account and sign-in (you, as parent):**
- Email address
- Password (stored as hash, never plaintext)
- Display name
- Apple user ID if you sign in via Apple

**Household and membership:**
- Household name
- Members of the household and their role (parent/child)
- Invitation codes (valid for 14 days)

**Children you register:**
- Name
- Optionally birth year and gender
- Avatar color
- Injury periods (start, optional end, free-text note)

**Activities:**
- Type (strength, football training, match, cup)
- Date, duration, team, age group, notes
- Match result, goals, assists, opponent (for matches)
- Cup details (name, end date, location, stage)

**Child sign-in (optional):**
- If you create an account for a child, an internal email on `kids.fotballloggen.local` is generated. It is a technical identifier only and is never used for communication.

## Legal basis

Processing is based on the **contract with you** (GDPR art. 6(1)(b)) – the app's core function requires sign-in and storage. Child data is processed based on **parental consent** (GDPR art. 6(1)(a) and art. 8).

## Where data is stored

Data is stored with **Supabase Inc.** (USA), the app's data processor. Transfers to the US rely on the EU SCCs and the EU–US Data Privacy Framework.

Apple Inc. processes only your email and Apple user ID if you use Apple Sign-in. You may choose "Hide My Email" – the app then receives only a relay address.

**No other third parties have access.** No analytics, tracking SDKs, or ad networks are used.

Within the app, other members of your household can see data about children and activities in the same household. You control membership via invitations.

## Retention

Data is retained as long as your account is active. Deleting your account removes:
- Your parent account and profile
- Households where you are the sole parent, including all content
- Households with other parents remain, minus your account

Supabase security logs (sign-in times, IP) are retained for up to 30 days.

## Your rights (GDPR)

You have the right to: access, correction, deletion, restriction, data portability (JSON export), objection, and to lodge a complaint with the Norwegian Data Protection Authority (datatilsynet.no).

To exercise these rights, email **ihne@hotmail.com**. Requests are answered within 30 days.

## Deleting your account

Email ihne@hotmail.com with subject "Delete account", or use the in-app delete function (when available). Deletion is permanent.

## Security

Data is transferred over TLS. Passwords are stored as bcrypt hashes. Access is governed by Postgres Row Level Security, so users only see data in households they belong to.

## Children under 13

The app is designed to be used by an adult parent or guardian. Child data is entered by the parent. The parent is responsible for consent and for explaining what is stored to the child.

We do not process child data for marketing or profiling.

## Changes

Material changes to this policy will be published here with a new date and shown in the app on first launch after the change.

## Contact

Questions or rights requests: **ihne@hotmail.com**.
