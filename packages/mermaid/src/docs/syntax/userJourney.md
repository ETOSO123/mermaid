# User Journey Diagram

> User journeys describe at a high level of detail exactly what steps different users take to complete a specific task within a system, application or website. This technique shows the current (as-is) user workflow, and reveals areas of improvement for the to-be workflow. (Wikipedia)

Mermaid can render user journey diagrams:

```mermaid-example
journey; A[Despertar] --> B[Escoger el atuendo]; B --> C[Ir al baño]; C --> D{¿Desayunar?}; D -->|Sí| E[Preparar desayuno]; D -->|No| F[Saltar desayuno]; E --> G[Desayunar]; F --> G; G --> H[Vestirse y organizarse]; H --> I{¿Cargar maletín?}; I -->|Sí| J[Preparar maletín]; I -->|No| L[No llevar maletín]; J --> K[Coger maletín]; L --> K; K --> M[Coger el transporte]; M --> N[Salir de casa]; N --> O[Iniciar labor a la hora indicada]; O --> P{¿Enfocarse en cada una de las actividades?}; P -->|Sí| Q[Trabajar con eficiencia]; P -->|No| R[Tomar un descanso]; Q --> S[Reportar novedades]; R --> S;
```

Each user journey is split into sections, these describe the part of the task
the user is trying to complete.

Tasks syntax is `Task name: <score>: <comma separated list of actors>`
