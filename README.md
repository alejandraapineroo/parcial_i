Objetivo
Simular la gestión de imágenes satelitales mediante un modelo Productor-Consumidor que separa la recepción (rápida/irregular) del procesamiento (lento/constante).

Implementación Técnica
Gestión de Datos: Se utiliza una queue.Queue (FIFO) para almacenar temporalmente las imágenes y evitar la pérdida de datos durante picos de recepción.

Paralelismo: Implementado con hilos (threading) para que los satélites y los analistas operen de forma independiente sin bloquearse entre sí.

Lógica:

Satélites: Generan datos en intervalos aleatorios.

Analistas: Procesan la cola según su capacidad disponible, permitiendo escalabilidad.

Ejecución: 

El flujo de datos se visualizará en la consola hasta que se interrumpa manualmente (Ctrl+C).
