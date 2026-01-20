# Match Attribute Properties

<br>

## MATCHATTPROP (Command)
The Match Attribute Properties Add-In is a powerful AutoCAD productivity tool designed to synchronize properties and formatting across block attributes.

* Match text properties including Layer, Color, Style, Height, and Width Factor.
* Synchronize geometric properties like Rotation, Justification, and Relative Position.
* Optionally sync actual attribute values (text content) across matching tags.
* Filter applications to only affect visible attributes, protecting background data.
  
<br>
<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a9540737-6427-447c-8889-598b9e84d448" width="50%" alt="MatchAttProp" />
</p>

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Download from Autodesk App Store
For the simplest experience, download the Match Attribute Properties add-in directly from the Autodesk App Store. The installer handles all configuration automatically.

1. Download and install the add-in from the Autodesk Web Store.
2. At the command prompt, type `MATCHATTPROP` to run the add-in.

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Download from GitHub
If you prefer to manage your plugins manually or are using the version from GitHub, use the Autoloader method. This ensures the add-in is loaded automatically every time you open AutoCAD.

1. Download the `MatchProps.Bundle` folder.
2. Copy the folder to: `%APPDATA%\Autodesk\ApplicationPlugins\`.
3. Launch or restart AutoCAD.
4. Approve the security prompt by clicking “Always Load”.
5. At the command prompt, enter `MATCHATTPROP`.

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Workflow
The application is designed around a "Pick and Apply" workflow to ensure accuracy before modifying drawing data.


https://github.com/user-attachments/assets/47bc1427-bd68-4f05-84b7-9f5dff59c1bf


### Step 1: Picking the Source
Click "Pick Block" and select the block reference that contains your desired formatting. A block snapshot will appear in the preview window.

### Step 2: Selecting Properties
Select the checkboxes for the specific properties you wish to transfer. Use "Select All" for a full sync or "Deselect All" to pick individual items like only Color or Position.

### Step 3: Applying to Targets
Click "Apply" and select your destination blocks. The tool will find matching Attribute Tags and update them instantly. The command exits automatically upon completion.

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Supported Properties
The tool synchronizes properties between blocks by matching **Attribute Tags**. If a tag exists in the source block but not the target, it is gracefully skipped.

### Property Types
* **General**: Layer, Color, Linetype, Lineweight, and Visibility.
* **Text**: Style, Height, Rotation, Width Factor, and Oblique Angle.
* **Geometry**: Relative Position (offset from block base), Justification, and Alignment Point.
* **Content**: Attribute Value (Text String synchronization).

### Command Options
* **Match Visible Attributes Only**: When this is active, the command ignores properties of hidden attributes within the source block.
* **Sync Attribute Values**: When this is active, the actual text content from the source block attributes is copied to the matching target block attributes.

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## About this Application
Our goal is to provide the Autodesk community with practical, high-performance tools that eliminate repetitive tasks. `MATCHATTPROP` was developed to extend the logic of the native AutoCAD `MATCHPROP` command specifically for block attributes.

The current version provides essential functionality for copying attribute properties. Based on user feedback, future updates may bring additional features and improvements.

Please report any bugs or suggestions for new functionality by sending a personal message to @arshdeepsingh404 via your Autodesk Community account. Your feedback is invaluable and will help improve this tool for the entire community.

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Developer
**Arshdeep Singh**<br>
Full-Stack Industrial Automation Developer  
Autodesk Expert Elite | C. Tech | CMSE® | CAPM®

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

## Version History
| Version | Date | Changes |
| :--- | :--- | :--- |
| **1.0.0** | January 2026 | Initial Release |

&nbsp;
<p align="center">◈ ◈ ◈</p>
&nbsp;

_© 2026 Match Attribute Properties. All rights reserved._
