# Homelab Status Tray App

## Overview
This project is a system tray application designed to display the status of various homelab services and provide actionable controls for managing them. The app aims to be lightweight, user-friendly, and highly extensible, enabling users to easily add new services and customize actions.

---

## Features
- **System Tray Integration:** Displays status updates directly in the system tray for quick access.
- **Extensible Backend:**
  - Written in Rust for performance and safety.
  - Easy to add or modify service configurations.
- **Optional Frontend:**
  - A frontend can be launched on demand for a more detailed view.
  - Includes functionality for buttons and controls tied to service-specific API calls.
- **Service Management:**
  - Quickly view service statuses.
  - Perform actions like start, stop, or restart services with mapped buttons.
- **Customizable Actions:**
  - Buttons and controls can be easily reconfigured to match specific API calls or functionality changes.

---

## Goals
1. **Performance:** Ensure the app remains lightweight while running in the background.
2. **Flexibility:** Make it easy to add new services or modify existing ones.
3. **User Experience:** Provide an intuitive system tray interface with optional detailed views.
4. **Reliability:** Ensure accurate status updates and reliable control functionality.

---

## Project Structure
1. **Backend (Rust):**
   - Handles service status polling and API interaction.
   - Maintains service configuration and logic.
2. **Frontend (TBD):**
   - Only runs when needed.
   - Displays detailed service information and controls.
3. **System Tray Manager:**
   - Connects the backend to the system tray interface.
   - Handles status updates and simple interactions.

---

## Future Plans
- Support for monitoring additional types of services (e.g., Docker containers, VMs, etc.).
- Integration with notification systems for critical alerts.
- Configuration UI for managing services without editing code.
- Cross-platform support (Windows, macOS, Linux).

---

## Getting Started
1. **Prerequisites:**
   - Rust installed on your machine.
   - Basic knowledge of Rust and system tray apps.
2. **Setup Instructions:**
   - Clone the repository.
   - Modify the service configuration in the backend to match your homelab setup.
   - Build and run the app.
