# Conexión TLE-5010/5011

[Página de inicio](../README.md) | [Nivel anterior](Axes-connection.md)

Los TLE5011 y TLE5010 son sensores hall de un solo canal. Operan usando el interface SPI en half-duplex.

![](../images/A1.1.jpg)

**Atención: La linea "Data" de los TLS501x, debe tener una resistencia pull-up de 1k para funcionar correctamente.**

* SPI_SCK - Común para todos los dispositivos SPI (TLE5011, MLX90393, MCP32XX y todas las cadenas registros de desplazamiento)
* SPI_MOSI - Común para todos los dispositivos SPI
* TLE5011_GEN - Común para todos los TLE5011. En algunas placas aparece nombrado como MISO
* TLE5011_CS - Individual para cada TLE5011.

El coste de los sensores TLE5010 y TLE5011 es comparable al de los sensores hall. Se recomienda el uso en los ejes más importantes del controlador, donde se usen de forma continuada en el simuador y cuando se necesite una precisión elevada en las lecturas. La duración de los sensores TLE es casi ilimitada al no necesitar contacto para su funcionamiento, como los sensores hall.

Las placas con los TLE5011 ya montados son raras de encontrar, por esa razón recomendamos hacerse la placa uno mismo. El diagrama del TEL5011 para Sprint Layout se puede obtener de [aquí](../3rd-party/hardware/)

O puedes utilizar un apadatador, por ejemplo este:

![Adaptador TLE501x](../images/SO-8.jpg)

Los sensores TLE5011/5010 respondel al cambio de dirección del eje del campo magnético con respecto al eje del sensor. Para esto, puedes usar un imán rectangular (como en la figura), imanes
The TLE5011/5010 sensors respond to a change in the direction of the axis of the magnetic field relative to the axis of the sensor. To do this, you can use rectangular (as in the figure). Los imanes con forma de disco o anillo se pueden usar si se está seguro que tienen magnetización **diametral**.

![Orientación imán](../images/A1.1.1.jpg)

La configuración de los ejes se describe en la sección [Configuración-ejes](Configuración-ejes.md)

[Página de inicio](../README.md) | [Nivel anterior](Axes-connection.md)
