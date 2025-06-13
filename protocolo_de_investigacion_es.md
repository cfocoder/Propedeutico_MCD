# Protocolo de Investigación
## Maestría en Ciencia de Datos

---

### 1. Título
**Desarrollo de Modelos Predictivos para el Pronóstico de Ingresos y Presupuestos mediante Ciencia de Datos en Empresas de Software como Servicio (SaaS)**

### 2. Planteamiento del Problema

Los procesos tradicionales de pronóstico de ingresos en la mayoría de las empresas son lentos y propensos a errores debido a su naturaleza manual, dependiendo frecuentemente de hojas de cálculo y juicio humano. Esta dependencia de métodos manuales, incluso cuando están integrados en sistemas corporativos, introduce ineficiencias inherentes. Para las empresas de Software como Servicio (SaaS), que dependen de ingresos recurrentes y diversos enfoques de facturación a clientes, construir modelos precisos que reflejen las posiciones futuras de efectivo puede ser particularmente desafiante.

La naturaleza dinámica del mercado, caracterizada por una mayor volatilidad y patrones de consumo cambiantes, limita aún más la agilidad y la capacidad de toma de decisiones fundamentales de los métodos tradicionales. Los pronósticos inexactos pueden llevar a costosos desabastecimientos o inventarios obsoletos, impactando directamente la rentabilidad. Este proyecto aborda la necesidad crítica de un modelo de pronóstico y presupuestación de ingresos más eficiente, preciso y adaptativo dentro de la industria SaaS.

### 3. Justificación

La proliferación de la Inteligencia Artificial y la Ciencia de Datos ofrece un nuevo paradigma para transformar procesos empresariales críticos, particularmente en el pronóstico de ingresos. Existe una clara demanda por parte de la dirección ejecutiva de información prospectiva que no solo sea precisa, sino también generada con la velocidad que impone el dinamismo del mercado.

Para las empresas SaaS, un pronóstico financiero preciso es crucial para una planificación estratégica efectiva, asignación de recursos y para proporcionar resultados futuros esperados a los inversionistas, con particular enfoque en métricas de retención y expansión (NRR/GRR) que son predictores clave del crecimiento sostenible. El aprovechamiento de algoritmos de aprendizaje automático, que pueden aprender de datos financieros históricos e incorporar información socioeconómica relevante y conjuntos de datos masivos, puede mejorar significativamente la eficiencia y precisión.

Este proyecto se justifica por su potencial para proporcionar a las empresas SaaS un modelo de pronóstico de ingresos que ofrezca estimaciones más robustas, frecuentes y oportunas comparado con empresas que dependen de forecasting manual o modelos lineales simples, optimizando así la planificación financiera y fortaleciendo la capacidad de la empresa para anticipar cambios y capitalizar oportunidades, contribuyendo a su sostenibilidad y crecimiento.

### 4. Antecedentes y Marco Teórico

El pronóstico de ingresos es una función empresarial fundamental que proporciona orientación esencial para la planificación estratégica, asignación de recursos, gestión de la cadena de suministro y competitividad en el mercado. Históricamente, los métodos estadísticos tradicionales han sido la piedra angular de esta disciplina, pero la creciente complejidad de los mercados globales, junto con la proliferación exponencial de Big Data y los avances computacionales, ha impulsado la adopción de técnicas sofisticadas de Ciencia de Datos y Aprendizaje Automático.

#### Métodos Estadísticos Tradicionales para el Pronóstico de Series Temporales

Los modelos clásicos de series temporales, como el **Suavizado Exponencial Temporal (ETS)** y los **Modelos Autorregresivos Integrados de Media Móvil (ARIMA)**, han sido ampliamente estudiados:

- **ETS**: Estos modelos asignan pesos exponencialmente decrecientes a observaciones pasadas, enfatizando datos recientes y capturando flexiblemente componentes de tendencia y estacionalidad.
- **ARIMA y SARIMA**: Modelan la autocorrelación en series temporales, con componentes para valores pasados (AR), diferenciación para estacionariedad (I) y errores de pronóstico pasados (MA). El modelo AR1, un caso específico, también puede utilizarse.

Sin embargo, estos métodos tradicionales frecuentemente tienen dificultades con **suposiciones restrictivas como estacionariedad y linealidad, tienen dificultad para incorporar un gran número de variables exógenas, y no pueden capturar fácilmente relaciones complejas y no lineales prevalentes en datos empresariales del mundo real**. Aunque los modelos más simples pueden ser efectivos en ciertos contextos, sus limitaciones a menudo requieren enfoques alternativos para dinámicas intrincadas y conjuntos de datos grandes.

#### Ciencia de Datos y Aprendizaje Automático en el Pronóstico de Ingresos

El **Aprendizaje Automático (ML)**, una rama de la inteligencia artificial, permite a los sistemas "aprender" de los datos, identificar patrones y tomar decisiones con mínima intervención humana. Para el pronóstico de ingresos, el **aprendizaje supervisado, específicamente la regresión, se utiliza para predecir valores numéricos continuos (ingresos futuros) basados en características de entrada**.

**Algoritmos de ML Relevantes para el Pronóstico:**

- **Modelos Lineales Regularizados** (ej., **LASSO**, **Ridge**, **Elastic Net**): Extienden la regresión lineal agregando términos de penalización para controlar la complejidad del modelo y prevenir el sobreajuste. LASSO es particularmente útil para la selección de características.
- **Modelos Basados en Árboles y de Ensamble** (ej., **Random Forest**, **Máquinas de Impulso Gradual** como **XGBoost** y **LightGBM**): Son no paramétricos y sobresalen capturando relaciones no lineales, ofreciendo alto rendimiento predictivo.
- **Redes Neuronales** (ej., **DNN**, **RNN**, **LSTM**): Son capaces de aprender patrones complejos y a largo plazo y manejar grandes volúmenes de datos. Han mostrado resultados prometedores en predicción financiera y se han aplicado para pronosticar ingresos de empresas.
- **Prophet**: Desarrollado por Facebook, es un procedimiento de pronóstico de series temporales robusto a datos faltantes y cambios de tendencia, modelando tendencias no lineales, múltiples estacionalidades (anual, semanal, diaria) y efectos de días festivos.
- **Servicios de Pronóstico Basados en la Nube**: Como Azure Machine Learning y Amazon Forecast, automatizan técnicas avanzadas de ML para pronóstico de series temporales a gran escala.

Estos enfoques modernos ofrecen ventajas significativas al **manejar datos de alta dimensionalidad, capturar relaciones complejas no lineales, incorporar flexiblemente una amplia gama de variables exógenas y adaptarse a patrones de datos cambiantes**, llevando a pronósticos más precisos, robustos y detallados.

#### Analítica de Big Data y Fusión de Datos

**Big Data** (caracterizado por Volumen, Variedad, Velocidad y Veracidad) ha revolucionado el pronóstico de ingresos al permitir la recolección, almacenamiento y procesamiento de conjuntos de datos masivos internos (transacciones, interacciones con clientes) y externos (tendencias de mercado, indicadores macroeconómicos, sentimiento social, datos competitivos). Esto permite a los algoritmos de ML descubrir patrones sutiles y verdaderos impulsores de ingresos frecuentemente indetectables con métodos tradicionales.

**La Fusión de Datos** es el proceso de integrar información de diversas fuentes heterogéneas (ej., CRM, ERP, comportamiento web, indicadores económicos, datos de cadena de suministro) para crear una vista más comprehensiva, consistente y precisa, lo que puede mejorar significativamente la precisión del pronóstico.

#### Estado del Arte en Pronóstico de Ingresos para Empresas SaaS

La literatura reciente (2020-2025) revela un creciente interés en modelos de pronóstico específicos para empresas SaaS. **Sukow & Grant (2013)** establecieron las bases teóricas del forecasting en modelos de suscripción, mientras que **Pattenden (2023)** demostró que los modelos híbridos ML-series temporales superan métodos tradicionales en un 12-18% para pronóstico de ingresos corporativos digitales. **Barker et al. (2018, 2020)** desarrollaron frameworks automatizados que integran métricas específicas SaaS (churn, expansion revenue, customer lifetime value) con algoritmos de ensemble learning, logrando mejoras significativas en precisión.

**Gap identificado**: Pese a estos avances, existe una carencia de modelos que integren sistemáticamente variables exógenas macroeconómicas con métricas operacionales SaaS (MRR, NRR, CAC) en un framework interpretable. La mayoría de estudios se enfocan en una sola dimensión (churn prediction o revenue expansion) sin considerar el impacto de factores externos en el forecasting integral de ingresos SaaS.

#### Desafíos y Consideraciones

A pesar de su potencial, implementar modelos avanzados presenta desafíos:

- **Calidad y Disponibilidad de Datos**: La calidad del modelo predictivo depende de datos históricos limpios, consistentes y suficientes. Datos faltantes, incorrectos o sesgados pueden degradar severamente el rendimiento.
- **Complejidad, Experiencia y Costos**: Los modelos de ML, especialmente el aprendizaje profundo, son complejos y requieren conocimiento especializado en estadística, programación, algoritmos de ML y experiencia en el dominio. Se asocian costos significativos con infraestructura y desarrollo.
- **Interpretabilidad del Modelo ("Caja Negra")**: Muchos algoritmos avanzados de ML se perciben como "cajas negras", dificultando entender cómo se hacen las predicciones, lo que puede obstaculizar la confianza y adopción. **Las técnicas de IA Explicable (XAI), como SHapley Additive exPlanations (SHAP) y LIME, se utilizan para proporcionar insights sobre las contribuciones de características, fomentando confianza y permitiendo validación por expertos del dominio**.
- **Consideraciones Éticas y Sesgos**: Los modelos pueden aprender y perpetuar sesgos históricos presentes en los datos de entrenamiento, enfatizando la necesidad de desarrollo responsable de IA y auditoría de sesgos.

#### La Analogía de Waze como Marco Conceptual Inspirador

Esta investigación se inspira en la inteligencia dinámica de sistemas de navegación como Waze, que sintetizan múltiples fuentes de datos en tiempo real (rutas históricas, tráfico actual, incidentes, clima) para calcular continuamente rutas óptimas. De manera análoga, este estudio busca desarrollar un modelo de pronóstico de ingresos que trascienda la dependencia de datos de ventas internos puramente históricos para integrar un **espectro más amplio y dinámico de factores de mercado relevantes para empresas SaaS**.

Esto incluye indicadores macroeconómicos, tendencias sectoriales, actividades competitivas, estacionalidades complejas, el impacto de campañas de marketing y promocionales, y otros eventos exógenos que influyen significativamente en los flujos de ingresos. **El objetivo es avanzar más allá de vistas estáticas y retrospectivas para construir un "navegador financiero estratégico" para SaaS, proporcionando pronósticos que no solo sean más precisos sino también ágiles, continuamente recalibrados y, crucialmente, interpretables**, permitiendo la identificación transparente de factores que impulsan los ingresos predichos, similar a cómo Waze proporciona justificaciones contextuales para sus rutas.

Esta transparencia, alcanzable a través de técnicas XAI como SHAP, es fundamental para fomentar la confianza del usuario, permitir validación cualitativa y enriquecer la comprensión estratégica empresarial para empresas SaaS.

### 5. Hipótesis

Basándose en el potencial transformador de la Ciencia de Datos y el Aprendizaje Automático para el pronóstico de ingresos SaaS:

**Hipótesis Principal (H1):** El desarrollo e implementación de un modelo de pronóstico de ingresos basado en ciencia de datos para empresas SaaS, integrando datos históricos internos con variables macroeconómicas y de mercado exógenas relevantes, generará pronósticos de ingresos con **mayor precisión (mejora mínima del 15% en MAPE) y mayor oportunidad** comparado con los métodos actuales de presupuestación y pronóstico predominantemente manuales y menos frecuentes.

- (La precisión se medirá usando métricas de error como **MAPE** o **RMSE**, y la oportunidad se refiere a la capacidad de generar pronósticos con mayor frecuencia y menor retraso temporal, aproximándose a una vista más dinámica de la situación financiera).

**Hipótesis Secundaria 1 (H1.1 - Modelo Semántico de Datos):** Construir un modelo que identifique y pese la influencia de múltiples factores (internos y externos) en los ingresos SaaS llevará a una **comprensión más profunda y semántica de los impulsores empresariales**. Esta comprensión, traducida al modelo, resultará en pronósticos que no solo sean numéricamente más precisos sino que también reflejen mejor la lógica subyacente del comportamiento de ingresos SaaS.

- (Esto implica que el modelo no será una "caja negra" sino que, a través de técnicas de interpretabilidad como **SHAP**, identificará las variables más influyentes).

**Hipótesis Secundaria 2 (H1.2 - Analogía Waze y "Tiempo Real"):** La capacidad del modelo propuesto de ser **actualizado y recalibrado más ágilmente y frecuentemente** (ej., mensual o trimestralmente con datos recientes, contrastando con ciclos anuales extendidos) proporcionará a la dirección SaaS información prospectiva más relevante adaptada a condiciones de mercado cambiantes, acercándose a un sistema de "navegación financiera" que permite ajustes estratégicos más dinámicos y oportunos.

- (Esto no implica "tiempo real" absoluto sino una mejora sustancial en la cadencia y adaptabilidad del proceso de pronóstico).

Estas hipótesis se fundamentan en la premisa de que los algoritmos de Aprendizaje Automático y las técnicas de Ciencia de Datos sobresalen detectando patrones complejos, modelando relaciones no lineales e integrando múltiples fuentes de información, lo cual es crucial para superar las limitaciones de enfoques tradicionales en entornos SaaS dinámicos.

### 6. Objetivos

El objetivo principal es transformar el proceso de pronóstico de ingresos y presupuestación en empresas SaaS desde metodologías tradicionales hacia un enfoque robusto y ágil basado en ciencia de datos.

#### 6.1. Objetivo General

**Desarrollar e implementar un modelo de pronóstico de ingresos para empresas SaaS utilizando técnicas de ciencia de datos** (incluyendo Aprendizaje Automático y análisis de series temporales) que integre datos históricos internos de la empresa con información exógena relevante, buscando **mejorar significativamente la precisión, frecuencia y oportunidad de las proyecciones financieras**, facilitando así una toma de decisiones estratégicas más informada y adaptativa.

#### 6.2. Objetivos Específicos

1. **Diagnosticar y Caracterizar el Proceso Actual**: Analizar el proceso existente de pronóstico de ingresos en una empresa SaaS típica, identificando limitaciones, cuellos de botella, consumo de recursos y métricas de rendimiento.

2. **Diseñar e Implementar una Arquitectura de Datos Integrada**: Identificar, recolectar, limpiar y preprocesar datos históricos internos relevantes (de ERP, CRM, plataformas de marketing, uso del producto) y variables exógenas pertinentes (indicadores macroeconómicos, datos de mercado, estacionalidad, etc.) para el pronóstico de ingresos SaaS. Estructurar un repositorio de datos para integración y acceso eficiente.

3. **Desarrollar y Entrenar Modelos Predictivos de Ingresos**: Investigar, seleccionar y aplicar diversas técnicas de ciencia de datos, incluyendo modelos de series temporales (ej., ARIMA, Prophet) y algoritmos de Aprendizaje Automático (ej., Regresión Lineal Regularizada, Random Forest, Gradient Boosting, Redes Neuronales), para el pronóstico de ingresos SaaS. Entrenar y optimizar parámetros del modelo usando datos históricos preparados, **con el objetivo de mejorar la precisión de pronóstico en al menos 15% vs métodos tradicionales (medido por MAPE)**.

4. **Evaluar y Validar el Rendimiento del Modelo**: Establecer métricas de evaluación cuantitativa (ej., MAPE, RMSE, MAE, MASE) para medir la precisión del pronóstico. Validar el rendimiento del modelo usando técnicas apropiadas (ej., validación cruzada de series temporales, datos de prueba no vistos) y comparar con procesos actuales o modelos de referencia tradicionales.

5. **Proponer un Marco para la Operacionalización y Actualización del Modelo**: Delinear un procedimiento para integrar el modelo de pronóstico desarrollado en el ciclo de planificación financiera SaaS. Definir una estrategia para actualizaciones periódicas del modelo y recalibración con nuevos datos, alineándose con la analogía del "navegador financiero" (Waze). Explorar y demostrar la interpretabilidad del modelo (ej., vía SHAP) para fomentar confianza y comprensión de los impulsores de ingresos entre los tomadores de decisiones.

### 7. Metodología

Este proyecto adoptará un **enfoque cuantitativo y aplicado**, con un **componente longitudinal** para el análisis de datos históricos. Será principalmente descriptivo y correlacional, evolucionando hacia un diseño cuasi-experimental para modelado y evaluación.

#### Fuentes de Datos

La "población" se refiere al universo de datos históricos y contextuales relevantes para el pronóstico de ingresos SaaS:

**Datos Internos de la Empresa:** Las fuentes primarias incluyen sistemas ERP, sistemas contables, CRM y bases de datos de ventas. Las variables clave serán ingresos históricos (desagregados por producto, línea de negocio, cliente, región), datos de transacciones, campañas de marketing internas y precios históricos. Para SaaS, esto incluye específicamente métricas críticas de SaaS: **MRR, ARR para ingresos recurrentes; NRR, GRR para retención y expansión; churn rate, CAC, LTV para eficiencia de adquisición; y ARPU/ARPA para rentabilidad por cliente**.

**Datos Externos (Variables Exógenas):** Fuentes secundarias como institutos nacionales de estadística, bancos centrales y firmas de investigación de mercado. Las variables pueden incluir PIB, inflación, tasas de interés, tipos de cambio, tasas de desempleo y potencialmente indicadores específicos de la industria (ej., crecimiento del mercado de software, actividad competitiva, clima si es relevante para el comportamiento del usuario).

#### Recolección y Preparación de Datos

Se seguirá un proceso riguroso para asegurar la calidad de los datos:

**Recolección de Datos:** Establecer contacto con departamentos relevantes de la empresa (Finanzas, Ventas, TI) para acceso a datos internos. Para datos externos, consultar portales oficiales y descargar conjuntos de datos relevantes.

**Limpieza y Preprocesamiento de Datos:**
- **Manejo de Valores Faltantes**: Evaluar naturaleza y extensión de datos faltantes; aplicar imputación (media/mediana/moda, k-NN) o eliminación.
- **Detección y Tratamiento de Valores Atípicos**: Usar métodos gráficos (diagramas de caja) y estadísticos (rango intercuartílico) para identificar y decidir el tratamiento (eliminación, transformación, retención).
- **Transformación de Datos**: Normalizar o estandarizar variables numéricas. Codificar variables categóricas (codificación one-hot, codificación de etiquetas). Para series temporales, aplicar transformaciones (ej., logarítmica) para estabilización de varianza y diferenciación para estacionariedad.
- **Integración de Datos**: Consolidar datos internos y externos en una estructura única, asegurando alineación temporal correcta.

**Ingeniería y Selección de Características:**
- **Variables Temporales**: Generar características como rezagos (valores de ingresos pasados), componentes de fecha (día de la semana, mes, trimestre, año) e indicadores de estacionalidad (ej., variables dummy para meses específicos).
- **Variables Agregadas/de Interacción**: Crear nuevas características (ej., promedios móviles, ratios, términos de interacción).
- **Selección de Características**: Identificar variables más predictivas y reducir dimensionalidad para prevenir sobreajuste usando análisis de correlación, importancia de características de modelos basados en árboles o conocimiento del dominio.

#### Técnicas de Modelado y Medición

**Herramientas de Software:** **Python** (con bibliotecas como Pandas, NumPy, Scikit-learn, Statsmodels, TensorFlow/Keras, Prophet) y **SQL** para manipulación, análisis y modelado de datos. Jupyter Notebooks o IDEs (VS Code, PyCharm). Herramientas de visualización: Matplotlib, Seaborn, Plotly. Microsoft Power BI o Tableau para dashboards.

**Técnicas de Modelado:**
- **Modelos Clásicos de Series Temporales**: ARIMA/SARIMA para estructura temporal y estacionalidad. Suavizado Exponencial (ETS), incluyendo Holt-Winters.
- **Modelos de Aprendizaje Automático**:
  - **Regresión Lineal Regularizada** (LASSO, Ridge, ElasticNet) para líneas base robustas y selección de variables.
  - **Modelos Basados en Árboles**: Random Forest, Máquinas de Impulso Gradual (XGBoost, LightGBM, CatBoost) para no linealidades e interacciones complejas.
  - **(Opcional) Redes Neuronales**: MLP, o RNN/LSTM para datos secuenciales complejos y más largos.
- **Modelos Especializados**: Prophet (Facebook).

**Entrenamiento y Validación del Modelo:**
- **División de Datos**: División cronológica en conjuntos de entrenamiento, validación y prueba.
- **Validación Cruzada de Series Temporales**: Usar validación cruzada de ventana deslizante o encadenamiento hacia adelante para respetar dependencia temporal y prevenir filtración de datos. Se utilizará validación cruzada temporal (no aleatoria) para preservar la estructura secuencial de los datos.
- **Ajuste de Hiperparámetros**: Emplear técnicas como Búsqueda en Cuadrícula, Búsqueda Aleatoria u optimización Bayesiana para encontrar hiperparámetros óptimos.

**Medición de Rendimiento:** Métricas estándar para precisión de pronóstico:
- **Error Absoluto Medio (MAE)**: Magnitud promedio de errores.
- **Error Cuadrático Medio (MSE)**: Penaliza errores más grandes más.
- **Raíz del Error Cuadrático Medio (RMSE)**: Raíz cuadrada de MSE, en las mismas unidades que la variable predicha.
- **Error Porcentual Absoluto Medio (MAPE)**: Error como porcentaje, útil para comparar diferentes escalas, pero sensible a valores cerca de cero.
- **Error Escalado Absoluto Medio (MASE)**: Compara error del modelo con un pronóstico ingenuo, útil para series estacionales.
- Comparación de modelos basada en estas métricas.

#### Procedimiento de Análisis (Operacionalización de la Analogía Waze)

El proceso general seguirá la analogía de Waze, buscando un sistema de pronóstico dinámico y adaptable:

- **Recolección Continua de Datos ("Sensores")**: Definir un pipeline para ingestión periódica de nuevos datos de ventas SaaS internos y actualizaciones de variables exógenas.
- **Preprocesamiento y Enriquecimiento ("Procesamiento de Señal")**: Aplicar limpieza, transformación e ingeniería de características a nuevos datos.
- **Generación de Pronósticos ("Cálculo de Ruta")**: Ejecutar el(los) modelo(s) seleccionado(s) en datos actualizados para generar pronósticos de ingresos para el horizonte deseado.
- **Evaluación y Calibración ("Recalcular Ruta")**: Monitorear continuamente el rendimiento del modelo contra valores reales. Reentrenar o ajustar hiperparámetros si el rendimiento se degrada significativamente.
- **Interpretación y Comunicación ("Instrucciones de Navegación")**: Utilizar técnicas de interpretabilidad (ej., **SHAP**, LIME, importancia de características) para entender factores que impulsan pronósticos. Presentar pronósticos e insights claramente vía dashboards o reportes automatizados.

#### Consideraciones Éticas

Asegurar confidencialidad y anonimato de datos sensibles de la empresa. Seguir regulaciones de protección de datos si se usan datos a nivel individual. Los modelos no se desarrollarán para tener impactos discriminatorios o injustos.

### 8. Recursos

**Recursos Humanos:** Investigador Principal (estudiante), Asesor Académico (orientación metodológica y teórica), y Contactos de la Empresa (Finanzas, TI, Ventas para acceso a datos y conocimiento del dominio).

**Recursos Materiales y Tecnológicos:** Computadora personal (laptop/desktop con suficiente poder de procesamiento y RAM), internet de alta velocidad. El software incluye **Python** (Pandas, NumPy, Scikit-learn, Statsmodels, Prophet, XGBoost, LightGBM, TensorFlow/Keras, Matplotlib, Seaborn, Plotly), **SQL**, Jupyter Notebooks/IDEs (VS Code, PyCharm), software de gestión de bases de datos (PostgreSQL, MySQL), y opcionalmente, software de BI (Power BI, Tableau). Gestores de referencias bibliográficas (Zotero, Mendeley) y suites de oficina estándar.

**Recursos Económicos y Financieros:** Priorizar **software de código abierto** (Python, R y bibliotecas) para minimizar costos de licenciamiento. Utilizar equipos de cómputo personales y recursos proporcionados por la universidad para evitar necesidades significativas de financiamiento externo. Costos por acceso a datos (fuentes públicas son típicamente gratuitas), entrenamiento (recursos en línea gratuitos/de bajo costo) y suministros menores de oficina.

### 9. Cronograma

El proyecto se desarrollará en las siguientes fases a lo largo de 12 meses:

**Fase 1: Revisión Bibliográfica y Diseño (Meses 1-2)**
- Revisión exhaustiva de literatura
- Refinamiento del marco teórico
- Diseño detallado de la metodología

**Fase 2: Recolección y Preparación de Datos (Meses 3-4)**
- Establecimiento de contactos con empresas SaaS
- Recolección de datos internos y externos
- Limpieza y preprocesamiento de datos

**Fase 3: Desarrollo de Modelos (Meses 5-7)**
- Implementación de modelos de series temporales tradicionales
- Desarrollo de modelos de aprendizaje automático
- Optimización de hiperparámetros

**Fase 4: Evaluación y Validación (Meses 8-9)**
- Evaluación comparativa de modelos
- Validación con datos de prueba
- Análisis de interpretabilidad

**Fase 5: Operacionalización y Documentación (Meses 10-11)**
- Desarrollo del framework de implementación
- Creación de dashboards y reportes
- Documentación de resultados

**Fase 6: Redacción Final y Presentación (Mes 12)**
- Redacción del documento final
- Preparación de presentación
- Entrega del proyecto

### 10. Referencias Bibliográficas

- Arboleda-Florez, M., & Castro-Zuluaga, C. (2023). *Interpretando pronósticos de demanda de ventas directas usando valores SHAP*. Production, 33, e20220035.

- Barker, J., Gajewar, A., Golyaev, K., Bansal, G., & Conners, M. (2018). *Pronóstico de Ingresos Empresariales Seguro y Automatizado*. Association for the Advancement of Artificial Intelligence.

- Box, G. E., Jenkins, G. M., Reinsel, G. C., & Ljung, G. M. (2015). *Análisis de series temporales: pronóstico y control*. John Wiley & Sons.

- Chernozhukov, V., Chetverikov, D., Demirer, M., Duflo, E., Hansen, C., Newey, W., & Robins, J. (2018). *Aprendizaje automático doble/des-sesgado para parámetros de tratamiento y estructurales*. The Econometrics Journal, 21, C1-C68.

- Ensafi, A., Khalili, S., & Alizadeh, M. (2022). *Pronóstico de ventas usando aprendizaje automático – un análisis comparativo*. International Journal of Information Management Data Insights, 2, 100058.

- Grobler-Dębska, K., Mularczyk, R., Gawęda, B., & Kucharska, E. (2025). *Métodos de Series Temporales y Herramientas de Inteligencia Empresarial para Planificación de Presupuestos—Estudio de Caso*. Appl. Sci., 15, 287.

- Katkar, S., Korake, M., Gaikwad, R., Ghodake, S., Rathod, S., & Jadhav, V. D. (2025). *Análisis Integral de Presupuesto y Ventas para Mejorar el Rendimiento Financiero*. International Journal of Scientific Research in Computer Science, Engineering and Information Technology, 11(2), 3796-3802.

- Kolkova, A. (2020). *La Aplicación del Pronóstico de Ventas de Servicios para Aumentar la Competitividad Empresarial*. Journal of Competitiveness, 12(2), 90–105.

- Ma, Q., & Xie, A. (2023). *Aplicación del Análisis de Big Data en Pronóstico de Ventas*. Proceedings of the 2nd International Conference on Financial Technology and Business Analysis.

- Martins, E., & Galegale, N. V. (2023). *Pronóstico de ventas usando algoritmos de aprendizaje automático*. Revista GeSec, 14(7), 11294-11308.

- Olamijuwon, J., & Zouo, S. J. C. (2024). *Aprendizaje automático en pronóstico presupuestario para finanzas corporativas: Un modelo conceptual para mejorar la planificación financiera*. Open Access Research Journal of Multidisciplinary Sciences, 1(6), 35-41.

- Sukow, A. E. R., & Grant, R. (2013). *Pronóstico y el Papel del Churn en Modelos de Negocio de Software-como-Servicio*. iBusiness, 5(1A), 49-57.

- Wang, Y., Xu, J., Gao, T., Zhang, H., Huang, S.-L., Sun, D. D., & Zhang, X.-P. (2025). *FinTSBridge: Una Nueva Suite de Evaluación para Predicción Financiera del Mundo Real con Modelos Avanzados de Series Temporales*. arXiv preprint arXiv:2503.06928v1.

- Wilms, I., & Croux, C. (2024). *Aprendizaje Automático para Pronóstico de Series Temporales Jerárquicas*. arXiv preprint arXiv:2402.09033v2.

- Zou, H., & Hastie, T. (2005). *Regularización y selección de variables vía elastic net*. Journal of the Royal Statistical Society: Series B (Statistical Methodology), 67(2), 301-320.

---

**Elaborado por:** [Nombre del estudiante]  
**Asesor:** [Nombre del asesor]  
**Programa:** Maestría en Ciencia de Datos  
**Fecha:** Junio 2025
