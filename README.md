# Vaja4-interrupt-button-STM32F0
interrupt 
--------------------------------------------------
ODGOVORI:
2. B.)  Gpio_EXTI0 je pin PA0 (push button), PC9 je zelena led, PC8 je modra LED.
3. c.)  HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_9);
d.)  50ms.
e.)  HAL_GPIO_TogglePin(GPIOC,GPIO_PIN_8);
f.)  HAL_Delay(500);
4. b.)Ko pritisnemo push blue button se prižge ZELENA led in sveti, medtem ko MODRA led ves čas utripa .
c.)Ne vpliva na delovanje tipke.  Zato, ker s pritiskom na tipko kličemo callback funkcijo prekinitve, da začne modra led svetiti. Tudi zaradi tega, ker zanki niso napisane skupaj ampak v drugih vrsticah( User code begin 3, User code begin 4).
--------------------------------------------------
KOMENTAR NA DELOVANJE:
S pritiskom na tipko se prižge zelena led, medtem ko modra led ves čas utripa z isto frekvenco. Program deluje brez napak.
