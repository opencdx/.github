<!-- Announcement Banner -->
| [🎉 **OpenCDx v1.0.1 is here** ↓](#releases) |
|--------------------------------|
| Updated libraries, minor feature enhancements, and DX polish across repos.  |


# Getting Started with OpenCDx

## <span style="color: rgba(131,56,138, 1);">OpenCDx — Engineered by Safe Health Systems, Inc.</span>

**Table of Contents**  
*Use the Table of Contents below to quickly navigate through the key sections and repositories of the OpenCDx platform.*  

- [Introduction](#introduction)
  - 🚀 Minimum Installation
- [Repositories Overview](#repositories-overview)
  - [OpenCDx (Backbone)](#1-opencdx-backbone)
  - [OpenCDx GUI](#2-opencdx-gui)
  - [OpenCDx ADR](#3-opencdx-adr)
  - [OpenCDx ADR-gui](#4-opencdx-adr-gui)
  - [OpenCDx UI Library](#5-opencdx-ui-library)
- [Next Steps](#next-steps)
- [Related Links](#related-links)
- [OpenCDx Team Members](#opencdx-team-members)
   
## Introduction

OpenCDx is a comprehensive platform designed for clinical data management, offering secure, scalable, and interoperable solutions across healthcare systems. The OpenCDx ecosystem includes several repositories that work together to streamline data management, enable clinical decision-making, and enhance user experiences.   
   
> **🚀 Minimum Installation**
> 
> To get started, you only need the core **[OpenCDx Repository](https://github.com/opencdx/opencdx)**.

## Repositories Overview
The [OpenCDx Repository](https://github.com/opencdx/opencdx) forms the platform's backbone, providing core backend services, secure clinical data management, and interoperability. The [OpenCDx GUI](https://github.com/opencdx/opencdx-gui) repository enhances this core, adding an administrative dashboard for system configuration and management, along with a client-facing application to facilitate public user interaction. Data collected via **OpenCDx and OpenCDx-GUI** is stored and also extended to the [OpenCDx ADR](https://github.com/opencdx/ADR) repository. Stored data can then be easily queried using [OpenCDx ADR-gui](https://github.com/opencdx/ADR-gui). Additionally, the [OpenCDx UI Library](https://github.com/opencdx/ui-library) ensures visual consistency by providing reusable UI components across all platform interfaces.  

**Below is a breakdown of the repositories under the OpenCDx organization**: 

--- 

### 1. **OpenCDx (Backbone)**

**Repository**: [OpenCDx](https://github.com/opencdx/opencdx)

**Overview**:  
OpenCDx serves as the core platform for managing clinical data in a healthcare environment. It acts as the backbone of the OpenCDx ecosystem, providing the **backend services** for data management, **interoperability**, and **integration** across different healthcare systems. This includes essential backend services and provides a system GUI for service management, along with a Swagger interface for easy API invocation.

**Key Features**:
- **Data Management**: Handles clinical data storage and retrieval.
- **Interoperability**: Ensures seamless communication between systems (e.g., medical devices, EHRs).
- **Core Functionality**: Manages the primary functions related to clinical data such as user access, data flow, system configuration, monitoring, and security.

---

### 2. **OpenCDx GUI**

**Repository**: [OpenCDx GUI](https://github.com/opencdx/opencdx-gui)

**Overview**:  
OpenCDx GUI is the **graphical user interface** for interacting with the OpenCDx platform. It provides a user-friendly interface that allows clinical teams and system administrators to visualize and manage clinical data workflows. OpenCDx-GUI includes an admin dashboard for administrative control and client app to configure interface for the public user.

**Key Features**:
- **Interactive Dashboard**: Centralized view of the OpenCDx system for monitoring and management.
- **Real-Time Data Viewing**: Allows users to interact with live data and clinical workflows.
- **User-Friendly Interface**: Simplifies interaction with complex clinical data.

---

### 3. **OpenCDx ADR**

**Repository**: [OpenCDx ADR](https://github.com/opencdx/ADR)

**Overview**:  
**OpenCDx ADR** serves as a data store for managing clinical data, including **form responses**, **test results**, and **clinical observations**. It allows users to efficiently query and retrieve data, providing a centralized platform for data management and integration.

**Key Features**:
- **Centralized Data Store**: Organizes and stores clinical data to enable easy querying and retrieval.
- **Query Capabilities**: Supports querying of form responses, test results, and other clinical data types in a normalized format.
- **Interoperability**: Facilitates integration with external systems and partners, allowing smooth data exchange and collaboration.
- **Data Management**: Ensures data consistency, security, and scalability for future growth.

---

### 4. **OpenCDx ADR-gui**

**Repository**: [OpenCDx ADR-gui](https://github.com/opencdx/ADR-gui)

**Overview**:  
**OpenCDx ADR-gui** provides a **graphical user interface (GUI)** for interacting with ADR data. This interface enables users to easily build queries and view ADR data in a visual, user-friendly manner.

**Key Features**:
- **Web-Based Interface**: Built using modern technologies like **Next.js** and **React**.
- **Drag-and-Drop Query Builder**: Makes it easy to build queries for interacting with ADR data.
- **Real-Time Query Execution**: Provides immediate feedback when querying ADR records.
- **Docker Support**: Allows for easy deployment of the GUI.

---

### 5. **OpenCDx UI Library**

**Repository**: [OpenCDx UI Library](https://github.com/opencdx/ui-library)

**Overview**:  
The OpenCDx UI Library is a **set of reusable UI components** and **templates** that serve as the foundational design layer for the OpenCDx ecosystem. These components are packaged as a Node.js module and are used across various OpenCDx GUI repositories to ensure consistent and efficient development.

**Key Features**:
- **Reusable Components**: Common UI elements like buttons, forms, and tables.
- **Tailwind CSS Integration**: Ensures responsive design and customization options.
- **Component-Based Architecture**: Provides standardized, modular components for integration across different repositories.

---

## Next Steps

To get started with OpenCDx, follow these steps:

1. **Minimum Installation:** Clone the essential [**OpenCDx Repository**](https://github.com/opencdx/opencdx), which provides core backend services, system GUI, and Swagger interfaces.
2. Optionally, clone other repositories based on your requirements.
3. Follow each repository's README for detailed installation instructions.
4. Integrate and configure components to effectively manage clinical data.

All OpenCDx repositories seamlessly integrate to offer a scalable and efficient solution for clinical data management and healthcare interoperability.

---

## Related Links

Explore additional resources and documentation to deepen your understanding of OpenCDx, its use cases, and the broader ecosystem. Below you'll find helpful links providing more detailed explanations, guides, and background information to support your OpenCDx implementation.

- [OpenCDx Initiative Overview](https://github.com/opencdx/.github/blob/main/README.md)

---

## Releases
<table border="1">
  <tr>
    <th>Tag</th>
    <th>Type</th> 
    <th>Title</th>
    <th colspan="2">OpenCDx Repositories</th>
    <th colspan="2">ADR Repositories</th>
    <th>UI Library</th>
  </tr>
  <tr>
    <td>v1.0.0</td>
    <td>Major Release</td>
    <td>Initial Open Source Release of OpenCDx</td>
    <td><a href="https://github.com/opencdx/opencdx/releases/tag/v1.0.0">opencdx</a></td>
    <td><a href="https://github.com/opencdx/opencdx-gui/releases/tag/v1.0.0">opencdx-gui</a></td>
    <td><a href="https://github.com/opencdx/ADR/releases/tag/v1.0.0">ADR</a></td>
    <td><a href="https://github.com/opencdx/ADR-gui/releases/tag/v1.0.0">ADR-gui</a></td>
    <td><a href="https://github.com/opencdx/ui-library/releases/tag/v1.0.0">ui-library</a></td>    
  </tr>
  <tr>
    <td>v1.0.1</td>
    <td>Minor Release</td>
    <td>Updated librarie and improved developer experience</td>
    <td><a href="https://github.com/opencdx/opencdx/releases/tag/v1.0.1">opencdx</a></td>
    <td><a href="https://github.com/opencdx/opencdx-gui/releases/tag/v1.0.1">opencdx-gui</a></td>
    <td>N/A</td>
    <td>N/A</td>
    <td><a href="https://github.com/opencdx/ui-library/releases/tag/v1.0.1">ui-library</a></td>    
  </tr>  
</table>


---
   
## OpenCDx Team Members   
[Ravinder Singh (rsdeosi@gmail.com)](mailto:rsdeosi@gmail.com)   
[Jeff Miller (jeff.miller@safehealth.me)](mailto:jeff.miller@safehealth.me)   
[Ranga Lakshminarayanan (ranga.lakshminarayanan@safehealth.me)](mailto:ranga.lakshminarayanan@safehealth.me)   
[Patrick Chou (patrick.chou@safehealth.me)](mailto:patrick.chou@safehealth.me)   
[Karthick Rajamurugan (karthick.rajamurugan@safehealth.me)](mailto:karthick.rajamurugan@safehealth.me)   
[Gaurav Mishra (gaurav.mishra@safehealth.me)](mailto:gaurav.mishra@safehealth.me)   


