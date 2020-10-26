Voor de installatie van de domeincontroller maken we gebruik van een nieuwe VM. Deze vm moet je niet helemaal opnieuw instellen. Ga op virtualbox naar de template vm dat je hebt aangemaakt en klik op clone. Hier kan je de nieuwe vm een naam en plaats geven waar je hem wilt opslaan. Na deze stap wordt je nieuwe vm gecreëerd.


# Configureren computer doormiddel van scripts. (eventueel als laatste script doen als je nog op internet moet)
Ga op de server naar de shared folder. Verplaats het script: scriptEXC naar de c schijf.

Open powershell als administrator en run het script. De computer zou hierna moeten restarten.
foto 11

Het script zal ervoor zorgen dat de naam, het ip address, Subnet en default gateway verandert wordt.

# Run sysrep (om in domein te krijgen)
Dit programma zorgt ervoor dat er een nieuwe security identifier wordt gecreëerd. Open verkenner en surf naar C:\Windows\System32\Sysprep. Start vervolgens het programma sysprep.exe.
Start het programma en pak alles default. 
Na de reboot geef je een nieuw wachtwoord in zodat deze anders is dan de andere vm's.

# Download exchange server 2019
Ga naar https://www.freesoftwarefiles.com/productivity/microsoft-exchange-server-2019-free-download/ op je vm. Hier kan je de nieuwste versie van exhance server downloaden. Sla het op op de c: schijf.
