# Sistema de Alquiler de Vehículos

Este es un sistema de alquiler de vehículos que permite a los usuarios ver una lista de vehículos disponibles, alquilar vehículos por un periodo de tiempo, ver el resumen de sus alquileres y generar facturas. El sistema también permite devolver los vehículos alquilados y actualiza la disponibilidad en tiempo real.

## Funcionalidades

- **Ver vehículos disponibles**: Los usuarios pueden ver una lista de vehículos disponibles con detalles como marca, modelo, tarifa por hora y estado (disponible o alquilado).
- **Realizar alquiler**: Los usuarios pueden seleccionar un vehículo, ingresar su información (nombre, correo electrónico, teléfono) y definir la duración del alquiler en horas.
- **Resumen de alquileres**: Se muestra una lista de los alquileres realizados con información detallada del vehículo, usuario, duración y costo total.
- **Generar factura**: Al finalizar el alquiler, el sistema genera una factura con los detalles del alquiler y un botón para imprimirla o enviarla por correo electrónico.
- **Devolución de vehículos**: Los vehículos pueden ser devueltos una vez finalizado el tiempo de alquiler, lo que actualiza su disponibilidad.

## Estructura de Clases

### `Vehicle`
Clase base para los vehículos, contiene propiedades y métodos comunes para todos los tipos de vehículos, como marca, modelo, tarifa por hora y métodos para calcular el costo de alquiler.

### `Car` y `Bike`
Subclases de `Vehicle` que representan un coche y una moto, respectivamente. Cada clase tiene propiedades adicionales específicas de su tipo, como el número de puertas para `Car` o el tipo de moto para `Bike`.

### `Rental`
Clase que representa un alquiler de vehículo, almacena la información del alquiler, el costo total y gestiona la devolución del vehículo.

### `RentalSystem`
Clase principal que gestiona la lista de vehículos, alquileres y ofrece métodos para alquilar, devolver vehículos, y listar los alquileres y vehículos disponibles.

## Uso

### Instalación

1. Clona este repositorio en tu máquina local:

   ```bash
   git clone https://github.com/tu_usuario/sistema-alquiler-vehiculos.git
