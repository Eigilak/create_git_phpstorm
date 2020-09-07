# Hvordan sætter jeg mit projekt op med Phpstorm og github (╯°□°)╯︵ ┻━┻ |  opdateret


<h3>1. Installer phpstorm</h3>
<ol> 
    <li>Download phpstorm:  https://www.jetbrains.com/phpstorm/download/#section=mac (windows) </li>
    <li>Sig ja til det hele</li>
    <li>done</li>
</ol>

<h3>2. Hvordan opretter jeg et nyt repo på Github? ( GITHUB.com ) </h3>
<ol>2
    <li>Login på github og gå til root url: github.com/</li>
    <li>Til højre ved siden af din profil kan du tilføje et nyt repo ved at trykke på plus også new repo</li>
    <li>skriv repo name</li>
    <li>Vælg public hvis alle skal kunne pushe, og vælg private så det kun er en bestemt gruppe</li>
    <li>Opret repo</li>
</ol>


<h3>3.Opsættelse af githubbruger / git til phpstorm ( I PHPSTORM ) </h3>
<ol>
    <li>Gå til Preferences </li>
    <li>Gå til Version Control</li>
    <li>Gå til GITHUB</li>
    <li>Klik plus og login med dine creds</li>
    <li><b>Hvad gør det?</b> <br> At du ikke skal logge ind med github hvergang du har et nyt projekt tilknyttet et nyt repo. Plus, så skal du kun bruge GUI og ikke terminalen</li>
</ol>

<h3>4. Tilføje eksisterende projekt til nyt rep i github (2 måder) </h3>
<ol>
<li>
    Måde 1 / terminal ( anbefalet ) 
        <ol>
            <li>(på Github.com) Lav et repo på Github.com uden nogen filer, altså uden readme og .gitignore </li>
            <li>(STIFINDER / EXPLORE ) Find din Øvelsemappe hvor du vil have øvelser i og åben det den med terminalen </li>
            <li>(TERMINAL) Opret et ny projekt med expo: expo init PROJEKTNAVN</li>
            <li>Hvis du oprettet med EXPO, så initialisere den git configuration ( så man behøver ikke skrive git init i projektet ) </li>
            <li>Åben dit nye projekt Øvelse/PROJEKTNAVN i PHPSTORM</li>
            <li>(I PHPSTORMS TERMINAL)Skriv:  git add . </li>
            <li>(I PHPSTORMS TERMINAL)Skriv:  git commit -m "First commit" </li>
            <li>(PÅ GITHUB.com) Find det oprettet repositories url fx: https://github.com/Eigilak/video.git</li>
            <li>(I PHPSTORMS TERMINAL ) Skriv: git remote add origin remote DIT URL, MIT ER = https://github.com/Eigilak/video.git</li>
            <li>(I PHPSTORMS TERMINAL ) Skriv: git remote add origin remote https://github.com/Eigilak/video.git</li>
            <li>(I PHPSTORMS TERMINAL ) Skriv: git remote -v</li>
            <li>(I PHPSTORMS TERMINAL ) Skriv: git push -u origin master</li>
            <li>(PÅ GITHUB ) Check om dine ting er pushet</li>
            <li>(I PHPSTORM ) Gå til GIT indstilingerne og kig på LOG</li>
        </ol>
    </li>
    <li> Måde 2 / mindre teknisk
    <ol>
            <li>(på Github.com) Lav et repo på Github.com uden nogen filer, altså uden readme og .gitignore </li>
            <li>(STIFINDER / EXPLORE ) Find din Øvelsemappe hvor du vil have øvelser i og åben det den med terminalen </li>
            <li>(STIFINDER / EXPLORE )Find mappen og se om der er hhv en usyndelig .git ( TRYK CMD + SHIFT + .(dot) for at vise på mac og windows google</li>
            <li>(STIFINDER / EXPLORE )Hvis der er, så kopier de to filer ind i dit projekt som du ønsker at commit til dit repo på github</li>
            <li>Åben projektet i phpstorm og følg nedestående guide guide</li>
        </ol>
    </li>
    
</ol>

<h3>5.Hvordan bruger jeg github med phpstorm? ( I PHPSTORM ) </h3>
<ol>
    <li>Sørg for du er logget ind med github</li>
    <li>Sørg for du har et aktivt gitprojekt (eventuelt check projekt for .git mappen)</li>
    <li>Der tre ikoner i toppen hhv blå og grøn. Fra venstre er det pull, commit og push</li>
    <li>Vigtigt at tilføje .gitignore inden du commiter
     <ol>
            <li>højre klik i projekt og tryk new .gitignor --> .ignore file git</li>
            <li>Skriv følgende i .gitignore: .idea</li>
            <li>Hvad er .idea? <br> config mappe, og er unik fra pc til pc, så lad vær med at push</li>
     </ol>
    </li>
    <li>Når man vil commite, så trykker man commit</li>
    <li>Skriver commit message </li>
    <li>Tryk på commit knappens pil som går ned for at pushe og commite samtidig</li>
    <li>hvis der er en succes, så vil phpstorm komme med en succes besked i højrer hjørne</li>
    <li>Vigtig viden - ligegyldig info
        <ol>
            <li>Du  kan  se på event log, om dine commits er gået i gennem (højre hjørne)</li>
            <li>Derudover kan man tjekke venstre hjørne ved knappen GIT derefter Log:all ( ved siden af terminalen) hvilket commit er den seneste</li>
        </ol>
    </li>
   </ol>



