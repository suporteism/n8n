# n8n Repository

This repository contains n8n configurations and workflows.

## Getting Started / Como Iniciar

1.  **Prerequisites**: ensure you have Docker and Docker Compose installed.
2.  **Run n8n**:
    ```bash
    docker compose up -d
    ```
3.  **Access**: Open [http://localhost:5678](http://localhost:5678) in your browser.

## Usage / Uso

### Import Workflow
1.  Open n8n at [http://localhost:5678](http://localhost:5678).
2.  Click **"Add Workflow"** (top right) -> **"Import from..."** -> **"From File"** (or copy contents).
3.  Select `workflows/hello_world.json` from this repository.
4.  Click **"Execute Workflow"** to see it run!

---

## Implementation Plan (History)

# Create First Workflow

## Goal
Provide a sample n8n workflow file that the user can import into their local instance. This demonstrates the "Git + n8n" workflow.

## Proposed Changes
### Repository Structure
#### [NEW] [workflows/hello_world.json](file:///Users/ismaelalves/n8n/workflows/hello_world.json)
- A simple n8n workflow JSON: Manual Trigger -> Code Node (Hello World).

## Verification Plan
- User imports the JSON file into n8n localhost UI.
- User executes the workflow.

---

## Walkthrough (History)

# Local n8n Setup Walkthrough

## What I Did
1.  **Initialized Git Repository**: Created README and pushed to `suporteism/n8n`.
2.  **Installed Docker**: Used Homebrew to install Docker Desktop.
3.  **Configured Environment**:
    - Created `docker-compose.yml` for n8n service.
    - Created `.env` for timezone settings.
4.  **Updated Documentation**: Added instructions to README.

## Validation
- **Docker Installation**: Verified `brew install --cask docker` was successful.
- **Service Start**: User executed `docker compose up -d`.
- **Status Check**: Verified container is running with `Up` status on port 5678.

## Next Steps
- Access n8n at [http://localhost:5678](http://localhost:5678).
- Create your first workflow!
