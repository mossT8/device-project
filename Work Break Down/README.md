# Work Breakdown Structure (WBS)
___
This document outlines a simple work breakdown structure for a web application where users can register and configure their ESP32 chip-based IoT devices. These devices record metrics and are customizable, allowing users to create tailored solutions.

The WBS is divided into three primary sections:
- **User Account Management**: For user registration, login, and profile management.
- **Device Management**: For adding, configuring, and managing devices.
- **Device Dashboard**: For viewing device data and customized graphs.
___

## 1. User Account Management
This section covers all actions related to managing user accounts, such as registration, login, and profile updates.
___

### 1.1 Register an Account
- **Goal**: Enable users to create a new account.
- **Requirements**:
  - User provides:
    - Email address
    - Password
    - Basic user details (e.g., name, address)
  - Soft email verification:
    - Upon registration, users receive limited access until email is verified.

### 1.2 Log into Account
- **Goal**: Allow users to log in securely to the web application.
- **Requirements**:
  - User provides:
    - Email or username
    - Password

### 1.3 Log out of Account
- **Goal**: Provide a secure way to end the user session.
- **Requirements**:
  - Ensure session data is cleared and no personal information is stored on the client-side after logout.

### 1.4 Change Account Password
- **Goal**: Allow users to update or recover their account password.
- **Requirements**:
  - Update password from profile settings.
  - Password recovery via a "Forgot Password" flow.

### 1.5 Change Email
- **Goal**: Enable users to update their email address.
- **Requirements**:
  - Verify the new email before making the change permanent.

### 1.6 Change Account Details
- **Goal**: Allow users to update personal details in their account.
- **Requirements**:
  - Editable fields:
    - Name
    - Address information
    - Contact information (e.g., phone number)

___
## 2. Device Management
This section covers adding, configuring, viewing, and removing user devices from their account.
___

### 2.1 Add Device
- **Goal**: Allow users to add new devices to their account.
- **Requirements**:
  - User provides:
    - Serial Number
    - Model Name
    - Custom device name for identification

### 2.2 View Devices
- **Goal**: Enable users to view a list of all devices associated with their account.
- **Requirements**:
  - Display basic device information (e.g., name, model).
  - Provide device status (active/inactive).

### 2.3 Configure Device
- **Goal**: Allow users to customize device settings based on their preferences.
- **Recording settings**:
  - User-configurable options:
    - Metric Name (e.g., temperature, humidity)
    - Recording Frequency (e.g., every minute, hourly)
    - Units (e.g., Celsius, Fahrenheit)
- **Graph settings**:
  - Customizable axes for visual data representation:
    - X-axis:
      - Label
      - Minimum and maximum values
    - Y-axis:
      - Label
      - Minimum and maximum values

### 2.4 Remove Device
- **Goal**: Enable users to remove devices from their account.
- **Requirements**:
  - Confirmation prompt before device removal.

___
## 3. Device Dashboard
This section focuses on providing users with a graphical interface to view and monitor their devices' metrics and data in real-time.
___

### 3.1 View Device Dashboard
- **Goal**: Provide users with an interactive dashboard to monitor device metrics.
- **Requirements**:
  - Display graphs for all configured metrics.
  - Real-time updates for data recorded by devices.
  - Allow customization of graph views (e.g., time range, data granularity).
