# GitHub Actions Lab: CI, Secrets, Variables & Artifacts

Hands-on demonstration of GitHub Actions CI workflows.

## Lab Implementation Details

| Component | Implementation | Expected Outcome |
|---|---|---|
| **Trigger** | `pull_request` on `main` | Workflow automatically triggers on PR |
| **Repository Secret** | `APP_API_KEY` configured via GitHub Secrets | Consumed in step safely without echoing/leaking |
| **Job-Level Variables** | `APP_ENV`, `BUILD_OUTPUT_DIR`, `APP_VERSION` | Available across all steps in the job |
| **Build Artifact** | `actions/upload-artifact@v4` with 7-day retention | Artifact downloadable directly from workflow run summary |

## Workflow File
The workflow is defined at [`.github/workflows/ci.yml`](.github/workflows/ci.yml).
