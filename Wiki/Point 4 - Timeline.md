[Back to menu](https://github.com/MichaelF89/MegaSearch/blob/master/Wiki/Menu.md)
------------------------------------------------------------------------------------------------------------------------------------------

Give next to a traditional list of results, a timeline in which you indicate how many hits there are over time.

------------------------------------------------------------------------------------------------------------------------------------------
De tijdlijn is in onze zoekmachine weergegeven als een histogram, die op de x-as de datum per dag aangeeft en op de y-as het aantal resultaten dat op die dag is gepost laat zien.

Deze tijdlijn kan redelijk informatief zijn voor de gebruiker. Een bepaald onderwerp kan enorm relevant geweest zijn in een korte tijdsperiode, en door de tijdlijn kan de gebruiker de resultaten makkelijk verder filteren om meer artikelen rond die tijd de vinden.

Er wordt gebruik gemaakt van 'Datetime' en van 'Pandas' om de tijdlijn te maken. Eerst worden alle resultaten van een query verzameld. Uit deze resultaten wordt de datum/tijd van plaatsing gehaald, en omgezet naar Datetime objecten om er makkelijker mee te kunnen werken. Daarna worden de datums in een Pandas Dataframe geplaatst, omdat het erg makkelijk is om te sorteren op bepaalde waardes in Pandas. De datums worden gesplit op jaar, maand en dag en daarna worden de aantallen geteld door een simpele count() functie. Deze data kan daarmee meteen worden geplot in een histogram.
