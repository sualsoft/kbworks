---
title: "Microsoft Teams Public Preview"
category: Governance
description: "Debby van der Mije  12 oktober 2021  Geen reacties"
image: /assets/img/blog/teams-public-preview.png
author: "Debby van der Mije"
author_image: "/assets/img/91f5acc932e1256b68cc4bab1612f6a1.png"
author_description: "De disrupter. Zorgt voor opschudding en een frisse blik. Doet alles net even anders. Staat voor productiviteit, effectiviteit en vrijheid met de nieuwe manier van samenwerken. Verantwoordelijk voor de visie en strategie."

hero:
  cover_image: "/assets/img/blog/teams-public-preview.png"
---

# Microsoft Teams public preview

Aan het begin van dit jaar heeft Microsoft een feature uitgebracht waardoor je bepaalde features eerder kan testen. Dit noemde zij public preview voor Microsoft Teams, zie ook [deze video](https://www.youtube.com/watch?v=drxvYP3_gSI). Vanaf 24-07-2021 gaat hier wat in veranderen en gaat Microsoft Teams de Preview van Office volgen. Dit betekend dat wanneer Office preview ge-update wordt, dat ook Teams wordt ge-update met de laatste nieuwe preview features.

Een belangrijk verschil is dat vroeger alleen een aantal mensen Teams updates kregen en dat dit verschilde van de mensen die Office previews kregen. Vanaf 24-07-2021 zullen de mensen die Office preview gebruiken, wat betekend dat zij Current Channel (preview) hebben, ook standaard Microsoft Teams Previews krijgen. Dit is namelijk de Global instelling. Wil je dit liever niet? Dan moet je dit in de policy aanpassen.

## Update de Microsoft Teams Policy’s

Hiervoor ga je als Microsoft Teams administrator naar [http://admin.teams.microsoft.com](http://admin.teams.microsoft.com/) en hier klik je op teams en dan op update Policy’s

![update policies](/assets/img/blog/update-policies-1024x522.png)

Wanneer je eenmaal in de policies zit dan kun je daar meerdere regels hebben, zoals hier bijvoorbeeld 2 regels: 1 globaal(standaard) en 1 voor test gebruikers. Wat direct opvalt is dat er achter beide Preview features hetzelfde staat. Namelijk Follow Office Preview…

![policies update](/assets/img/blog/policies-update-1024x522.png)

Wil je dit aanpassen voor de standaard gebruikers dan klik je op de policy(beleidsregel) die je wil aanpassen en dan kun je deze aanpassen. Je hebt momenteel nog keuze uit 3 opties:

![Instellingen Microsoft Teams Preview](/assets/img/blog/instelling-preview-1024x522.png)

Wat straks overblijft is dus not Enabled en Follow office Preview. Voor het uitzetten kies je dus not enabled en vervolgens apply. Na deze wijziging kan het tot 24 uur duren voor de Policy actief is.

##

## Hoe kan ik mijn Office in Preview krijgen?

Standaard staat je Office vaak op Monthly of soms zelfs nog later. [Hier kun je trouwens alle vormen van updates vinden](https://docs.microsoft.com/en-in/deployoffice/overview-update-channels#BKMK_MC). En op [deze pagina](https://docs.microsoft.com/en-in/officeupdates/update-history-microsoft365-apps-by-date) kun je alles zien wat er wekelijks wordt ge-update. Om te zien in welke release jij zit kun je eenvoudig naar office gaan. Vervolgens kun je op Bestand en dan op Account klikken.

![huidig kanaal office](/assets/img/blog/huidig-kanaal-office.gif)

Om je huidige versie aan te passen naar de preview versie moet je een command prompt uitvoeren. Dit doe je door op start te klikken en vervolgens CMD te type. Vergeet niet dat je deze opstart als administrator.

![commandprompt opstarten](/assets/img/blog/commandprompt-opstarten.gif)

Hierna type je in de command prompt:”**cd C:Program FilesCommon FilesMicrosoft SharedClickToRun**” Met dit commando ga je naar de locatie waar de installatie file staat van Office.

![root van office](/assets/img/blog/root-van-office.png)

Vervolgens type je “**OfficeC2RClient.exe /changesetting Channel=CurrentPreview**” en op enter. Hierdoor wordt het configuratie bestand aangepast.

![Configuratie aanpassen](/assets/img/blog/Configuratie-aanpassen.png)

Wanneer dit gedaan is, moet de huidige gebruiker nog ge-update worden. Dit doe je door dit in te typen “**OfficeC2RClient.exe /update user”** en vervolgens op enter te klikken. Office gaat nu updaten naar de preview versie. In mijn geval werd er niets ge-update.

![office update](/assets/img/blog/office-update.gif)

Hierna kijken we of Office is ge-update en zijn we in sync. Let wel op, voor Teams moet je nog wel via Info en dan Public preview aanzetten. Daarna moet je Teams opnieuw opstarten.
