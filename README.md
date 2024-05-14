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
La síntesis es el proceso de convertir el código RTL en una red de puertas lógicas y otros componentes digitales que pueden ser implementados físicamente en un chip FPGA. Durante la síntesis, Vivado realiza optimizaciones de diseño y genera una netlist, que es una descripción detallada de cómo los componentes lógicos están interconectados. Esta netlist está específicamente adaptado al dispositivo FPGA que estás utilizando, teniendo en cuenta las características y limitaciones del hardware.

#### Implementation
Toma la netlist generada por la síntesis y la coloca y enruta dentro de la arquitectura del FPGA. Esto implica asignar las funciones lógicas específicas a los bloques lógicos del FPGA y conectar estos bloques a través de su matriz de interconexión. Este paso es crítico porque las decisiones de colocación y enrutamiento afectan directamente al rendimiento, al uso del área, y al consumo de energía del diseño final.

#### Device programming
Carga el diseño finalizado y probado en el FPGA físico. Esto se hace generalmente a través de un archivo de configuración, un archivo bitstream, que contiene toda la información necesaria para configurar los elementos programables del FPGA. Este archivo se transfiere al FPGA utilizando un programador o directamente desde un sistema embebido o computadora que está conectada al FPGA.

### Diagrama FSM
![Texto alternativo](https://github.com/GabrielCua11/MyFSM/blob/main/diagrama.png)

### Estados


### Simulación en Logisim


### Guía para ver video
