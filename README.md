## Descripción del proyecto

Al operador de telecomunicaciones Interconnect le gustaría poder pronosticar su tasa de cancelación de clientes. Si se descubre que un usuario o usuaria planea irse, se le ofrecerán códigos promocionales y opciones de planes especiales. El equipo de marketing de Interconnect ha recopilado algunos de los datos personales de sus clientes, incluyendo información sobre sus planes y contratos.

## Servicios de Interconnect

Interconnect proporciona principalmente dos tipos de servicios:

1. Comunicación por teléfono fijo. El teléfono se puede conectar a varias líneas de manera simultánea.
2. Internet. La red se puede configurar a través de una línea telefónica (DSL, *línea de abonado digital*) o a través de un cable de fibra óptica.

Algunos otros servicios que ofrece la empresa incluyen:

- Seguridad en Internet: software antivirus (*ProtecciónDeDispositivo*) y un bloqueador de sitios web maliciosos (*SeguridadEnLínea*).
- Una línea de soporte técnico (*SoporteTécnico*).
- Almacenamiento de archivos en la nube y backup de datos (*BackupOnline*).
- Streaming de TV (*StreamingTV*) y directorio de películas (*StreamingPelículas*).

La clientela puede elegir entre un pago mensual o firmar un contrato de 1 o 2 años. Puede utilizar varios métodos de pago y recibir una factura electrónica después de una transacción.

## Descripción de los datos

Los datos consisten en archivos obtenidos de diferentes fuentes:

- `contract.csv` — información del contrato;
- `personal.csv` — datos personales del cliente;
- `internet.csv` — información sobre los servicios de Internet;
- `phone.csv` — información sobre los servicios telefónicos.

En cada archivo, la columna `customerID` (ID de cliente) contiene un código único asignado a cada cliente. La información del contrato es válida a partir del 1 de febrero de 2020.

## Preguntas que deseo responder con el análisis

- ¿Se tienen más contratos activos que inactivos?
- ¿Cuál es el tipo de contrato que consumen los usuarios?
- ¿Cuál es el período que más duran los contratos mensuales?
- ¿Cuál es el período que más duran los contratos por año?
- ¿Cuál es el período que más duran los contratos por dos años?
- ¿Los usuarios con pareja tienden a tener hijos?
- ¿Los usuarios senior tienen pocos contratos?
- ¿La mayoría de los contratos activos no tienen dependientes?
- ¿Los que tienen dependientes gastan menos en contratos?
- ¿Qué tipo de pago utilizan más?

# Plan de trabajo
`El objetivo del análisis es pronosticar cuáles son los clientes que desean cancelar su suscripción.` Para predecir el objetivo del proyecto se llevarán a cabo los siguientes puntos:

1. **Inicialización del proyecto**
   - Cargar las librerías
   - Lectura de los datos

2. **Preparar los datos**
   - Revisión de formato snake case en columnas
   - Identificar datos faltantes y duplicados
   - Revisión y corrección o modificación de datos
     - Funciones para la revisión de datos
     - Revisión de contract
     - Revisión de internet
     - Revisión de personal
     - Revisión de phone
     - Observación del análisis de los datos
   - Enriquecimiento de los datos

3. **Análisis de los datos**
   - Análisis de la proporción de contratos activos vs. inactivos
   - Duración de contratos mensuales
   - Duración de contratos anuales
   - Duración de contratos de dos años
   - Usuarios con pareja y tendencia a tener hijos
   - Usuarios senior y cantidad de contratos
   - Dependientes y contratos activos
   - Dependientes y gasto en contratos
   - Métodos de pago más utilizados

4. **Modelado**
   - Revisión de datos
   - Features engineering
   - Escalado de los datos
   - Segmentación de datos en entrenamiento, validación y pruebas
   - Creación de función de entrenamiento
   - Entrenamiento de modelo sin aplicar balanceo
     - Regresión Logística
       - Criterios de validación
     - Árboles de Decisión
       - Criterios de validación
     - Random Forest
       - Criterios de validación
     - XGBClassifier
       - Criterios de validación
     - CatBoostClassifier
       - Criterios de validación
   - Entrenamiento de modelo con Oversampling
     - Regresión Logística
       - Criterios de validación
     - Árboles de Decisión
       - Criterios de validación
     - Random Forest
       - Criterios de validación
     - XGBClassifier
       - Criterios de validación
     - CatBoostClassifier
       - Criterios de validación
   - Entrenamiento de modelo con Undersampling
     - Regresión Logística
       - Criterios de validación
     - Árboles de Decisión
       - Criterios de validación
     - Random Forest
       - Criterios de validación
     - XGBClassifier
       - Criterios de validación
     - CatBoostClassifier
       - Criterios de validación
   - Creación de tabla de resultados
   - Prueba de modelo con los valores test

5. **Conclusión del proyecto**

6. **Informe de la solución**


