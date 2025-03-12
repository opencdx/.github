# OpenCDx Modules

## Modules
- [OpenCdx Admin](#opencdx-admin)
- [OpenCdx Audit](#opencdx-audit)
- [OpenCdx Classification](#opencdx-classification)
- [OpenCdx Classification Analyzer](#opencdx-classification-analyzer)
- [OpenCdx Client](#opencdx-client)
- [OpenCdx Commons](#opencdx-commons)
- [OpenCdx Communications](#opencdx-communications)
- [OpenCdx Config](#opencdx-config)
- [OpenCdx Discovery](#opencdx-discovery)
- [OpenCdx Gateway](#opencdx-gateway)
- [OpenCdx IAM](#opencdx-iam)
- [OpenCdx Logistics](#opencdx-logistics)
- [OpenCdx Media](#opencdx-media)
- [OpenCdx Proto](#opencdx-proto)
- [OpenCdx Questionnaire](#opencdx-questionnaire)
- [OpenCdx Tinkar](#opencdx-tinkar)

---

### OpenCdx Admin
**Business Feature**:  
Service Discovery and Monitoring   

**Purpose**:  
The OpenCdx Admin module implements a Spring Admin server to support service discovery and monitoring within the OpenCDx platform. It allows different services in the system to find each other and provides tools for monitoring their health and performance.  

**How it Helps:**
- **For system administrators**: Ensures that all services are discoverable, enabling better management of service dependencies and health checks.
- **For monitoring**: Offers a centralized view of the system's status and performance metrics, supporting proactive maintenance and issue resolution.

**Key Features:**
- Spring Admin server for service discovery.
- Health and performance monitoring for system services.

---

### OpenCdx Audit
**Business Feature**:  
Audit Log Management and Event Processing  

**Purpose**:  
The OpenCdx Audit module is responsible for managing audit logs within the OpenCDx ecosystem. It processes audit messages received over the messaging system and transforms them into AuditEvent objects for logging and further analysis.

**How it Helps:**
- **For administrators**: Provides a robust mechanism to track and log all critical events within the system, ensuring compliance with regulatory requirements for auditing and monitoring.
- **For security**: Helps ensure that all actions taken within the system are logged and traceable, allowing for better data governance, security oversight, and forensic investigations if needed.

**Key Features:**
- Receives and processes audit messages using the OpenCDXMessageService.
- Outputs AuditEvents to logs, which can be extended in a production environment to store and process audit data effectively.

---

### OpenCdx Classification
**Business Feature**:  
Data Classification for Clinical Analysis  

**Purpose**:  
The OpenCdx Classification module provides a service to classify clinical data based on user form submissions and test kit images. It enables the system to categorize incoming clinical data, making it easier to analyze and process for healthcare applications.

**How it Helps:**
- **For healthcare providers**: It categorizes clinical data, such as test results or form submissions, into meaningful classifications for easier analysis and faster decision-making.
- **For developers**: Provides a REST API and gRPC services for seamless integration with other OpenCDx modules and external systems, allowing for real-time classification of clinical data.

**Key Features:**
- Classifies clinical data based on form submissions and test images.
- Provides REST API and gRPC services for integration.

---

### OpenCdx Classification Analyzer
**Business Feature**:  
Data Classification and Analysis Engine  

**Purpose**:  
The OpenCdx Classification Analyzer module provides a default analysis engine that supports the classification of clinical data using various algorithms. This engine plays a crucial role in processing clinical data and generating classification results using rules engines, machine learning models, and other classification algorithms.

**How it Helps:**
- **For data scientists and analysts**: It enables the classification of clinical data and supports advanced analytics, helping derive meaningful insights from raw data.
- **For healthcare providers**: It assists in categorizing data based on predefined classifications, streamlining data processing for diagnostic purposes and decision-making.

**Key Features:**
- Implements classification models for clinical data.
- Supports machine learning and rule-based algorithms for classification.

---

### OpenCdx Client
**Business Feature**:  
gRPC Communication for Microservices  

**Purpose**:  
The OpenCdx Client module provides a Spring library that automatically configures services to communicate using gRPC to microservices. This enables OpenCDx services to efficiently interact in a microservice-based architecture, ensuring secure and scalable data exchange across distributed systems.

**How it Helps:**
- **For developers**: Simplifies the integration of services using gRPC in microservices architecture by automatically configuring communication protocols.
- **For system architects**: Facilitates building scalable, efficient, and secure systems where services can communicate asynchronously and reliably.

**Key Features:**
- Automatically configures services to communicate using gRPC.
- Provides a scalable and secure microservices communication setup.

---

### OpenCdx Commons
**Business Feature**:  
Autoconfiguration and Shared Services  

**Purpose**:  
The OpenCdx Commons module enables the autoconfiguration of various OpenCDx components, providing essential shared services and utilities across the platform. This module ensures that common functionalities, like messaging and auditing, are standardized and configured consistently across all modules.

**How it Helps:**
- **For developers**: Simplifies the integration of common services by automatically configuring necessary components, ensuring consistency across different OpenCDx modules.
- **For system administrators**: Provides essential interfaces and services, such as OpenCDXMessageService and OpenCDXAuditService, that ensure smooth communication and auditing within the platform.
- **For security**: The OpenCDXHtmlSanitizer and OpenCDXNationalHealthIdentifier interfaces ensure that data is sanitized and unique identifiers (like health IDs) are generated securely.

**Key Features:**
- OpenCDXMessageService for messaging across modules.
- OpenCDXAuditService for submitting audit messages.
- OpenCDXHtmlSanitizer for sanitizing HTML data.
- OpenCDXNationalHealthIdentifier for generating unique health identifiers.

---

### OpenCdx Communications  
**Business Feature**:  
Secure and Standardized Communication Across Services  

**Purpose**:  
The OpenCdx Communications module facilitates secure, standardized communication between various services within the OpenCDx platform and external systems. It ensures that data exchanged between services follows established protocols and is transmitted securely, maintaining consistency and privacy across different modules of the platform.  

**How it Helps:**  
- **For system administrators**: Ensures that communication between different services within the platform is secure and compliant with the required communication standards, simplifying the management of service integrations.
- **For developers**: Provides an easy-to-use communication layer for integrating different services and systems, allowing them to securely exchange data and interact with each other.
- **For security**: Enforces security standards like encryption and data integrity checks to ensure that the data exchanged between services remains private and untampered.

**Key Features:**  
- Secure communication between OpenCDx services and external systems.
- Support for both REST and gRPC protocols for flexibility in communication.
- Encryption of data both in transit and at rest, ensuring data confidentiality.
- Standardized communication methods to ensure consistency across modules.

---

### OpenCdx Config
**Business Feature**:  
Centralized Configuration Management  

**Purpose**:  
The OpenCdx Config module implements a Spring Configuration Server that provides centralized configuration management for OpenCDx services. It ensures that all services within the OpenCDx ecosystem have access to consistent and secure configuration settings.

**How it Helps:**
- **For system administrators**: Simplifies managing configuration across all services by centralizing the configuration data in one place, enabling easy updates and maintenance.
- **For developers**: Ensures that each service uses a common set of configuration settings, making development and deployment more streamlined.
- **For security**: Provides an API to encrypt sensitive information, ensuring that critical data such as passwords is securely stored and transmitted.

**Key Features:**
- Centralized configuration for all OpenCDx services.
- Encryption API to secure sensitive information used across the system.

---

### OpenCdx Discovery
**Business Feature**:  
Service Discovery for OpenCDx Microservices  

**Purpose**:  
The OpenCdx Discovery module implements Spring Discovery server functionality. It is responsible for enabling services within the OpenCDx platform to discover and communicate with each other dynamically, as well as providing monitoring of these services.

**How it Helps:**
- **For system administrators**: Facilitates the detection of services and helps ensure that microservices can locate each other within the distributed system.
- **For developers**: It simplifies the configuration of microservices by automating the service discovery process, reducing the complexity of manual configurations.

**Key Features:**
- Spring Discovery server for microservice communication.
- Service monitoring to ensure healthy communication between services.

---

### OpenCdx Gateway
**Business Feature**:  
API Gateway for Secure Service Access  

**Purpose**:  
The OpenCdx Gateway module provides a central entry point for accessing all OpenCDx service APIs. It manages secure, standardized communication between external applications and the platform’s internal services, enabling both RESTful and gRPC communication.

**How it Helps:**
- **For developers**: Simplifies the integration of external applications with OpenCDx by providing a single gateway for API access.
- **For system administrators**: Ensures centralized management and monitoring of all incoming API requests, improving security and scalability.

**Key Features:**
- Supports REST API and gRPC communication.
- Dockerized for easy deployment and scalability.

---

### OpenCdx IAM
**Business Feature**:  
Identity and Access Management for OpenCDx Services  

**Purpose**:  
The OpenCdx IAM module provides the identity and access management service for the OpenCDx platform. It enables the creation, modification, deletion, and retrieval of user profiles, organizations, workspaces, and providers within OpenCDx.

**How it Helps:**
- **For system administrators**: It ensures secure user management by creating system and regular user profiles, enabling role-based access control across OpenCDx services.
- **For security**: Facilitates authentication and authorization, ensuring that only authorized users have access to OpenCDx services.

**Key Features:**
- Supports REST and gRPC APIs for managing users, including user creation, password management, and login operations.
- Defines various user types: system users, regular users, and trial users, with different permissions and statuses.

---

### OpenCdx Logistics
**Business Feature**:  
Shipping and Delivery Tracking  

**Purpose**:  
The OpenCdx Logistics module is responsible for managing and tracking deliveries within the OpenCDx platform. It handles various logistics-related processes, including the tracking of delivery IDs, order statuses, timestamps, and other shipping details.

**How it Helps:**
- **For logistics teams**: It tracks the journey of clinical data and supplies, providing real-time updates and managing the delivery process efficiently.
- **For healthcare providers**: It helps ensure that clinical data or medical products are delivered securely and on time.

**Key Features:**
- Delivery tracking with information such as current location, recipient, and delivery status.
- Integration with Docker for easy deployment.
- REST API and gRPC interfaces for communication with external systems.

---

### OpenCdx Media
**Business Feature**:  
Media File Handling and Storage  

**Purpose**:  
The OpenCdx Media module is designed for managing media files (such as images, videos, or audio) within the OpenCDx platform. It provides the necessary infrastructure for uploading, storing, and retrieving media files, which are essential in clinical data contexts (e.g., medical imaging or patient records).

**How it Helps:**
- **For healthcare providers**: Allows for the secure storage and retrieval of media files associated with patient records, ensuring easy access to relevant multimedia data.
- **For developers**: Implements a file storage service interface that can be extended to use different storage backends, such as local file systems or cloud storage solutions.

**Key Features:**
- OpenCDXFileStorageService interface for file storage management.
- Dockerized service for media handling, ensuring scalability and easy deployment.
- REST API and gRPC endpoints for communication with other systems.

---

### OpenCdx Proto
**Business Feature**:  
Protocol Buffers for gRPC Communication  

**Purpose**:  
The OpenCdx Proto module is used to generate gRPC services from Protobuf files. These generated services form the communication layer for the OpenCDx platform, enabling secure and efficient communication between services through standardized protocols.

**How it Helps:**
- **For developers**: Simplifies the integration of gRPC-based communication by generating the necessary service files and APIs directly from Protobuf definitions.
- **For system architects**: Ensures consistency in the data models and communication structures used across the OpenCDx platform, facilitating seamless interaction between microservices.

**Key Features:**
- Generates gRPC services from Protobuf files.
- Ensures consistency in data communication and interoperability across OpenCDx services.

---

### OpenCdx Questionnaire
**Business Feature**:  
Clinical Data Collection via Questionnaires  

**Purpose**:  
The OpenCdx Questionnaire module is designed for creating and managing questionnaires used to collect clinical data. It provides both REST API and gRPC services to enable the display of forms, data collection from users, and management of patient surveys, assessments, or other forms of clinical data intake.

**How it Helps:**
- **For healthcare providers**: Facilitates the structured collection of patient data through questionnaires, ensuring that the data is standardized and ready for integration with other healthcare systems.
- **For developers**: Provides an easy-to-integrate service that handles questionnaire management and data collection within clinical applications.

**Key Features:**
- Supports REST API and gRPC for form handling and data collection.
- Dockerized for easy deployment and scalability.

---

### OpenCdx Tinkar
**Business Feature**:  
Data Analysis and Machine Learning Integration  

**Purpose**:  
The OpenCdx Tinkar module interfaces with the Tinkar platform, which supports data analysis and machine learning operations. It is designed to gather the necessary data for running machine learning models and generating insights from clinical datasets.

**How it Helps:**
- **For data scientists**: It enables seamless integration of machine learning models within the OpenCDx platform, providing the tools required to analyze clinical data.
- **For healthcare providers**: Supports advanced analytics that can improve clinical decision-making by extracting actionable insights from clinical data.

**Key Features:**
- Provides REST API and gRPC interfaces for accessing the Tinkar service.
- Dockerized for easy deployment and scalable use in cloud or on-premises environments.
- Interfaces with Tinkar’s database to process and analyze data efficiently.

