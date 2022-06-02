
| Código |	Descripción	                                            | Comentarios |
|--------|------------------------------------------------------------------|-------------|
| 00     | Error en memoria                                                 |-            |
| B0     | No iniciado por pico incorrecto                                  |-            |
| B1     | No iniciado por pico en Uso                                      |-            |
| BA     | No iniciado por surtidor sin conexión                            |-            |
| BD     | Corte por falla de la fuente de alimentación eléctrica.          |-            |
| BE     | Corte por tiempo sin descolgar.	                            | En equipos viejos. |
| BF     | Corte por tiempo sin descolgar o sin caudal.                     | Sin actividad del pulser o sin descolgar el pico |
| C0     | Corte por límite de carga alcanzado.	                            | Límite en vehículo. |
| C1     | Corte normal colgando pico	                                    |-            |
| C2     | Corte normal 2.	                                            | Sólo en consolas viejas. |
| C4     | Corte por teclado en consola.	                            | Apretando la tecla DEL. |
| C6     | Corte por falla en el pulser.	                            | No aplica a todos los pulser, sólo es válido para una secuencia de pulsos del pulser. Se puede deshabilitar desde Configuraciones -> Validar Pulser. |
| ES     | Modo Estacion de Servicio	                                    | Despacho en modo manual |
| H1     | Carga parcial                                                    | Hotfueling |
| H2     | Carga acumulada en la etapa                                      | Hotfueling |
| H3     | Corte de bomba por detección de flujo con electroválvula cerrada | Hotfueling, en dashboard muestra E200 |
| H4     | Corte por falta de señal de sonda                                | Hotfueling Sonda offline |
| H5     | Corte por falta de detección de flotante                         | Hotfueling, detección de ecos 0. |
| PR     | Falla en tique de impresora                                      |-            |
| RC     | Abastecimiento con caudalimetro	                            |-            |
| RS     | Abastecimiento solo con sondas	                            |-            |
| UE     | Transaccion en progreso.	                                    | No debería aparecer casi nunca, o mientras se está despachando. |
| UL     | Lazo desconectado                                                | Solo en vector por ahora |
| ER     | Transacción recuperada                                           | Transacción recuperada de la memoria del EMR4 |
| E1     | Error en EMR4                                                    | Puede ser un error popup, menu, encoder, preset, etc.. |
| U0     | Error desconocido al querer activar con comando AT               | Error al activar con AT. |
| U1     | Otra transacción en curso                                        | Error al activar con AT. |
| U2     | Pico desactivado                                                 | Error al activar con AT  |
| U3     | Pico en uso                                                      | Error al activar con AT  |
| U4     | Nodo pico offline                                                | Error al activar con AT |  
| U5     | Nodo pico inexistente                                            | Error al activar con AT |  
| U6     | Lazo desconectado                                                | Error al activar con AT |  
| U7     | Pico inexistente en la consola                                   | Error al activar con AT |
| U8     | Error en el límite preseteado                                    | Error al activar con AT |
| U9     | Esperando el comando BT para activar                             | Error al activar con AT |
| BR     | Corte por reincio de la consola durante el despacho              | Solo aplica a nodos CC | 
| UD     | Transacción no habilitada por falta de saldo por departamento.   |-            |
| BL     | Corte por límite de dígitos máximo en diplay LCD                 | Solo aplica a nodos CC | 
| MN     | Transacción creada manualmente                                   |-            |