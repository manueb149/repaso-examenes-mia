

# 1. Diseña un pequeño proyecto de investigación basado en IA para reducir el abandono escolar en educación secundaria.

**Título del proyecto:** Sistema inteligente de predicción y prevención del abandono escolar en secundaria.

**1. Planteamiento del problema:**  
El abandono escolar es una problemática creciente en entornos urbanos de alta vulnerabilidad social. Las instituciones no cuentan con herramientas tempranas para detectar señales de riesgo. Se propone usar IA para predecir abandono y personalizar intervenciones.

**2. Hipótesis:**  
Un modelo de clasificación entrenado con datos históricos de asistencia, notas y participación puede predecir con al menos 85% de precisión los casos de riesgo de abandono.

**3. Objetivos:**  
- Diseñar un modelo predictivo basado en árboles de decisión.
- Integrar el modelo a un sistema de alertas para tutores escolares.
- Evaluar la precisión, recall y utilidad percibida por docentes.

**4. Metodología:**  
- Dataset de 5 años de historial académico, asistencia, contexto familiar.
- Preprocesamiento: imputación, normalización, codificación de variables categóricas.
- Modelos: árboles de decisión, Random Forest.
- Validación: 5-fold cross-validation.
- Entrevistas a docentes sobre la utilidad del sistema.

**5. Resultados esperados:**  
- Precisión esperada: >85%.
- Recall en clase positiva (abandono): >75%.
- Alta aceptación docente para acciones preventivas.

**6. Conclusión:**  
Este sistema puede ayudar a intervenir tempranamente y personalizar acciones educativas. Requiere consideraciones éticas por el uso de datos personales, que se abordarán mediante consentimiento informado y anonimización.


# 2. Redacta una propuesta de sistema IA explicable para medicina preventiva.

**Título del proyecto:** Modelo explicable para predicción de riesgo cardiovascular a partir de datos primarios de salud.

**1. Problema:**  
Los modelos de predicción médica suelen ser cajas negras, lo que dificulta su adopción por profesionales. Se busca crear un sistema transparente, basado en árboles de decisión, para evaluar riesgo de eventos cardiovasculares.

**2. Hipótesis:**  
Un modelo interpretable con menos del 10% de variables puede alcanzar precisión superior al 80% manteniendo explicabilidad clínica.

**3. Objetivos:**  
- Entrenar modelos interpretables para predicción binaria (evento/no evento).
- Aplicar técnicas de explicabilidad como SHAP.
- Evaluar la confianza de médicos en las predicciones.

**4. Metodología:**  
- Datos: historial clínico, análisis de sangre, hábitos de vida.
- Modelado: árboles de decisión, regresión logística.
- Técnicas de explicabilidad: SHAP, local feature importance.
- Evaluación: métricas + encuestas a médicos.

**5. Resultados esperados:**  
- Precisión ≥ 82%, recall ≥ 78%.
- Médicos declaran alto grado de comprensión y confianza (>80%).

**6. Conclusión:**  
La explicabilidad es clave para integrar IA en medicina. Este enfoque permite apoyar decisiones clínicas sin sustituirlas.

# 3. Propón un proyecto de IA que utilice agentes inteligentes para coordinar drones en labores de rescate en zonas de desastre natural.

**Título del proyecto:** Sistema multiagente para coordinación autónoma de drones en zonas de desastre.

**1. Problema:**  
La gestión de drones en labores de búsqueda y rescate en zonas afectadas por desastres naturales requiere decisiones rápidas, cobertura eficiente y cooperación entre múltiples dispositivos. Un enfoque basado en agentes inteligentes permitiría distribuir tareas adaptativamente.

**2. Hipótesis:**  
Un sistema multiagente con agentes heterogéneos que utilicen aprendizaje por refuerzo distribuido puede mejorar en al menos un 20% la cobertura de áreas críticas frente a enfoques centralizados.

**3. Objetivos:**  
- Diseñar una arquitectura de agentes para drones autónomos.
- Implementar políticas de coordinación y aprendizaje adaptativo.
- Evaluar cobertura, eficiencia de rutas y tiempo de respuesta.

**4. Metodología:**  
- Simulación en entornos de desastre (forestal, urbano) con REAS definidos.
- Agentes con sensores (visión, temperatura) y actuadores (movimiento, envío de señal).
- Algoritmo de aprendizaje: Deep Q-Learning distribuido.
- Métricas: % de cobertura, tiempo medio por misión, tasa de colisiones.

**5. Resultados esperados:**  
- Mayor eficiencia en cobertura de zonas críticas.
- Capacidad de adaptación a cambios dinámicos del entorno.
- Validación mediante simuladores (ROS + Gazebo).

**6. Conclusión:**  
El enfoque multiagente permite descentralización, redundancia y adaptabilidad. Resulta útil para misiones de alta incertidumbre y requiere supervisión ética y operativa rigurosa para evitar riesgos colaterales.

# 4. Diseña un experimento para evaluar el impacto de un modelo de recomendación de recursos educativos en el rendimiento de estudiantes universitarios.

**Título:** Evaluación de un sistema de recomendación adaptativo en entornos universitarios.

**1. Problema:**  
Los entornos de e-learning suelen ofrecer recursos de forma estática. Un sistema basado en IA puede personalizar contenidos según el perfil del estudiante, mejorando su rendimiento académico.

**2. Hipótesis:**  
Los estudiantes que usan el sistema de recomendación tendrán una mejora promedio del 15% en sus notas en comparación con un grupo control.

**3. Objetivos:**  
- Desarrollar un sistema de recomendación de recursos basado en filtrado colaborativo y perfilado semántico.
- Evaluar su impacto en el desempeño académico.
- Analizar la percepción de utilidad por parte de los usuarios.

**4. Metodología:**  
- Participantes: 100 estudiantes divididos en grupo experimental (con sistema) y control (sin sistema).
- Variables:
  - Independiente: uso del sistema de recomendación.
  - Dependiente: nota final del curso.
  - Intervinientes: motivación, asistencia, nivel previo.
- Algoritmos: KNN + NLP para perfilado semántico.
- Instrumentos: notas, encuestas, registros de interacción.

**5. Resultados esperados:**  
- Mejora estadísticamente significativa en notas.
- Alta percepción de utilidad.
- Identificación de patrones de uso exitosos.

**6. Conclusión:**  
La IA puede aumentar la eficacia del aprendizaje personalizado. El diseño debe considerar la equidad y accesibilidad para evitar favorecer solo a perfiles tecnológicos.
