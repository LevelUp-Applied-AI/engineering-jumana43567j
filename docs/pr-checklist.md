# Pre-PR Self Review Checklist

## Git & Repository Setup
- [ ] I accepted the GitHub Classroom assignment and am working in the correct repository
- [ ] I cloned the repository to my local machine using `git clone`
- [ ] I am working on a feature branch (NOT on main)
- [ ] I created the branch using `git checkout -b pr-05-pr-hygiene`
- [ ] I verified with `git status` that I am not on main

## Folder & File Structure
- [ ] I created the `.github` directory using `mkdir .github`
- [ ] The file `.github/pull_request_template.md` exists in the correct path
- [ ] The file `docs/pr-checklist.md` exists in the correct path
- [ ] The README.md file includes a "How to run" section
- [ ] I verified all file paths are correct before committing

## Environment & Execution
- [ ] The virtual environment `.venv` exists
- [ ] I successfully activated the virtual environment
- [ ] `(.venv)` appears in the terminal
- [ ] There are no environment or dependency errors

## Code Quality & PR Readiness
- [ ] The PR includes only the required changes for this assignment
- [ ] No debug prints or temporary code remain
- [ ] I reviewed my changes before pushing
- [ ] All required files are staged, committed, and pushed