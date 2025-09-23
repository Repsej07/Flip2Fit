# Flip2Fit – Testing Documentation

## 1. Overview
Testing ensures that Flip2Fit works correctly across devices, exercises, and use cases.  
This includes **unit tests**, **integration tests**, and **manual testing** for camera-based motion analysis and real-time feedback.

---

## 2. Unit Testing
**Purpose:** Test individual modules and functions to ensure they behave as expected.  

### Modules to Test:
1. **Exercise Detection**
   - Verify correct exercise type is identified from input data.
2. **Movement Analysis**
   - Check angle calculations, posture correctness detection, and repetition counting.
3. **Feedback System**
   - Ensure correct feedback messages are generated for different movement errors.
4. **User Profile Management**
   - Test creation, deletion, and switching of profiles.
5. **Settings & Notifications**
   - Validate saving/loading of exercise settings and scheduled notifications.

### Example Tools:
- **Flutter:** flutter_test  
- **Data calculations:** Pure unit tests with mocks for MediaPipe output
---

## 3. Integration Testing
**Purpose:** Ensure that combined modules work together as expected.

### Key Integration Flows:
1. **Camera → MediaPipe → Feedback**
   - Test if live camera input is correctly processed by MediaPipe.  
   - Validate that feedback corresponds accurately to movements.
2. **Exercise Session → Logging → History**
   - Ensure session data is stored locally and displayed in history.
3. **Profile Management + Settings**
   - Validate switching profiles updates exercise preferences and history correctly.

### Tools & Approach:
- Use device simulators/emulators for iOS and Android.  
- Mock camera input for automated testing of MediaPipe processing.  
- Optional: Appium for cross-platform automated integration tests.

---

## 4. Manual Testing
**Purpose:** Verify real-world usability and camera-based tracking.

### Test Scenarios:
1. **Exercise Execution**
   - User performs each exercise and verifies real-time feedback.  
   - Test in various lighting conditions and camera angles.
2. **Error Handling**
   - Camera denied → app shows proper permission request.  
   - MediaPipe fails to track → app displays guidance to reposition.
3. **Multi-user Profiles**
   - Create multiple profiles, perform exercises, and verify that history is correctly associated.
4. **Notifications**
   - Test that reminders appear at scheduled times and lead users to the correct exercise.
5. **Device Compatibility**
   - Test on low-end and high-end devices to check performance and lag.

---

## 5. Test Reporting
- Record **test results** in a spreadsheet or a `TestingResults.md` file.  
- Include:
  - Test case ID  
  - Description  
  - Expected result  
  - Actual result  
  - Status (Pass/Fail)  
  - Notes for any bugs or anomalies

---

## 6. Future Testing Considerations
- Add automated regression tests whenever new exercises or features are added.  
- Implement performance benchmarks for real-time feedback latency.  
- Track MediaPipe version updates and re-test pose detection accuracy.  
