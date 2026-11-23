# Lösning

## Nyckelkommandon

```bash
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
