# Seminarski-DMS

OPIS

Za potrebe realizacije VPN konekcije između dve lokacije klijenta, potrebno je napraviti simulaciju realizacije VPN konekcije putem Ipsec protokola. Klijent poseduje dva rutera klase Cisco 7201 i za prvu fazu povezivanja mora realizovati vezu između dve kancelarije gde poseduje po jedan internet link sa statičkom IP adresom.

REŠENJE
U ovoj simulaciji, prikazana je mreža sa više rutera. Centralni ruter je R2 kroz koji prolazi VPN saobraćaj. Prilikom prenosa saobraćaja sa računara PC-1 ka PC-2 formira se tunel između rutera R1 i R3 tako da ruter R2 samo „propušta“ saobraćaj između R1-R3 bez uvida u to da postoji formirani VPN tunel kao i to da nema uvid u sadržaj enkapsuliranih paketa (kriptovani). 

KONFIGURACIJA
Za konfiguraciju je iskorišćen GNS3 simulatorsko okruženje. Od upotrebljenih resursa prikazano je sledeće:
- 3 virtuelna rutera (Cisco 7200, Cisco IOS 15.2(4)S4 sa K9 licencom)
- 2 virtuelna switch-a (bez konfiguracije, radi simulacije lokalne mreže)
- 2 virtuelna računara (PC-1 i PC-2)
