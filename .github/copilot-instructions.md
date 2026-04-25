# SpencerMarcu GitHub Profile Repository

This is a GitHub profile repository containing static content that displays on Spencer Marcu's GitHub profile page. The repository contains profile documentation and content files with no build system, runtime applications, or testing frameworks.

**ALWAYS** reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Repository Structure and Navigation

- **Repository Type**: GitHub profile repository (static content only)
- **Primary Files**: 
  - `README.md` - Main profile content displayed on GitHub
  - `Spencer-Marcu` - Additional profile text file with detailed information
  - `.github/` - GitHub-specific configuration and documentation

### Quick Repository Overview
```bash
# View repository structure
ls -la
```
Expected output:
```
.
..
.git/
.github/
README.md
Spencer-Marcu
```

### View All Content Files
```bash
# List all documentation and content files
find . -type f \( -name "*.md" -o -name "Spencer-Marcu" \) -not -path "./.git/*"
```
Expected output:
```
./README.md
./.github/copilot-instructions.md
./Spencer-Marcu
```

## Working Effectively

### Essential Commands - All Validated and Working
- **View main profile content**: `cat README.md`
- **View detailed profile**: `cat "Spencer-Marcu"`
- **Check repository status**: `git --no-pager status`
- **View recent changes**: `git --no-pager log --oneline -5`
- **Count content lines**: `wc -l README.md "Spencer-Marcu"`

### Content Editing Workflow
1. **Always backup before editing**:
   ```bash
   cp README.md README.md.backup
   cp "Spencer-Marcu" "Spencer-Marcu.backup"
   ```

2. **Edit content files** using your preferred editor or editing method (for example, nano or vim)

3. **Validate changes immediately**:
   ```bash
   # Verify content renders correctly
   cat README.md
   cat "Spencer-Marcu"
   ```

4. **Check git status after changes**:
   ```bash
   git --no-pager status
   git --no-pager diff
   ```

## Git Operations

### Standard Git Workflow (All Commands Validated)
```bash
# Check current status
git --no-pager status

# View changes made
git --no-pager diff

# Stage changes
git add README.md
git add "Spencer-Marcu"

# Commit with descriptive message
git commit -m "Update profile content: [description of changes]"

# Push changes
git push origin [branch-name]
```

### Branch Management
```bash
# View current branch
git branch

# View all branches
git branch -a

# Create new branch for changes
git checkout -b feature/update-profile

# Switch branches
git checkout [branch-name]
```

## Validation

### Content Validation Checklist
- **Markdown Syntax**: Ensure README.md uses valid markdown formatting
- **Content Accuracy**: Review profile information for accuracy and current relevance
- **File Integrity**: Verify both README.md and Spencer-Marcu files are present and readable
- **Git Status**: Ensure no unintended files are staged for commit

### Manual Validation Steps
1. **Read all content files completely**:
   ```bash
   cat README.md
   cat "Spencer-Marcu"
   ```

2. **Verify file structure**:
   ```bash
   ls -la
   find . -type f -not -path "./.git/*"
   ```

3. **Check for any untracked files**:
   ```bash
   git --no-pager status
   ```

## Common Tasks

### Update Profile Information
1. Edit README.md for main profile content
2. Edit Spencer-Marcu file for detailed information
3. Validate changes with `cat` commands
4. Commit and push changes

### Review Content
```bash
# Quick content overview
echo "=== README.md ===" && cat README.md && echo -e "\n=== Spencer-Marcu ===" && cat "Spencer-Marcu"

# Content statistics
wc -l README.md "Spencer-Marcu"
```

### File Operations
```bash
# Create backup copies
cp README.md README.md.$(date +%Y%m%d_%H%M%S)
cp "Spencer-Marcu" "Spencer-Marcu.$(date +%Y%m%d_%H%M%S)"

# Restore from backup (if needed)
cp README.md.backup README.md
cp "Spencer-Marcu.backup" "Spencer-Marcu"
```

## Critical Notes

### No Build or Test Requirements
- **NO BUILD PROCESS**: This repository contains only static content - no compilation, building, or packaging required
- **NO TESTING FRAMEWORK**: No unit tests, integration tests, or automated testing infrastructure
- **NO RUNTIME VALIDATION**: Content is static and displayed directly by GitHub - no application execution needed
- **NO DEPENDENCIES**: No package managers (npm, pip, etc.) or dependency installation required

### Content Guidelines
- README.md should follow standard GitHub profile markdown formatting
- Spencer-Marcu file is plain text format
- Keep content professional and current
- Ensure proper spelling and grammar

### Git Best Practices
- Always use descriptive commit messages
- Review changes with `git diff` before committing
- Use feature branches for significant content updates
- Keep commits focused on related changes

## Frequently Used Commands Reference

```bash
# Repository overview
ls -la

# Content viewing
cat README.md
cat "Spencer-Marcu"

# Git status check
git --no-pager status

# View changes
git --no-pager diff

# Content statistics
wc -l README.md "Spencer-Marcu"

# Find all content files
find . -type f \( -name "*.md" -o -name "Spencer-Marcu" \) -not -path "./.git/*"

# Recent commit history
git --no-pager log --oneline -5
```

## Expected File Contents

### README.md Structure
- Profile welcome message
- About Me section
- Skills & Technologies section
- Connect with Me section
- Repository description footer

### Spencer-Marcu File Structure
- Developer profile header
- Professional commitment statement
- Current focus areas (bulleted list)
- Contact and collaboration invitation

## Time Expectations
- **Content edits**: Immediate (< 1 minute)
- **Git operations**: Immediate (< 30 seconds)
- **File validation**: Immediate (< 30 seconds)
- **NO LONG-RUNNING OPERATIONS**: All tasks complete within seconds

This repository requires no special timeouts or long-running command considerations due to its simple static content nature.