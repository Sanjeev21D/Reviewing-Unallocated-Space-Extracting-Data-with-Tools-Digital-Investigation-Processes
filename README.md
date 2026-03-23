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
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9296a0ee-5329-49a0-bc4b-f9a7fe66f96f" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c89cc56c-ee55-45e9-a9f6-ec169d498a3a" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/aa595403-7d33-4e72-8f8f-1c539cdad9ba" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1a36d960-b085-4f52-90be-454876c3ce87" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/94a7cbbb-2b08-4af9-b16b-01003bf6811a" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2e091832-8996-444e-943d-b70d855c72dd" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a85df209-f0cc-44b8-80cd-59b7c504ef65" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/df47f894-e4c1-4c5e-b318-6a5227fa0cdb" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ad973def-967b-48bd-92eb-c73fe04606f4" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/00c71a0a-b97b-4b98-ad89-125edc3a3dbd" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fcfd7924-15f1-4519-9267-6a412da464fd" />
## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

