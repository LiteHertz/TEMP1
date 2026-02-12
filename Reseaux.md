# Réseaux

## Modbus

### Paramètres de la drive

Prendre note que la drive monte au paramètre suivant lorsque le paramètre est appliqué  
Comment envoyer un signal à la drive  
`Adresse du slave` `Fonction a envoyer` `emplacement de la case a modifier` `valeure a ecrire`  
Ex : `01` `06` `091B` `0001` Mise du parametre RUN mis a 1  
Ex : `01` `06` `091B` `0000` Mise du parametre RUN mis a 0  
Pour communiquer avec la drive, s'assurer dutiliser RTU, avec 2 stop bits, word de 8 bit, baudrate de 9600
Prendre note que le prof a dit que la comm en generale se fait avec les P9.XX, et de ne pas utiliser les autres parametres.
Prendre note que la fréquence détient un chiffre de décimale, donc, il faut envoyer 300 hertz pour une commande de 30 hertz, de même pour 60, 600 Hz.

- P9.00 (Communication Address)
- P9.01 (Transmission Speed)
- P9.02 (Communication Protocol)
- P9.26 (Serial Comm Speed Reference)
- P9.27 (Serial Comm RUN Command)
