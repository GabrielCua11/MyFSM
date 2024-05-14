# Examen Parcial 3 de Sistemas Digitales

## Link al video

[Video demostrativo de Gabriel Cuá](URL)

## Explicación

### Tablas

El documento Excel contiene una tabla de transiciones y una tabla de salidas para la FSM que controla el semáforo con una señal de emergencia que redirige a todos los estados hacia el estado S0. Adicionalmente tiene otro botón de pánico que los redirige al estado S2, y un semáforo para bicicletas. Recordemos que...

- Tabla de transiciones: define cómo el semáforo cambia de un estado a otro basado en las entradas actuales y las señales de emergencia y pánico.
- Tabla de salidas: define las salidas (luces de semáforo activadas) para cada estado posible.

### Pasos del development flow

A continuación de describen los cinco pasos del flujo de diseño típico en Vivado para desarrollar y desplegar un sistema digital en una FPGA.

#### RTL Code
RTL (Register Transfer Level) Code se refiere a la escritura del código fuente que describe el comportamiento y la estructura del sistema digital que quieres implementar. En el caso de este proyecto, este código se escribió en SystemVerilog. Este paso implica definir cómo los datos se mueven y se transforman en tu sistema, estableciendo registros, operaciones lógicas, máquinas de estados finitos, y más.

#### RTL Simulation
Una vez que tenemos nuestro código RTL, el siguiente paso es simularlo para verificar su comportamiento antes de implementarlo en hardware. RTL Simulation permite probar y validar el diseño simulando cómo reaccionará ante diferentes estímulos o entradas sin necesidad de hardware físico. Esto es crucial para identificar y corregir errores lógicos o de diseño. Se usa un testbench, que es un entorno de prueba que genera señales de entrada para el diseño y permite observar las salidas correspondientes.

#### Synthesis


#### Implementation


#### Device programming
