# Flip2Fit – Use Cases

## Use Case 1: Perform an Exercise

**Actor:** User  
**Goal:** Complete an exercise and receive real-time feedback.  

**Preconditions:**  
- User has installed the app and opened it.  
- User has selected an exercise from the library.  
- Camera permission has been granted.

**Main Flow:**  
1. User selects an exercise from the library.  
2. App activates the camera and MediaPipe pose tracking.  
3. User performs the exercise in front of the camera.  
4. App analyzes user movements in real-time.  
5. App provides feedback on posture, repetitions, and correctness.  
6. Exercise session ends, and performance is logged.

**Alternative Flows:**  
- If the camera cannot be accessed, the app shows an error and suggests granting permissions.  
- If MediaPipe cannot detect movements properly, the app shows guidance for proper positioning.

---

## Use Case 2: Track Exercise History

**Actor:** User  
**Goal:** View past exercise sessions and monitor progress.  

**Preconditions:**  
- User has completed at least one exercise session.  

**Main Flow:**  
1. User navigates to the “History” or “Progress” section.  
2. App displays past sessions with dates, exercises performed, and feedback summaries.  
3. User can select a session to see detailed performance metrics (e.g., posture correctness, repetitions).  

**Alternative Flows:**  
- If no past sessions exist, the app displays a message encouraging the user to start exercising.

---

## Use Case 3: Adjust Exercise Settings

**Actor:** User  
**Goal:** Modify exercise difficulty or duration.  

**Preconditions:**  
- User is logged in (if multi-user profiles are supported).  
- Exercise has adjustable settings.  

**Main Flow:**  
1. User selects an exercise.  
2. User opens “Settings” for the exercise.  
3. User adjusts difficulty, duration, or repetitions.  
4. App saves settings for future sessions.  

**Alternative Flows:**  
- If settings cannot be saved (e.g., storage issue), app displays an error and allows retry.

---

## Use Case 4: Receive Notifications/Reminders

**Actor:** User  
**Goal:** Receive reminders to exercise regularly.  

**Preconditions:**  
- User has enabled notifications in the app.  

**Main Flow:**  
1. App schedules reminders based on user preferences (time of day, frequency).  
2. At the scheduled time, app sends a notification.  
3. User taps the notification to open the app and perform an exercise.  

**Alternative Flows:**  
- If notifications are blocked by the system, app shows a warning with instructions to enable them.

---

## Use Case 5: Manage User Profiles(Optional)

**Actor:** User  
**Goal:** Create or switch between multiple profiles.  

**Preconditions:**  
- App supports multi-user profiles.  

**Main Flow:**  
1. User opens the “Profiles” section.  
2. User creates a new profile or selects an existing one.  
3. App loads personalized exercise settings and history.  

**Alternative Flows:**  
- If the profile cannot be saved, app displays an error and allows retry.  

