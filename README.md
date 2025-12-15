# DevOps-Configuration
Documentation of configuration management and asset mapping.
# Configuration & Asset Management Lab

This repository documents my introduction to how software handles data and assets through configuration files.

## Project: Database & Asset Mapping (Football Manager)
**Objective:** Modify local configuration files (XML) to correct database discrepancies and map binary assets (images) to the correct user IDs.

### Methodology
1. **Unique Identifier (UID) Mapping:**
   - The software relies on unique Player IDs to retrieve data.
   - I wrote configuration lines to map local image files to specific Player IDs (e.g., `<record from="12345" to="graphics/pictures/person/12345/portrait"/>`).
   - This taught me that file naming conventions must match the database keys exactly for the software to read them.

2. **Data Integrity Correction:**
   - Edited the `.lnc` (Name Change) configuration files to replace placeholder text with accurate real-world data.
   - Verified that changes in the text file correctly updated the UI (User Interface) upon software reload.

### Tools Used
* **Text Editor:** Notepad++ (for editing XML and Config files).
* **File System:** Managing directory structures to ensure the software could locate the new assets.

## Why is this relevant to DevOps?
Even though this is a game, it taught me the fundamentals of **Configuration Management**:
* Software behavior is controlled by text files.
* If a file path or ID is off by one character, the system fails to load the asset.
* Attention to detail in syntax is critical.
