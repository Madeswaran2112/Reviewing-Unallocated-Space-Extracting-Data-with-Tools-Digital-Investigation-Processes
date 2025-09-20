<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/66ef4683-0cc3-49c0-9ed5-05fbc4d88a82" /># Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
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

<img width="1884" height="995" alt="img 1" src="https://github.com/user-attachments/assets/52d8a814-4b96-43cb-91bf-bb77da228004" />

<img width="1023" height="485" alt="image" src="https://github.com/user-attachments/assets/77f5aec9-9639-47a8-9c44-b9144f39e77a" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/40b9dcea-e704-48d9-8a18-6de02ec4be3d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/afd81c8e-d341-44e4-b3d8-8003337a1083" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/478126a3-dd20-4a4b-9313-e5bf01fcdef3" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/493ba926-bf5d-492d-848e-4622cfe37926" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b9d1dcd8-9ebf-4995-a00c-4bc6204c61af" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fa484a45-a3bd-42b7-a20d-02a51a9388c5" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

