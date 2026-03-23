# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fb27fd03-595c-4bf1-b835-356c4142cd56" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7314cc09-3f6e-4165-b54c-92ae23e3e893" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f5f033e4-cd88-4a7a-a752-e2e1b85734b1" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/77bb8b73-2e17-4934-becd-b426f5576542" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/bf703f85-2f98-46a2-882e-b68801e4db78" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c04321c0-5cb2-4d6a-88ac-54c156c67a7e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/3fd69dfc-018f-463d-a17f-065b7cd251c3" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/352475b7-7ed0-4249-a856-bdd9e73ed4ee" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/91397b12-7402-4251-bf28-2afe73fb0676" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c656b4d3-328a-4637-9e5f-8b8f71499302" />
## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

