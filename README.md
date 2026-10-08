# oracle-free-vps-catcher (WIP)

An automated Node.js tool to continuously request and claim Always Free Ampere ARM instances (`VM.Standard.A1.Flex`) in congested regions with Telegram control.

> 🚧 **Upcoming Release Notice (Work in Progress):** 
> We are currently refactoring the tool to interact **directly with the native OCI REST API**. The features listed below represent the planned architecture and are not yet available in the current codebase.

---

## 📌 Planned Features & Architecture

* **No OCI CLI Dependency:** Complete removal of the `oci-cli` binary and Python dependencies. The application will issue raw HTTPS requests straight to Oracle Cloud infrastructure.
* **Native Request Signing:** Built-in cryptographic request signing using Node.js standard `crypto` module paired with your API key (`.pem`).
* **Lightweight Footprint:** Native API integration means negligible RAM/CPU overhead, making it easy to run on tiny VPS instances, Raspberry Pi, or Docker containers.
* **Continuous Auto-Catcher:** Smart polling logic across Availability Domains to claim ARM resources as soon as capacity opens up.
* **Telegram Management:** Real-time notification system and bot control interface (`/status`, `/pause`, `/resume`, `/set_interval`).

---

## 🛠 Planned Configuration Setup

Once released, the project will require standard OCI API credentials instead of CLI authentication
