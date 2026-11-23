# Lösning

## Nyckelkommandon

```bash
git status
git ls-files .env
git rm --cached .env
git status
git commit -m "Stop tracking .env"
git push
git log --oneline
git switch case-02-ratt-branch
git cherry-pick <commit-id>
git switch case-02-fel-branch
git reset --hard HEAD~1
git branch
git status
git add .
git commit -m "Min ändring"
git fetch origin
git merge origin/main
git status
```

## Därför händer det

`.env` är redan committad och spåras därför av Git. Att lägga till `.env` i `.gitignore` gör inte att Git slutar spåra en fil som redan finns i historiken.

Med `git rm --cached .env` tar du bort filen från Git men inte från datorn. Eftersom `.env` finns i `.gitignore` kommer Git sedan att ignorera filen.

## Tips

- Använd `git ls-files .env` för att kontrollera om `.env` fortfarande spåras.
- Använd `git rm --cached .env` för att ta bort `.env` från Git utan att ta bort filen från datorn.
- Kontrollera med `git status` att `.env` inte längre är tracked.
- Kontrollera att `.env` fortfarande finns kvar på datorn.
- Kontrollera att `.env` finns med i `.gitignore`.
- Committa och pusha ändringen när du har kontrollerat att allt fungerar.
Commits tillhör den branch där de skapades.

Om du råkar arbeta i fel branch kan du flytta commiten till rätt branch med `git cherry-pick` och sedan ta bort den från den felaktiga branchen.

## Tips

- Använd `git log --oneline` för att hitta commit-id.
- Kontrollera att du står i `case-02-ratt-branch` innan du kör `git cherry-pick`.
- I det här caset ska commiten flyttas från `case-02-fel-branch` till `case-02-ratt-branch`.
- Kontrollera med `git status` att allt är klart.
Du har börjat arbeta och gjort egna ändringar i `case-01-glomde-pull`, men branchen innehåller inte de senaste ändringarna som finns i `main`.

Efter att du har committat ditt eget arbete kan du hämta den senaste informationen från GitHub och sedan lägga in ändringarna från `main` i din egen branch.

På så sätt får din branch både dina egna ändringar och de senaste ändringarna från `main`.

## Tips

- Använd `git branch` för att kontrollera att du står i `case-01-glomde-pull`.
- Använd `git status` för att kontrollera dina ändringar.
- Committa ditt eget arbete innan du hämtar in ändringarna från `main`.
- Använd `git fetch origin` för att hämta den senaste informationen från GitHub.
- Använd `git merge origin/main` för att lägga in ändringarna från `main` i din branch.
- Kontrollera med `git status` att allt ser rätt ut efteråt.
- Kontrollera att både dina egna ändringar och ändringarna från `main` finns kvar.
