# Case 05 – .env är fortfarande spårad av Git

## Scenario

En utvecklare har av misstag committat och pushat filen `.env` till Git.

Efteråt skapades en `.gitignore` där `.env` lades till, men filen fortsätter ändå att spåras av Git.

## Din uppgift

1. Kontrollera varför `.env` fortfarande spåras av Git.
2. Se till att Git slutar spåra `.env` utan att filen tas bort från datorn.
3. Kontrollera att `.env` nu ignoreras av Git.
4. Kontrollera att `.env` fortfarande finns kvar på datorn.

> **Tips:** .gitignore påverkar bara filer som Git inte redan spårar. Om filen redan är committad måste du först sluta spåra den.
# Case 02 – Jag råkade jobba på fel branch

## Scenario

Du arbetar i branchen `case-02-fel-branch`.

Du ska gjort en ändring i projektet och skapat en commit.

Efteråt upptäcker du att arbetet egentligen skulle ha gjorts i branchen `case-02-ratt-branch`.

## Din uppgift

1. Gör en mindre ändring i projektet.
2. Skapa en commit i `case-02-fel-branch`.
3. Flytta din commit till `case-02-ratt-branch`.
4. Kontrollera att din commit finns i `case-02-ratt-branch`.
5. Återställ `case-02-fel-branch` så att den inte längre innehåller din commit.

> **Tips:** Kontrollera alltid vilken branch du arbetar i innan du börjar utveckla.
# Case 01 – Jag glömde hämta de senaste ändringarna

## Scenario

Du arbetar i branchen `case-01-glomde-pull`.

Du har gjort några egna ändringar i projektet och committat dem i din branch.

Efteråt inser du att du glömde hämta de senaste ändringarna från `main` innan du började arbeta.

`main` innehåller nu ändringar som saknas i din branch.

Du behöver därför hämta den senaste versionen av `main` och lägga in den i din branch utan att förlora ditt eget arbete.

## Din uppgift

1. Gör en eller flera egna ändringar i `case-01-glomde-pull`.
2. Committa dina ändringar.
3. Kontrollera vilken branch du arbetar i.
4. Hämta de senaste ändringarna från `main`.
5. Lägg in ändringarna från `main` i din branch.
6. Kontrollera att din branch nu innehåller både dina egna ändringar och de senaste ändringarna från `main`.

> **Tips:** Jämför projektet före och efter att du hämtat in ändringarna från `main`.
