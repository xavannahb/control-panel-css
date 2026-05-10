# Controlpanel CSS

## Gekozen opdracht 

Ik heb gekozen om een control panel te gaan maken. Ik was geinspireerd door een opdracht van iemand van voorgaande jaren die een minecraft kat kon laten lopen. Ik heb vroeger altijd minecraft gespeeld dus ik wilde graag iets met de bloemen van Minecraft gaan doen. 

## Per week 

### Week 1 

**Wat heb ik gedaan?**

In de eerste week ben ik begonnen met een concept te verzinnen. Ik ben begonnen met mijn minecraft bloem eerst uit te tekenen om hem vervolgens met CSS grid te ontwerpen. Ik heb CSS Grid gebruikt om de bloem op te bouwen uit blokjes. Ik heb elke blokje een bepaalde positie gegeven in de juiste column en row. Met die structuur heb ik ook verschillende bloemen gemaakt. 

Daarnaast ben ik ook gaan experimenteren met de achtergronden ervan. Ik heb een dag en een nacht versie gemaakt om mee te beginnen. In principe gewoon een light en dark mode. Daarnaast heb ik gekeken hoe ik een zon of maan kon toevoegen eraan met een kleine animatie dat ze bewegen.

**Wat heb ik geleerd?**

Ik heb geleerd hoe ik met radio buttons :checked verschillende bloemen kon laten zien zonder javascript te gebruiken. Daarnaast heb ik ook daarmee verschillende achtergronden voor de bloemen in een dag en nacht modes. Hier heb ik geleerd om kleine animaties te maken voor de zon en maan.

**Voortgang**

De feedback was  het ontwerp was te statisch. Alles lag plat, er was geen diepte of dynamiek. Tegelijkertijd was de technische basis solide — custom properties, grid, en een duidelijke kleurlogica waren al aanwezig.

Het ontwerp was leuk bedacht alleen een beetje plat. Het is eigenlijk gewoon een 2d bloem. Hier is het misschien leuk om hem 3d te maken. En de zon en maan zijn in minecraft toch ook niet rond? 

### Week 2

**Wat heb ik gedaan?**

Op basis van de feedback besloot ik het ontwerp om te zetten naar 3D. Samen met Sanne heb ik met <cube> kubussen gemaakt in css. Sanne heeft me geleerd hoe ik hier met perspective, transform-style: preserve-3d en rotateX / rotateY de zijkanten van een kubus kunt positioneren zodat ze allemaal op de juiste hoek staan. Ik heb toen op basis van een kubus alle andere aangepast en weer met dezelfde grid een 3d bloem gemaakt. 

Daarnaast ben ik toen gaan kijken hoe ik hem nog meer 3d kan laten lijken. Hier heb ik de met behulp van Sanne en berekening gemaakt om ervoor te zorgen dat de kubussen naar voren en naar achter geplaatst konden worden. 

    /*     translate:0 0 calc(var(--s) * -1); zorgt ervoor dat de bloem naar achter gaat */
    /*     translate:0 0 var(--s); zorgt ervoor dat de bloem naar voren gaat */

Sanne heeft me ook geholpen met het veranderen van de rotatie van de bloem. Door gewoon de hele section op de x of y as te draaien kan je makkelijk een rotatie geven aan je ontwerp. Ik dacht eigenlijk dat je hierbij kubus voor kubus zou moeten verschuiven... 

html:has([value="links"]:checked) & {
        rotate:y 90deg;
}

**Wat heb ik geleerd?**

Dat het maken van een 3D-kubus in CSS makkelijker is dan het lijkt. Ik vond het leuk om ermee te experimenteren om te kijken hoe de kubussen kon positioneren maar er gaat wel veel tijd in zitten om ze allemaal op de juiste positie te krrijgen. Door CSS nesting te gebruiken heb ik per <cube> en <side> de kubus kunnen positioneren. 

**Feedback**

Ik had nog niet echt een 'controlpanel' wat eigenlijk de bedoeling was van de opdracht. Ik had kubussen en bloemen, maar het "control panel" zelf ontbrak nog. Het paneel er echt als een bedieningspaneel uit moest zien niet als een formulier of een rij buttons.

### Week 3

**Wat heb ik gedaan?**

In week 3 ben ik begonnen met het bedieningspaneel te maken. Ik een footer gemaakt waar je de kleur, tijd en rotatie kon aanpassen. Ik heb deze gemaakt alleen was hij niet in de minecraft stijl. Ik heb aan ChatGPT gevraagd voor minecraft kleuren. Om de styling een beetje minecraft te krijgen heb ik een beetje geexperimenteerd met shadows en borders om wat diepte te krijgen om het meer op een bedieningspaneel te laten lijken.

**Feedback**

Het paneel stond in de footer dus het was niet helemaal een bedieningspaneel. Daarnaast mag er wat meer oog naar de styling gaan. Het paneel moet aan het ontwerp toevoegen niet gewoon een controlpanel zijn. 

### Week 4

**Wat heb ik gedaan?**

Ik ben vooral bezig geweest met alle code goed nalopen. De control panel heb ik in de html en css compleet veranderd. Ik heb de controlpanel opnieuw gemaakt en hem verplaatst naar de rechterkant. Hierdoor lijkt het meer op een bedieningspaneel dan een footer van een website. 

Ik heb dezelfde soort styling gebruikt alleen geprobeerd wat meer controls toe te voegen aan mijn ontwerp. Ik heb geen nieuwe bloemen gemaakt maar alleen de kleuren aangepast om tijd te besparen. 

Daarnaast ben ik bezig gegaan met de achtergronden veranderen. Hier heb ik achteraf niet genoeg tijd aan besteed. Ik probeerde met een grid in de body een regenboog te maken maar er zit al een grid op de body om ervoor te zorgen dat alles goed gepositioneerd staat. Als ik meer tijd had zou ik dit helemaal omgooien en daar meer aandacht aan besteden. Ik ben te veel bezig geweest met de control panel mooi en werkend te krijgen

**Wat heb ik geleerd?**

CSS nesting heeft mij geholpen om bepaalde elementen alleen werkend te krijgen binnen de {}. Daarnaast heb ik veel geleerd over het 3d ontwerpen en dat het veel moeilijker lijkt dan dat het daadwerkelijk is. Door 
perspective en transform-style: preserve-3d te gebruiken kon ik mijn bloem 3d krijgen en positioneren. 

## Bronnen

* Inspiratie: project van student uit vorig jaar (Minecraft-kat in CSS)
* Sanne (docent) – uitleg over 3D-kubussen met perspective en transform-style, week 2
* MDN Web Docs – CSS transform
* MDN Web Docs – CSS nesting
* MDN Web Docs – @keyframes
* MDN Web Docs – perspective
* Minecraft bloemendesigns als visuele referentie