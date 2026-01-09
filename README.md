# Test Case: Pip Full Priority Chain

## Package Manager
Pip

## Python Version Detection
- **Source**: .python-version (PRIORITY #1)
- **Expected Version**: 3.9.5

## All 8 Priority Files Present (Different Versions)
1. .python-version - 3.9.5 ✓ **SHOULD WIN**
2. .tool-versions - 3.10.0 (IGNORED)
3. pyproject.toml - >=3.11 (IGNORED)
4. Pipfile - 3.12 (IGNORED)
5. setup.py - >=3.8 (IGNORED)
6. setup.cfg - >=3.7 (IGNORED)
7. requirements.txt - Comment: 3.10+ (IGNORED)
8. environment.yml - 3.12 (IGNORED)

## Test Purpose
Ultimate stress test: All 8 priority files present with different versions. Validates complete priority order implementation.
