# Filmutforskare

En liten filmutforskare som körs helt i webbläsaren (ren `index.html`, ingen server).
Sök på tema, titel, skådespelare eller regissör; filtrera på årtal och kategorier;
få förslag utifrån filmer du gillar. Data hämtas från [TMDb](https://www.themoviedb.org/).

## Använd den

Öppna sidan (lokalt eller via GitHub Pages). Första gången klistrar du in din egen
**gratis TMDb-nyckel** (themoviedb.org → Settings → API → "API Key (v3 auth)").
Nyckeln sparas **bara i din webbläsare** (localStorage), aldrig i koden eller på nätet.
Valfritt: en gratis [OMDb-nyckel](https://www.omdbapi.com/apikey.aspx) för äkta IMDb-betyg.

Alla inställningar (genrer, årtal, favoriter) sparas per enhet/webbläsare – så varje
dator kommer ihåg sina egna val.

## Publicera på GitHub Pages

1. Lägg filerna i ett GitHub-repo.
2. Settings → Pages → Source: "Deploy from a branch" → branch `main`, mapp `/ (root)`.
3. Öppna `https://<användarnamn>.github.io/<repo>/`.

`film_config.json` (nyckeln till den gamla Python-versionen) ligger i `.gitignore`
och checkas aldrig in.

## Gamla Python-versionen

`film.py` är den ursprungliga serverversionen (kräver Python + `film_config.json`).
Den behövs inte för den statiska sidan men ligger kvar för referens.
