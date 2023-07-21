```mermaid
    graph TD;
        style A fill:#9FD8D8, stroke:#333, stroke-width:2px, stroke-dasharray: 5, 5, shape:rect
        style B fill:#AED581, stroke:#333, stroke-width:2px, stroke-dasharray: 5, 5, shape:round-rectangle
        style C fill:#FFD54F, stroke:#333, stroke-width:2px, stroke-dasharray: 5, 5, shape:round-rectangle
        style D fill:#AED581, stroke:#333, stroke-width:2px, shape:round-rectangle
        style E fill:#F0BB5E, stroke:#333, stroke-width:2px, shape:parallelogram
        style F fill:#F0BB5E, stroke:#333, stroke-width:2px, shape:parallelogram
        style G fill:#F0BB5E, stroke:#333, stroke-width:2px, shape:parallelogram
        style H fill:#9FD8D8, stroke:#333, stroke-width:2px, shape:rect

        A[Dépôt GitHub] --> B[Configuration du webhook]
        B --> C[Événement détecté]
        C --> D[Notification envoyée au webhook]
        D --> E[Jenkins (URL : https://example-jenkins.com/webhook)]
        E --> F[Traitement de la notification]
        F --> G[Déclenchement des jobs (tâches)]
        G --> H[Exécution des jobs]
```