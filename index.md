# Word Document Generator – Documentation

## Overview

The **Word Document Generator** is a powerful solution that automates the creation of Word using dynamic data and customizable templates. It is designed to empower **business users**—especially in highly regulated sectors like **banking, insurance, and finance**—to manage and format document templates directly in **Microsoft Word**, without constant IT support.

### Key Objectives
- **Automate document creation** to reduce manual editing and errors.
- **Increase compliance** through structured templates.
- **Minimize IT involvement**: Business users can create, edit, and manage templates in Word.
- **Format control**: Users can define string, decimal, and datetime formatting directly in templates.

### Why This Product Exists
Traditional document generation solutions rely heavily on IT departments to implement every formatting change or new document layout. This solution shifts ownership to business users by leveraging **Word’s familiar interface** while allowing templates to be dynamically filled with structured data.

The backend system uses **JSON Schema** to define document types, enabling flexible, validated data inputs. Combined with a **Word Add-in**, the system allows users to bind schema fields to placeholders in Word, apply formatting, and preview results.

### Vision & Roadmap
- **Current**: Available as a Word plugin with a backend deployed via Docker (Azure or on-prem).
- **Future**: Support for **Web-based Office (Office for the Web)** to allow editing templates in the browser. Support for PDF documents.

### Target Industries
This system is ideal for organizations that generate high volumes of client-facing or internal documents:
- **Insurance companies**
- **Banks and financial institutions**
- **Leasing providers and fintechs**

### Common Use Cases
- Claims documents
- Loan agreements
- Invoices and billing plans
- Financial reports
- Customer onboarding forms

### Core Features
- **Word Add-in** UI for template design
- **JSON Schema-based** data binding
- **Dynamic formatting** for dates, numbers, strings
- **REST API** for document generation
- **Authentication via OAuth2** (Azure Entra supported)
- **Support for DOCX**

### Technical Architecture
- **Word Template Designer Add-in** communicates with the **DocGen API**.
- **Templates** are stored on a mounted storage volume (e.g., Azure Files).
- API can be deployed to **Azure Kubernetes Service (AKS)** or on-prem via **Docker**.
- **Authentication**: OAuth2-based, tested with **Azure Entra ID**.
- **CI/CD**: Fully automated deployment via Azure DevOps.

### Technologies Used
- .NET Core (C#)
- Office.js for Word Add-in
- Azure Storage
- Docker & Kubernetes (AKS)
- Refit (for API clients)
- JSON Schema for data validation

### Deployment Options
- **Cloud**: Azure Kubernetes Service (AKS) with Azure Storage
- **On-Premises**: Deploy via Docker with a mounted network volume for templates

### Business Model
- **Enterprise Licensing**
- Closed source: No open-source release is planned

---

## API Usage
[TODO – covered in another section.]

## Code Examples
[TODO – covered in another section.]

## Postman Collection
[TODO – covered in another section.]

---

> ⚠️ This page is automatically generated. For technical inquiries or feature requests, please contact the product team.
