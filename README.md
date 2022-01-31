# Vaja14-UART-Putty-NUCLEO

Privzeto je UART2 vmesnik povezan na USB priključek razvojne ploščice. Katere dva mostička bi morali odspajkati in kateri dve povezavi pospajkati, da bi lahko uporabili pina Tx/D1 in Rx/D0? _SB13___ in __SB14__, __SB63__ in __SB64___.

V področju Connectivity aktivirajte protokol USART2 kot asinhroni. Katera dva pina sta se pobarvala zeleno oz. se aktivirala? ____PA2____ in ____PA3_____.  

V polju Configuration izbranega serijskega vmesnika pustimo privzeto hitrost (Baud Rate), ki znaša ___115200_____Bits/s.  

Za to funkcijo zapišite ukaz za vklop/izklop zelene LED (pomagajte si z metodo toggle, glej vaja0a). _____HAL_GPIO_TogglePin(GPIOA, GPIO_PIN_5);______. 

Dodajte še ukaz za zakasnitev s funkcijo Delay iz knjižnice HAL, in sicer 2 sekunde (glej vaja0a): _____HAL_Delay(1000)_______. 


KOMENTAR:
Imei smo težave pri tipki, saj smo mislili, da efinirana tipka ne deluje oz. ni nastavljena na pin PC13. Zato smo poskušali z drugo tipko, ki smo jo vezal na PC13. Kmalu smo ugotovili, da smo se zmotili in še enkrat preverili kako smo nastavili pin PC13 in ugotovili, da je bil namesto na exit13 nastavljen na INPUT. Ko smo to ugotovili smo nalogo brez večjih težav rešili do konca.

Luka Buzina, Žiga Kuder, Luka Nograšek
