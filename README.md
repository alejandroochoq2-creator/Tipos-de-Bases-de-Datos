# Actividad-7.

> [!NOTE]
> ### 1. Tipos de Datos más Comunes en Bases de Datos
> 
> * **INT / INTEGER (Enteros):** Números sin decimales.
>   * *Edad:* `25` (Registro de la edad de un usuario).
>   * *Documento de identidad:* `1018420391` (Identificador único de una persona).
>   * *Stock:* `150` (Cantidad de inventario disponible en bodega).
> 
> * **VARCHAR(n) (Cadenas de Texto de Longitud Variable):** Texto con un límite definido de caracteres.
>   * *Nombre completo:* `"Laura Gómez"` (Registro de datos del cliente).
>   * *Correo electrónico:* `"contacto@empresa.com"` (Contacto para autenticación).
>   * *Dirección:* `"Calle 45 # 18-20"` (Ubicación de entrega).
> 
> * **DECIMAL(p, s) / NUMERIC (Números Decimales de Precisión Exacta):** Valores con parte entera y decimal definida.
>   * *Precio:* `49.99` (Costo exacto de un producto).
>   * *Salario:* `2500000.50` (Monto a pagar a un empleado).
>   * *Tasa de interés:* `1.75` (Porcentaje aplicado en créditos).
> 
> * **DATE (Fechas):** Registro de fecha en formato `AAAA-MM-DD`.
>   * *Fecha de nacimiento:* `1995-08-14` (Para validar la mayoría de edad).
>   * *Fecha de contratación:* `2021-03-01` (Inicio de vínculo laboral).
>   * *Vencimiento:* `2028-11-30` (Expiración de una tarjeta de crédito).
> 
> * **BOOLEAN / TINYINT(1) (Valores Lógicos):** Verdadero (`TRUE`/`1`) o Falso (`FALSE`/`0`).
>   * *Estado de usuario:* `TRUE` (Saber si una cuenta está activa).
>   * *Pago realizado:* `FALSE` (Saber si una factura sigue pendiente).
>   * *Términos y condiciones:* `TRUE` (Confirmación de aceptación de políticas).

> [!IMPORTANT]
> ### 2. Reflexión sobre la frase "No hay sistema" y sus consecuencias
> Escuchar la frase **"No hay sistema"** evoca una parálisis operativa total donde la infraestructura tecnológica o las bases de datos quedan inaccesibles, deteniendo la atención al público y el procesamiento de transacciones.
> 
> **Consecuencias específicas:**
> 1. **Pérdida y corrupción de datos:** Caídas bruscas sin respaldos automatizados destruyen registros recientes o dejan bases de datos inconsistentes.
> 2. **Ineficiencia y retrasos:** Al regresar a métodos manuales (papel y lápiz), los tiempos de procesamiento se multiplican, creando cuello de botella.
> 3. **Errores de procesamiento:** El factor humano en el registro manual incrementa la tasa de errores en cálculos, registros duplicados y mala lectura de datos.

> [!WARNING]
> ### 3. Impacto Sectorial y Ejemplos Históricos
> 
> **Impacto por sectores:**
> * **Salud:** Impide consultar historias clínicas, antecedentes de alergias o dosis de medicamentos, poniendo en riesgo la vida del paciente.
> * **Banca:** Paraliza transferencias, cajeros automáticos y pagos con tarjetas, deteniendo la economía de los usuarios.
> * **Comercio:** Bloquea la facturación, la actualización de inventarios y el despacho de productos.
> 
> **3 Ejemplos Históricos:**
> 1. **Caída global por actualización de CrowdStrike (2024):** Una actualización defectuosa dejó fuera de servicio millones de servidores Windows, cancelando más de 5,000 vuelos a nivel mundial e interrumpiendo la atención en hospitales y bancos.
> 2. **Apagón informático en British Airways (2017):** Un fallo eléctrico en su centro de datos paralizó los sistemas de facturación y equipaje, afectando a 75,000 pasajeros y cancelando más de 800 vuelos.
> 3. **Cierre del Colonial Pipeline por Ransomware (2021):** Un ciberataque obligó a apagar los sistemas de gestión del mayor oleoducto de EE. UU., provocando desabastecimiento de combustible y compras de pánico en varios estados.
> 4. ---

## 3. Antes de las Computadoras: Procesos Manuales vs. Era Digital

Antes de la informática, las operaciones dependían exclusivamente del papel, registros contables encuadernados, sellos físicos, archivo en carpetas y comunicación por correo postal o telegrama.

### **Cuadro Comparativo**

| Proceso / Sector | Era Pre-Digital (Manual) | Era Digital (Sistemas Informáticos) |
| :--- | :--- | :--- |
| **Transacciones Bancarias** | Libretas de ahorro físicas completadas a mano; actualización de saldos mediante fichas de cartón y validación de firmas en papel. | Transferencias electrónicas instantáneas desde aplicaciones móviles y procesamiento de pagos en milisegundos. |
| **Solicitudes y Historias Médicas** | Expedientes físicos archivados en carpetas de papel. La búsqueda de un historial requería desplazamiento físico y tiempo. | Historias clínicas electrónicas (EHR) accesibles en segundos desde cualquier terminal autorizada. |
| **Gestión de Inventario (Comercio)** | Conteos manuales periódicos registrados en libros contables. Alto riesgo de descuadres por pérdidas o robos no detectados. | Monitoreo del stock en tiempo real mediante lectores de códigos de barras/RFID e integración automática con la caja. |
| **Búsqueda de Información / Archivo** | Archiveros físicos organizados por orden alfabético o temático. Espacio físico limitado y riesgo de incendio o deterioro. | Bases de datos relacionales y almacenamiento en la nube con búsquedas complejas mediante consultas SQL. |
2 weeks ago

Update README.md
<img src="FOR GIT HUB.png" alt="">
### 🔄 Comparativa: Excel vs. Base de Datos Relacional (RDBMS)

| Criterio | Microsoft Excel (Hoja de Cálculo) | Base de Datos Real (MySQL, PostgreSQL, etc.) |
| :--- | :--- | :--- |
| **Capacidad de Almacenamiento** | Limitado (máximo **1,048,576 filas** por hoja). Se vuelve lento con grandes volúmenes de datos. | Prácticamente **ilimitado** (escala a terabytes/petabytes según la infraestructura). |
| **Concurrencia (Múltiples Usuarios)** | Limitada. Aunque existen versiones colaborativas en la nube, surgen conflictos al editar celdas simultáneamente. | **Alta concurrencia**. Miles de usuarios y sistemas pueden leer y escribir al mismo tiempo sin bloqueos. |
| **Integridad y Validaciones** | Baja. Permite mezclar texto, números y fechas en una misma columna accidentalmente. | **Estricta**. Cada columna define un tipo de dato fijo (`INT`, `VARCHAR`, `DATE`) y reglas (`NOT NULL`, `UNIQUE`). |
| **Relación de Datos** | Manual. Se vinculan datos mediante fórmulas complejas (`BUSCARV` / `XLOOKUP`), propensas a romperse. | Nativa. Uso de **Claves Primarias (PK)** y **Claves Foráneas (FK)** para garantizar consistencia entre tablas. |
| **Seguridad y Permisos** | Básica. Se protege todo el archivo con contraseña o rangos específicos de celdas. | Granular. Se asignan permisos específicos por usuario para consultar, insertar, modificar o eliminar tablas. |
| **Automatización y Consultas** | Basado en interfaz gráfica, filtros manuales y macros (VBA). | Consultas complejas en segundos mediante **SQL** y conexión directa con lenguajes como Python. |
