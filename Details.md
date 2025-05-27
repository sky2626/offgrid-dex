## Built With

Our **OffGrid Dx** mobile application is engineered with a strong emphasis on reliability, performance, and resource efficiency, leveraging the following technologies:

### Languages
* **Dart:** The programming language powering the Flutter framework, chosen for its efficiency, strong typing, and excellent tooling.

### Frameworks & Libraries
* **Flutter:** The UI toolkit used for building natively compiled applications for mobile (Android & iOS) from a single codebase, prioritizing performance and a consistent user experience.
* **Provider** (or **Riverpod** / **Bloc**): For robust state management within the Flutter application, ensuring data consistency and reactivity.
* **GoRouter** (or **auto_route** / **Navigator 2.0**): For declarative and robust routing within the application, managing navigation paths effectively.

### Data Storage & Management
* **SQLite:** The lightweight, embedded relational database used for all on-device, offline data storage. This is critical for storing the comprehensive medical knowledge base, symptom checker logic, patient records, and diagnostic results without requiring internet access.
    * **`sqflite` (Flutter package):** For direct interaction with the SQLite database in Flutter.
    * **`drift` (formerly `moor`):** (Optional, but highly recommended for larger, more complex data models) A reactive persistence library for SQLite, offering compile-time safety and a more structured way to interact with the database.

### AI/ML (For future expansion of diagnostic capabilities)
* **TensorFlow Lite (TFLite):** For deploying highly optimized, lightweight machine learning models directly on the device. This allows for on-device inference for advanced diagnostic pattern recognition without cloud dependency.
    * **`tflite_flutter` (Flutter package):** To integrate and run TFLite models within the Flutter application.

### Communication & Synchronization (For occasional, low-bandwidth data sync)
* **HTTP/HTTPS (with `http` package):** For secure, occasional data synchronization when internet connectivity is available. Focus on efficient data transfer protocols.
* **RESTful API (Backend, if applicable):** A lightweight backend API for receiving anonymized public health data and delivering updates to the knowledge base. (e.g., built with Python/Django, Go, Node.js, etc., on a low-cost server. *Note: The backend itself would be separate from the mobile app's tech stack description, but worth mentioning its interaction.*)
* **JSON:** For data serialization during synchronization.

### Other Technologies & Concepts
* **Git:** For version control.
* **GitHub/GitLab/Bitbucket:** For source code hosting and collaboration.
* **Responsive UI Design:** Principles applied to ensure optimal usability across various mobile screen sizes (smartphones and tablets).
* **Energy-Efficient Coding Practices:** Development focused on minimizing battery consumption through optimized algorithms and UI rendering.
* **Data Compression Algorithms:** Utilized for optimizing the size of the on-device medical knowledge base and for efficient data transfer during synchronization.
