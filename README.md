# Vaja3-ADC-trigger-timer-conversion-STM32F0


 Izbrala sva pin PC0
Ko se pin obarva zeleno se zraven njega izpiše ADC_IN10
Aktiviramo zeleno LED diodo na izhodu PD12
V Clock Configuration spremenimo APB1 Timer clock (MHz) na 16 MHz
(pritisnemo ENTER).Opazimo da se ta frekvenca spremeni in hkrati spremeni oziroma prilagodi še nekatere druge frekvence.
 V razdelku TIM1, pod Counter Settings, bi radi časovniku spremenili frekvenco na 1 kHz, zato moramo frekvenco ABP1 Timer Clock preskalirati v polju Prescaler (PSC – 16 bit value). Ta vrednost znaša 16.000
# Komentar na delovanja:

Program deluje vendar je branje dokaj ne natančno (verjetno zaradi 8-bitne resolucije in kvalitete potenciometra ).
