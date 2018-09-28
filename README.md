# Antirrebote
Antirrebote digital para pulsadores escrito en VHDL para FPGA

Programa escrito en VHDL cuya función es que el sistema se mantiene en el mismo estado cada vez que se mantiene presionado un pulsador.
EJ:
  ->Pulsador A en estado Bajo; Pout=0
  ->Presionamos pulsador A; Pin=1
  ->Pulsador A en estado Alto; Pout=1
  Si mantenemos presionado el pulsador, es decír; Pin=1
  ->Pulsador A se mantiene en estado Alto
  
 Si soltamos el pulsador, Pout aún seguirá en estado Alto.
 Pout cambia si y solo el pulsador vuelve a ser presionado.
 
 El Antirrebote es ideal para toda clase de circuitos que usan pulsadores.
 De no usar Antirrebote, cada vez que se presione el pulsador, Pout oscilará entre Alto y Bajo
