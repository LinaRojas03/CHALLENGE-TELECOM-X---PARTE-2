# 📊 Predicción de Cancelación de Clientes (Churn Prediction) – Telecom X

Este proyecto tiene como objetivo predecir la **cancelación de clientes** en una empresa de telecomunicaciones utilizando **Machine Learning**.  
Se implementan y comparan dos modelos: **Regresión Logística** y **Random Forest**, analizando su rendimiento y las variables más relevantes que influyen en la cancelación.

---

## 📂 Contenido del Repositorio

- `notebooks/TelecomX2_LATAM.ipynb` → Cuaderno principal con el análisis, preprocesamiento de datos, entrenamiento de modelos y evaluación.
- `data/` → Carpeta con los datos de entrada (dataset original y procesado).
- `README.md` → Documento de referencia y guía de uso.

---

## 🚀 Instalación y Ejecución

### Clonar el repositorio
```bash
git clone https://github.com/tu_usuario/telecom-churn-prediction.git
cd telecom-churn-prediction
```

---

## 📊 Ejecución del Código

El análisis y los modelos se ejecutan desde el cuaderno de Google Colaboratory o Jupyter Notebook.

1. Abrir el archivo notebooks/analisis_churn.ipynb.
2. Ejecutar las celdas en orden:
   - Carga de datos
   - Limpieza y preprocesamiento
   - Entrenamiento de modelos
   - Evaluación y comparación de métricas
   - Análisis de importancia de variables
3. Visualizar resultados y conclusiones.

---

## 📈 Modelos Implementados

Se entrenaron y compararon dos modelos:

| Modelo                  | Exactitud | Precisión | Recall | F1-score |
| ----------------------- | --------- | --------- | ------ | -------- |
| **Regresión Logística** | 0.7689    | 0.5393    | 0.6979 | 0.6084   |
| **Random Forest**       | 0.7902    | 0.6169    | 0.4866 | 0.5441   |}

- Regresión Logística: Mejor recall, lo que significa que detecta más clientes propensos a cancelar.
- Random Forest: Mejor precisión y exactitud, aunque detecta menos clientes en riesgo.

---

## 🔍 Variables Más Relevantes

### 📌 Top 5 Regresión Logística

> customer.tenure (antigüedad del cliente) → Coef. negativo, a mayor tiempo, menor probabilidad de cancelación. <br>
> account.Contract_Two year → Contratos largos reducen la cancelación. <br>
> internet.InternetService_Fiber optic → Mayor probabilidad de cancelación. <br>
> account.PaymentMethod_Electronic check → Mayor probabilidad de cancelación. <br>
> account.Contract_One year → Disminuye cancelación.

### 📌 Top 5 Random Forest

> customer.tenure <br>
> account.Charges.Monthly <br>
> account.PaymentMethod_Electronic check <br>
> internet.TechSupport_Yes <br>
> internet.OnlineSecurity_Yes

---

## 💡Estrategias de Retención Propuestas

- Fidelizar clientes nuevos: Programas de permanencia y descuentos para los primeros meses.
- Ofrecer soporte técnico proactivo: Clientes con servicios de soporte y seguridad cancelan menos.
- Incentivar contratos largos: Planes de 1 o 2 años con beneficios adicionales.
- Revisar servicio de fibra óptica: Altas tasas de cancelación podrían indicar problemas de calidad o precios.
- Analizar método de pago “Electronic check”: Posibles problemas de cobro o experiencia de pago.

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas!
Puedes abrir un issue o enviar un pull request para proponer mejoras.

