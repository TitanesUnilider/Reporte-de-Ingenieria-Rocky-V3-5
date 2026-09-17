# Rocky V3 — WRO Future Engineers 2026
**Equipo:** Titanes Unilider  
**Coach:** Ing. Victor Manuel García Ríos[cite: 1]

Repositorio oficial de documentación técnica, reportes de ingeniería y control cinemático del robot autónomo Rocky V3 para la competencia World Robot Olympiad (WRO) Future Engineers[cite: 1, 2, 3].

---

## Índice de Documentación Técnica

* **[Documentación Técnica y Estado del Sistema](./Rocky%20WRO%20Future%20Engineers%20-%20Documentacion...)**[cite: 1]
  * Arquitectura completa del chasis ($30 \times 19\text{ cm}$, batalla $17\text{ cm}$, ruedas $7\text{ cm}$)[cite: 1].
  * Mapeo de puertos EV3 (Motor C tracción, Motor A dirección, Gyro en 3, Ultrasonidos en 1 y 2)[cite: 1].
  * Calibración cromática HSV definitiva en Picamera2 (formato XBGR8888)[cite: 1].
  * Lógica de odometría longitudinal y evasión paramétrica[cite: 1].

* **[Reporte de Ingeniería: Calibración y Estabilización EV3](./Reporte%20de%20Ingenieria%20Rocky%20V3%205)**[cite: 2]
  * Sintonización del lazo PID ($K_p = -0.8$, $K_d = 0.0$, $\text{DEADBAND} = 4.0^\circ$) para erradicar el *chattering*[cite: 2].
  * Eliminación del bloqueo de hilo en la dirección mediante `block=False` a $50\text{ Hz}$[cite: 2].
  * Parada de emergencia sanitizada e implementación de la FSM base[cite: 2].

* **[Reporte de Diagnóstico Inicial](./Reporte%20de%20Diagnostico%20Inicial%20Rocky%20V3%204)**[cite: 3]
  * Análisis de fallas de cableado, excepciones en runtime y pérdida de control por codificación[cite: 3].

* **Bitácoras de Evolución del Chasis:**
  * `Primer Reporte Rocky V3.docx`
  * `Transicion Rocky V2 a Rocky V3.docx`
  * `Reporte Tecnico 06 Rocky V3.docx`
  * `Reporte Técnico 07 Integracion RPi y EV3.docx`

---

## Estado Actual del Sistema
* Hardware base y dirección Ackermann estabilizados[cite: 1, 2].
* Visión artificial calibrada en banco para bloques rojos, verdes y magenta[cite: 1].
* Próximo paso: Integración del encoder del motor C para navegación longitudinal por odometría[cite: 1].
