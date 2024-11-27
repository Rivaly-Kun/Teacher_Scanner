#Cordova API to build android application faster
#Cordova Setup 

#Cordova APK is located here:
--> platforms\android\app\build\outputs\apk\debug\app-debug.apk

 Here’s a step-by-step list to set up Cordova:

---

### **1. Install Node.js**
- Download and install Node.js from the [official website](https://nodejs.org/).
- Verify installation:
  ```bash
  node -v
  npm -v
  ```

---

### **2. Install Cordova CLI**
- Use npm to install Cordova globally:
  ```bash
  npm install -g cordova
  ```
- Verify Cordova installation:
  ```bash
  cordova -v
  ```

---

### **3. Create a New Cordova Project**
- Create a new project:
  ```bash
  cordova create project_name com.example.projectname ProjectName
  ```
  Replace:
  - `project_name` with the folder name.
  - `com.example.projectname` with the unique app ID.
  - `ProjectName` with the app’s display name.

---

### **4. Navigate to the Project Directory**
- Move into the project folder:
  ```bash
  cd project_name
  ```

---

### **5. Add Platforms**
- Add a platform (e.g., Android, iOS):
  ```bash
  cordova platform add android
  ```
  To add iOS:
  ```bash
  cordova platform add ios
  ```
- Check installed platforms:
  ```bash
  cordova platform ls
  ```

---

### **6. Add Plugins**
- Add necessary Cordova plugins:
  Example:
  ```bash
  cordova plugin add cordova-plugin-camera
  ```
- List installed plugins:
  ```bash
  cordova plugin ls
  ```

---

### **7. Build the Project**
- Build for a specific platform:
  ```bash
  cordova build android
  ```
  For all platforms:
  ```bash
  cordova build
  ```

---

### **8. Run the App**
- Test on a connected device or emulator:
  ```bash
  cordova run android
  ```
  Replace `android` with `ios` if using an iOS device.

---

### **9. Test and Debug**
- Use Chrome DevTools for debugging Android apps:
  - Connect your Android device and enable USB debugging.
  - Open Chrome and navigate to: `chrome://inspect`.

---

### **10. Update Cordova Components**
- To keep Cordova, platforms, and plugins up to date:
  ```bash
  npm update -g cordova
  cordova platform update android
  cordova plugin update
  ```

---

### **11. Troubleshooting**
- Check for missing dependencies or issues:
  ```bash
  cordova requirements
  ```
