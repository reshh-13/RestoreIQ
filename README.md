#  RestoreIQ – AI-Powered Artifact Conservation and Restoration Management System
**Preserving History Through Intelligent Technology.**

##  About the Project

RestoreIQ is an AI-powered artifact conservation and restoration management system developed using **Zoho Creator, Zoho CRM, and Deluge scripting**.

The system is designed to simplify artifact management and restoration activities within a museum. It provides a centralized platform for registering artifacts, assessing their condition, identifying artifacts requiring restoration, assigning conservation specialists, and maintaining restoration records.

By integrating AI-based image classification with workflow automation, RestoreIQ helps streamline the artifact conservation process and reduces the need for manual coordination.

##  Key Features

- **Artifact Registration:** Register and maintain artifact information in a centralized system.
- **AI-Powered Damage Detection:** Analyze uploaded artifact images using Zoho Creator's Object Detection model.
- **Automated Classification:** Classify artifacts into `Normal` and `Restore` categories.
- **Damage Assessment:** Allow employees to upload artifact images and submit assessment notes.
- **Employee Management:** Retrieve employee information from Zoho CRM using Employee ID.
- **Specialist Management:** Register and manage conservation specialists.
- **Restoration Task Assignment:** Allow administrators to assign restoration tasks to specialists.
- **Automated Notifications:** Generate restoration alerts in Zoho CRM and trigger email notifications to assigned specialists.
- **Restoration History:** Maintain records of restoration activities, materials used, remarks, completion dates, and before-and-after images.
- **Calendar Integration:** Integrate restoration scheduling with Zoho Calendar.

##  Technology Stack

| Technology | Purpose |
| Zoho Creator | Main application and form management |
| Zoho CRM | Employee data, specialist contacts, and restoration alerts |
| Deluge Script | Workflow automation and application logic |
| Zoho Creator Object Detection | AI-based image classification |
| Zoho Calendar API | Restoration scheduling integration |


### Zoho Creator – Main Application

The application consists of five primary forms:

1. **Artifact Registration** – Stores artifact details.
2. **Damage Assessment** – Records employee assessments, uploaded images, and AI classification results.
3. **Specialist Registration** – Maintains conservation specialist information.
4. **Restoration Task** – Manages restoration assignments.
5. **Restoration History** – Stores completed restoration details, materials, remarks, and before-and-after images.

### Zoho CRM – Supporting Application

The CRM integration contains three modules:

1. **Employees (Custom Module)** – Stores employee information such as name, email, and department.
2. **Contacts (Standard Module)** – Maintains specialist contact information.
3. **Restoration Alerts (Custom Module)** – Stores restoration assignment notifications.

##  AI Integration

RestoreIQ uses the **Zoho Creator Object Detection model** to classify uploaded artifact images.

The AI processing workflow is:

1. An employee selects a registered artifact.
2. An image of the artifact is uploaded.
3. The Object Detection model analyzes the image.
4. The model generates a classification: `Normal` or `Restore`.
5. The result is recorded in the Damage Assessment form.
6. Artifacts classified as `Restore` are flagged for administrator review.

The classification supports the initial assessment process. Restoration decisions require appropriate human review.

##  System Workflow

```text
Artifact Registration
        ↓
Employee Submits Damage Assessment
        ↓
Artifact Image Upload
        ↓
AI-Based Image Classification
        ↓
   Normal / Restore
        ↓
Admin Reviews Flagged Assessment
        ↓
Creates Restoration Task
        ↓
Assigns Conservation Specialist
        ↓
CRM Restoration Alert
        ↓
Automated Email Notification
        ↓
Restoration Activity
        ↓
Restoration History Updated
```

##  User Roles

- **Administrator:** Manages artifacts, specialists, assessment reviews, and restoration task assignments.
- **Employee:** Submits damage assessments, uploads artifact images, and adds notes.
- **Conservation Specialist:** Handles assigned restoration activities and updates restoration history.


##  Developed By
**Reshma S**  
