# Lab-03-Robotica-2025-2
Laboratorio 3 de Robótica 2025-2s, realizado por Jeison Diaz y Mateo Ramos

# Integrantes
1. Jeison Nicolás Diaz Arciniegas [jediazar@unal.co](JeisonD0819)
2. Mateo Ramos Cujer [mramoscu@unal.edu.co](MateoKGR)

# Informe

Indice:
1. [Cuadro comparativo](#cuadro-comparativo)
2. [Descripción de las configuraciones home](#descripcion-config)
3. [Procedimiento detallado](#procedimiento)
4. [Explicación completa](#explicacion)
5. [Descripción funcionalidades EPSON RC+ 7.0](#descripcion-funciones)
6. [Análisis comparativo EPSON RC+ 7.0, RoboDK y RobotStudio](#analisis)
7. [Diseño Gripper](#gripper)
8. [Diagrama de flujo](#diagrama)
9. [Plano de planta](#planos)
10. [Código desarrollado](#codigo)

## Cuadro comparativo

| Característica | **EPSON T3-401S** | **Motoman MH6** | **ABB IRB140** |
|----------------|--------------------|------------------|----------------|
| **Tipo de robot** | SCARA (4 ejes) | Articulado (6 ejes) | Articulado (6 ejes) |
| **Grados de libertad (DOF)** | 4 | 6 | 6 |
| **Carga máxima (Payload)** | 3 kg | 6 kg | 6 kg |
| **Alcance máximo** | 400 mm | 1373 mm | 810 mm |
| **Repetibilidad** | ±0.02 mm | ±0.08 mm | ±0.03 mm |
| **Velocidad máxima** | Hasta 4500 mm/s (ejes XY) | 230°/s (articulaciones) | 225°/s (articulaciones) |
| **Montaje** | De mesa (compacto) | En piso, pared o techo | En piso, pared o invertido |
| **Controlador** | EPSON RC+ 7.0 | NX100 / DX100 | IRC5 Compact |
| **Fuente de potencia** | 200–240 V CA monofásico | 200–230 V CA trifásico | 200–600 V CA trifásico |
| **Aplicaciones típicas** | Ensamble electrónico, empaque, pick and place | Soldadura, manipulación de piezas, paletizado | Ensamble, manipulación de materiales, mantenimiento de máquinas |
| **Peso del robot** | ~27 kg | ~130 kg | ~98 kg |
| **Ventajas principales** | Compacto, rápido, bajo costo y fácil de integrar | Alta carga, gran alcance, estructura robusta | Preciso, compacto, ideal para espacios reducidos |
| **Limitaciones** | Alcance corto, solo 4 ejes | Menor precisión que ABB | Mayor costo que Epson |
| **Software asociado** | EPSON RC+ 7.0 | MotoSim EG / NX100 | RobotStudio |
| **Comunicación con PC** | USB / Ethernet | Ethernet / RS-232 | Ethernet / USB |

## Descripción de las configuraciones home
## Procedimiento detallado
## Explicación completa
## Descripción funcionalidades EPSON RC+ 7.0
## Análisis comparativo EPSON RC+ 7.0, RoboDK y RobotStudio

EPSON RC+ 7.0 es el software oficial de programación y control de los robots EPSON. Está pensado para trabajar directamente con el manipulador real, permitiendo definir trayectorias, rutinas y controlar entradas y salidas digitales desde una interfaz bastante intuitiva. Lo más fuerte de EPSON RC+ es su comunicación directa con el robot T3-401S, ya que no requiere configuraciones externas ni licencias adicionales. Sin embargo, es un entorno más cerrado: solo funciona con robots EPSON y no ofrece tantas opciones de simulación avanzada como otras plataformas.

RoboDK, por otro lado, es un software más flexible y multiplataforma. Permite importar modelos de robots de diferentes marcas (ABB, KUKA, Fanuc, Yaskawa, etc.) y programarlos en un entorno 3D muy visual. Además, facilita la generación de código offline, lo que ayuda a probar trayectorias antes de implementarlas físicamente. Es ideal para simulaciones, análisis de alcance, tiempos de ciclo y programación sin depender del hardware, aunque la precisión de la simulación depende del modelo y la calibración.

RobotStudio, desarrollado por ABB, es probablemente el entorno más completo en términos de simulación industrial. Está enfocado en la programación de robots ABB, ofreciendo herramientas de modelado, simulación de celdas completas y generación de código RAPID directamente compatible con los controladores IRC5. Su entorno es más pesado y técnico, pero también más robusto para proyectos de automatización real.

EPSON RC+ es perfecto para la práctica directa con el manipulador EPSON T3-401S; RoboDK es el más versátil para comparar y probar diferentes marcas; y RobotStudio tiene una simulación más avanzada, aunque está cerrado al ecosistema ABB.

## Diseño técnico del gripper neumático
## Diagrama de flujo
## Plano de planta
## Código desarrollado