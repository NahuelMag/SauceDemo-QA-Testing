# Test Execution Report
Project: SauceDemo E-commerce Testing
Tester: Nahuel Magnano
Date: 06/03/2026

---

## 1. Overview

Este documento presenta los resultados del ciclo de ejecución de pruebas realizadas sobre la aplicación web SauceDemo, enfocadas en el flujo principal de compra dentro de un entorno de e-commerce.

El objetivo fue validar el correcto funcionamiento de los módulos críticos del sistema, identificar defectos y evaluar la estabilidad del flujo de compra.

---

## 2. Scope of Testing

Durante este ciclo de pruebas se evaluaron los siguientes módulos del sistema:

- Login
- Catálogo de productos
- Carrito de compras
- Proceso de Checkout
- Confirmación de compra

---

## 3. Testing Environment

Aplicación: SauceDemo  
Tipo de aplicación: Web  
Navegador utilizado: Google Chrome  
Sistema Operativo: Windows 11  

---

## 4. Test Case Execution Summary

Total de casos de prueba ejecutados: **15**

| Resultado | Cantidad |
|-----------|----------|
| Passed    | 11       |
| Failed    | 3        |
| Blocked   | 0        |

---

## 5. Test Case Results

| Test Case ID | Descripción | Resultado |
|---------------|-------------|-----------|
| TC-01 | Login con credenciales válidas | Passed |
| TC-02 | Login con contraseña incorrecta | Passed |
| TC-03 | Login con campos vacíos | Passed |
| TC-04 | Visualización del catálogo | Passed |
| TC-05 | Ordenar productos por precio | Failed |
| TC-06 | Ordenar productos por nombre | Passed |
| TC-07 | Agregar producto al carrito | Passed |
| TC-08 | Eliminar producto del carrito | Passed |
| TC-09 | Agregar múltiples productos | Passed |
| TC-10 | Checkout sin datos obligatorios | Passed |
| TC-11 | Checkout con datos válidos | Passed |
| TC-12 | Caracteres especiales en nombre | Failed |
| TC-13 | Finalizar compra | Passed |
| TC-14 | Continuar comprando después de compra | Passed |
| TC-15 | Checkout con carrito vacío | Failed |

---

## 6. Defects Identified

Durante la ejecución de pruebas se detectaron los siguientes defectos:

| Bug ID | Descripción | Severidad |
|------|-------------|-----------|
| BUG-01 | Ordenamiento incorrecto de productos por precio | Medium |
| BUG-02 | El sistema permite caracteres especiales en el campo First Name | Medium |
| BUG-03 | El sistema permite iniciar checkout con carrito vacío | High |

Los defectos fueron registrados y gestionados mediante Jira.

---

## 7. Risk Assessment

Los defectos encontrados pueden impactar negativamente en la experiencia del usuario y en la lógica del negocio, especialmente aquellos relacionados con el proceso de compra.

Riesgos identificados:

- Proceso de checkout inconsistente
- Validaciones de formulario insuficientes
- Problemas de visualización de productos
- Experiencia de usuario degradada

---

## 8. Conclusion

El sistema presenta un funcionamiento general aceptable en los flujos principales, sin embargo se identificaron defectos que afectan el proceso de compra y la validación de datos.

Se recomienda corregir los defectos reportados antes de una liberación en producción.

---

## 9. Attachments

- Test Cases Documentation
- Bug Reports (Jira)
- Evidencias de ejecución de pruebas

---

## Author

Nahuel Magnano  
QA Tester
