```mermaid
flowchart TD
    A[User opens app] --> B[Select exercise from library]
    B --> C[Camera activates & MediaPipe tracks pose]
    C --> D[User performs exercise]
    D --> E[App analyzes movement in real-time]
    E --> F[Provide feedback on posture, reps, and correctness]
    F --> G[End session & log performance]
    G --> H[Option to view history or repeat exercise]

    %% Error handling
    C --> I[Camera not accessible?]
    I --> J[Show error: enable camera permission]
    C --> K[MediaPipe tracking fails?]
    K --> L[Show guidance to reposition user]
