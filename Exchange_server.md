Voor de installatie van de domeincontroller maken we gebruik van een nieuwe VM. Deze vm moet je niet helemaal opnieuw instellen. Ga op virtualbox naar de template vm dat je hebt aangemaakt en klik op clone. Hier kan je de nieuwe vm een naam en plaats geven waar je hem wilt opslaan. Na deze stap wordt je nieuwe vm gecreëerd.
Verwijder NAT uit de netwerkconfiguratie van de server.
Op de server zou je automatisch op internet moeten kunnen als de domeincontroller opstaat.
Zorg ervoor dat de server genoeg ruimte heeft. Voeg desnoods nog een extra harde schijf toe


# Run sysrep 
Dit programma zorgt ervoor dat er een nieuwe security identifier wordt gecreëerd. Open verkenner en surf naar C:\Windows\System32\Sysprep. Start vervolgens het programma sysprep.exe.
Vink Generalize aan, zorg er ook voor dat Shutdown options op Reboot staat. Klik vervolgens op OK om het proces te starten.
Na de reboot geef je een nieuw wachtwoord in zodat deze anders is dan de andere vm's.


# Configureren computer doormiddel van scripts. (eventueel als laatste script doen als je nog op internet moet)
Ga op de server naar de shared folder. Verplaats het script: scriptEXC naar de c schijf.

Open powershell als administrator en run het script. De computer zou hierna moeten restarten.
foto 11

Het script zal ervoor zorgen dat de naam, het ip address, Subnet en default gateway verandert wordt.

Kijk na of de instellingen van de netwerkadapter voldaan zijn.


Log hierna in met gegevens: Arne\arne.corona en als wachtwoord Admin2020 voor het verdere verloop van de exchange server download.




# Download exchange server 2019
Ga naar https://www.freesoftwarefiles.com/productivity/microsoft-exchange-server-2019-free-download/ op je vm. Hier kan je de nieuwste versie van exhance server downloaden. Deze zal in de shared folder staan. Herplaats deze van de shared folder naar een schijf waar plaats op is. In ons geval de c: schijf.

Ga naar de folder en klik op de iso.

Ga naar de dvd drive van exchanche server en klik op de setup en EXCHANGESERVER
foto 15

Klik in het scherm van de introductie op next.
foto 16

Accepteer de license agreement
foto 17

Klik op use recommended settings
Foto 18

Installeer de mailbox role en zorg ervoor dat hij automatisch server roles en features intalleert indien nodig. 
Foto 20

Geef de installatie een plaats.
foto 22

Geef de naam mee van de organisatie
foto 23

Kies ervoor om malware scanning niet uit te zetten
Foto 24

Wacht to de readiness checks klaar zijn
foto 25

Er komen errors op. Download de bestanden die hierbij komen. Download unified communications managed api 4.0 runtime met de default settings.
foto 26

Download als 2de visual c++ redistributable packages for sivual studio 2013
FOTO 27

Retry hierna de readiness checks, hierna zouden er geen error meer mogen zijn. Druk hierna op install
foto 28

Na de setup progress kan je op finish drukken
foto 29
