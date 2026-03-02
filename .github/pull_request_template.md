## What changed

- Created `.github/pull_request_template.md`
- Created `docs/pr-checklist.md`
- Updated `README.md` to include a "How to run" section
- Verified project virtual environment setup

## Why

- `.github/pull_request_template.md` was added to standardize future pull requests and provide clear structure for reviewers.
- `docs/pr-checklist.md` was created to ensure proper self-review before opening any PR.
- The "How to run" section in `README.md` helps reviewers and contributors understand how to set up and execute the project.
- Virtual environment verification ensures the project runs in an isolated and consistent environment.

## How to test

1. Navigate to the project root directory.
2. Activate the virtual environment:
   - Windows: `source .venv/Scripts/activate`
3. Confirm that `(.venv)` appears in the terminal.
4. Verify the following files exist:
   - `.github/pull_request_template.md`
   - `docs/pr-checklist.md`
   - Updated `README.md` with "How to run" section.

## Checklist

- [ ] Verified correct folder structure and file paths
- [ ] Confirmed each file is in the correct directory
- [ ] Confirmed the virtual environment activates successfully
- [ ] README contains a proper "How to run" section
- [ ] All required files are committed and pushed