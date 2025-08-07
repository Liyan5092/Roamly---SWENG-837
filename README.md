# Roamly – Generative AI Travel Itinerary Planner

Roamly is an AI-powered travel itinerary planner that allows users to generate, edit, and export multi-day travel plans based on their preferences. This system is designed using clean software architecture principles, with strong emphasis on maintainability, scalability, and modular design.

---

## 📌 Project Highlights

- Built using **Blazor** for Web, **.NET MAUI** for Mobile, and **Azure Cloud** for deployment.
- Uses **Generative AI** for smart itinerary generation via an external AI model.
- Designed with **GRASP, SOLID, and GoF patterns** to ensure clean separation of concerns and flexible extensibility.

---

## 🧠 Problem Statement

Modern travelers want personalized trip plans without manually researching every destination. Roamly simplifies that process by letting users input their preferences and instantly receive a tailored itinerary powered by AI.

---

## 🧩 UML Diagrams & Design Components

| Diagram | Description |
|--------|-------------|
| **Use Case Diagram** | Identifies all actors (RegisteredTraveler, GuestTraveler, Admin) and their interactions (e.g., generate itinerary, export, give feedback). |
| **Activity Diagram** | Shows step-by-step flow of itinerary generation, including input collection, AI processing, and export flow. |
| **Sequence Diagrams** | Models how components interact to generate and edit saved itineraries. |
| **Domain Model** | Visualizes core concepts like User, Itinerary, DayPlan, and TravelPreferences. |
| **Class Diagram** | Details attributes and methods of all classes (ItineraryService, FeedbackService, etc.). |
| **State Machine Diagram** | Tracks the lifecycle of an Itinerary (draft → generated → saved → exported). |
| **Component Diagram** | Shows internal architecture: Client apps, Application services, External APIs, and DBs. |
| **Deployment Diagram** | Depicts how components are deployed on Azure using App Services, Databases, AI endpoints, and Monitoring tools. |

> 🗂️ All `.txt` plant uml scripts are in the `/Scripts` folder and rendered visuals are in `/Images`.

---

## 🎯 Design Principles & Patterns

- **GRASP**: Controller (service layer), Creator (Itinerary creates DayPlan), Low Coupling/High Cohesion.
- **SOLID**: SRP, OCP, LSP, DIP applied across domain and application services.
- **GoF Patterns**: Strategy (AI generation modes), Observer (monitoring), Factory Method (dynamic itinerary types), Facade (simplified services).
- **Microservices Best Practices**: Service decomposition, API Gateway via Azure App Service, Monitoring with App Insights.

More detailed explanations are available in the **Design Patterns** section of the documentation and video.

---

## 🎥 Video Presentation

🎞️ Slides: [PowerPoint](Powerpoint/Roamly_Presentation.pptx)

---

## 🛠️ Tech Stack

- **Frontend**: Blazor (.NET), .NET MAUI
- **Backend**: .NET 8, C#, Web API
- **Cloud**: Azure App Services, Azure Monitor, Azure Blob Storage
- **AI Integration**: External model endpoint (e.g., Azure OpenAI or HuggingFace)

---

## ✅ How to Navigate This Repo

- View rendered UML diagrams in `/images`
- Modify diagram source in `/scripts`
- Read the full PDF documentation in `/word`
- Watch the design walkthrough in `/video`
- Clone or fork to test architecture or code

---

## 📃 License

This project is released under the MIT License.
