# Flip2Fit – Requirements Analysis

## 1. Project Overview
**Project Name:** Flip2Fit  
**Type:** Cross-platform mobile application  
**Purpose:** Help users exercise more effectively by analyzing their movements using the phone camera and providing real-time feedback.  

**Key Features:**  
- Uses **Google MediaPipe API** for motion tracking.  
- Detects and analyzes exercise movements (e.g., squats, push-ups, lunges).  
- Provides **real-time feedback** on posture, repetitions, and performance.  
- Works on **iOS and Android** devices.  

---

## 2. Functional Requirements

| ID  | Requirement | Description |
|-----|------------|-------------|
| FR1 | Camera access | The app must access the device camera to track user movements. |
| FR2 | Exercise detection | The app must detect different types of exercises using MediaPipe. |
| FR3 | Movement analysis | The app must analyze user posture, angles, and repetitions. |
| FR4 | Feedback system | The app must provide feedback on correctness, form, and performance. |
| FR5 | Exercise logging | The app must log user performance and history for progress tracking. |
| FR6 | User profiles | The app must allow multiple users with personalized exercise settings. |
| FR7 | Exercise library | The app must provide a library of exercises with instructions. |
| FR8 | Notifications | The app must remind users to perform exercises regularly. |

---

## 3. Non-Functional Requirements

| ID  | Requirement | Description |
|-----|------------|-------------|
| NFR1 | Cross-platform | The app must run on both iOS and Android devices. |
| NFR2 | Performance | Real-time analysis must occur with minimal delay (<1s). |
| NFR3 | Security | User data must be stored securely and comply with privacy regulations. |
| NFR4 | Usability | The UI should be intuitive, clear, and responsive for all user levels. |
| NFR5 | Reliability | The app must handle camera access failures gracefully. |
| NFR6 | Maintainability | Code should be modular and well-documented for future updates. |

---

## 4. Technical Requirements

- **Framework:** React Native / Flutter (for cross-platform support)  
- **Motion Analysis:** Google MediaPipe (Pose/Hand tracking APIs)  
- **Backend:** Optional (for cloud storage, logging, or user accounts)  
- **Data Storage:** Local device storage (SQLite or similar)  
- **Third-party Libraries:** Camera access, UI components, analytics  

---

## 5. User Requirements

- User must be able to **select exercises** from the library.  
- User must see **real-time feedback** while performing exercises.  
- User must be able to **track progress** over time.  
- User must have the option to **adjust exercise difficulty** or duration.  
- User must have **privacy control** over any stored data.  
