//Test Automation Framework (Java + Selenium + Cucumber + JUnit)

Este repositorio contiene un framework base para pruebas automatizadas utilizando:

-  **Java 17**
-  **Selenium 4**
-  **Cucumber (BDD)**
-  **JUnit 4**
-  **Maven**
-  Integración con **Jenkins**
-  Compatible con **Bitbucket/GitHub** y pipelines de CI/CD

---

// Características

- Estructura modular y limpia
- Soporte para **pruebas BDD** con archivos `.feature`
- Ejecución de pruebas con **JUnit y Maven**
- Soporte para **Page Object Model** (se puede expandir fácilmente)
- Generación de **reportes HTML** de Cucumber
- Preparado para integración continua con **Jenkins**

---

// Estructura del proyecto

```
src/
├── main/java/              # (opcional) Clases auxiliares
└── test/java/
    ├── stepDefinitions/    # Definiciones de pasos de Cucumber
    └── runner/             # Clase TestRunner con configuración
resources/
└── features/               # Escenarios en formato Gherkin
```

---

// Cómo ejecutar las pruebas

```bash
# Ejecutar pruebas con Maven
mvn clean test
```

---

// Jenkinsfile

Incluye un `Jenkinsfile` básico con las siguientes etapas:

1. Checkout desde Bitbucket
2. Instalación de dependencias con Maven
3. Ejecución de pruebas automatizadas
4. Publicación de resultados (`.xml` para Jenkins)

---

// Requisitos

- Java 17+
- Maven 3.9+
- ChromeDriver configurado en el `PATH` del sistema
- Jenkins (opcional)
