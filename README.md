# AI GIS Reporting App

A mobile-first web application for reporting public infrastructure and utility issues using AI and GIS integration.

---

## Overview

This project demonstrates how a simple user interaction can be transformed into structured geospatial data.

A user captures a utility or infrastructure issue using their phone camera, AI analyzes the image, the user can refine the result if needed, and the final report is stored as a geographic point in ArcGIS Online.

👉 From photo to map, in just a few steps.

The application is fully deployed and works as a live web app.

---

## Why this project exists

The goal was not to build a complex system, but to explore a practical connection between AI and GIS through a clean and realistic user experience.

Instead of focusing on features, the emphasis was on:

- simplicity of interaction  
- minimal user effort  
- realistic mobile behavior  
- reliable classification  
- structured geospatial output  

This approach ensures that the app feels closer to a real product than a technical demo.

---

## How it works

The application follows a simple and intuitive flow:

1. The app opens directly in camera mode  
2. The user captures a photo of a public infrastructure issue  
3. The system requests:
   - camera permission  
   - location permission  
4. AI analyzes the image  
5. The app proposes an issue classification  
6. The user can optionally add clarification  
7. AI refines or confirms the result  
8. The report is submitted and stored in ArcGIS Online  

---

## Deployment

The application is deployed using Vercel, enabling:

- serverless backend functions  
- seamless integration with GitHub  
- automatic deployment on every push  

This setup allows the app to run as a fully functional online service, not just a local prototype.

---

## Architecture

The system is built as a lightweight pipeline connecting three layers:

### Frontend
- Camera access (browser API)  
- Geolocation (background capture)  
- UI and interaction logic  

### AI Layer
- Image analysis  
- Controlled classification  
- Clarification handling  

### GIS Layer
- ArcGIS Online Feature Layer  
- Stores and visualizes reported issues  

Data flow:

User → Camera → AI → Validation → ArcGIS → Map

---

## AI behavior and constraints

The AI is intentionally constrained to ensure reliability.

Supported issue types include:

- pothole  
- garbage  
- graffiti  
- broken_light  
- damaged_sign  
- water_leak  
- sidewalk_damage  
- fallen_tree  

Special categories:
- no_issue  
- unknown  

Key rules:

- classification must be based on visible evidence  
- indoor or private scenes are ignored  
- user clarification can refine, but not override visual context  

This ensures that reported data remains consistent and usable in GIS.

---

## Data handling

Each report contains:

- issue_type  
- description  
- latitude  
- longitude  
- gps_accuracy  
- timestamp  

Location is captured in the background and is not displayed to the user.

Coordinates are stored with high precision, while accuracy represents the uncertainty radius in meters.

---

## UX approach

A major part of the project focused on improving user experience rather than adding complexity.

Key principles:

- no unnecessary steps  
- no technical messages exposed to users  
- minimal interface  
- fast interaction flow  
- mobile-first design  

The clarification step was redesigned into a lightweight AI interaction, visually similar to messaging apps:

- user input on one side  
- AI response on the other  

This creates a more natural interaction without turning the app into a full chatbot.

---

## Use cases

This concept can be applied in multiple real-world scenarios:

- municipalities and city services  
- smart city platforms  
- infrastructure maintenance systems  
- utilities monitoring (water, electricity, roads)  
- citizen reporting platforms  

The strength of the system lies in converting unstructured input (images) into structured geospatial data.

---

## Challenges and decisions

Several important challenges shaped the final solution:

- balancing simplicity and functionality  
- reducing UI clutter without losing clarity  
- controlling AI behavior to avoid incorrect classifications  
- keeping the system stable while improving UX  
- ensuring frontend and GIS layers remain synchronized  

The key principle throughout development was:

👉 improve the experience without breaking the system

---

## Current state

The application currently supports:

- automatic camera start  
- image capture and preview  
- background geolocation  
- AI-based image classification  
- optional clarification flow  
- controlled issue taxonomy  
- ArcGIS Online integration  
- bilingual interface (Serbian and English)  

---

## Cost considerations

The project is designed as a low-cost MVP.

Main components:

- AI usage based on API calls  
- serverless backend  
- ArcGIS Online integration  

Costs are controlled by:

- limiting the number of AI requests  
- using a single-pass analysis approach  
- avoiding unnecessary processing  

---

## Key insight

This project is not just a UI concept.

It represents a working pipeline that connects:

- user input  
- AI interpretation  
- user validation  
- geospatial systems  

---

## Next steps

Potential future improvements include:

- in-app map preview  
- improved success feedback  
- visualization by issue type  
- clustering and filtering  
- image storage  
- advanced analytics  

---

## Summary

The project shows how a simple mobile interaction can become structured, location-aware data through AI and GIS integration.

The focus was not on complexity, but on clarity:

- simple flow  
- controlled AI  
- meaningful output  
- real-world usability  
