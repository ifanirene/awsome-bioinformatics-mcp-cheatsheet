# Claude Code Configuration

## Instructions
When applying rules, reference them in brackets [rule-name] within responses for clarity and traceability.

You should also use a to do list to organize your thoughts (`tasks.md` or other scratchpad, if it does not exist use  `todo.md`). Especially when you receive a new task, you should first review the content of the todo.md and the context files, first explain the task, and plan the steps you need to take to complete the task. You can use todo markers to indicate the progress, e.g.
[X] Task 1
[ ] Task 2
Also update the progress of the task in the scratchpad when you finish a subtask.
When all the tasks are completed, you should update the scratchpad to summarize the session.

## Learning and Memory
- Document reusable project information (library versions, model names, fixes) in this file
- Track recurrent errors and their solutions to prevent repetition
- Use this file as a scratchpad for task organization and planning

## Environment Management
- **Primary conda environment**: Use the vascular-nuclei environment located at `/Volumes/IF_PHAGE/conda_envs/vascular-nuclei`
- **Activation command**: `conda activate /Volumes/IF_PHAGE/conda_envs/vascular-nuclei`
- **Environment verification**: Always run `conda list` to verify environment before package operations
- **Package management**: Use mamba for package installation when possible
- **Python environment**: Ensure numpy, scipy, matplotlib, seaborn, pandas, scikit-learn are available
- **Testing environment**: All Python scripts should be executed within the activated conda environment
- **Build new environments in**: `/Volumes/IF_PHAGE/conda_envs/` (only if needed for specific tasks)

## Code Style and Structure
- Use functional and declarative programming patterns; avoid classes
- Prefer iteration and modularization over code duplication
- Use comprehensive docstrings for all functions and classes
- Include type hints for better readability and error detection

## Naming Conventions
- Directories: lowercase with dashes (e.g., `components/form-wizard`)
- Component files: PascalCase (e.g., `VisaForm.tsx`)
- Utility files: camelCase (e.g., `formValidator.ts`)
- Favor named exports for components and utilities

## Code Annotations
Use standardized annotation blocks for new/modified code:
```python
"""
@description 
This component handles [specific functionality].
It is responsible for [specific responsibilities].

Key features:
- Feature 1: Description
- Feature 2: Description

@dependencies
- DependencyA: Used for X
- DependencyB: Used for Y

@examples
- Example usage quick
- Example usage detailed parameter setting
"""
```

## Error Handling
- Implement proper error boundaries
- Log errors appropriately for debugging
- Provide user-friendly error messages
- Handle network failures gracefully

## Testing
- Test memory usage and performance
- Implement unit tests for functions and pipeline components

## Documentation
- Maintain clear README with setup instructions
- Document API interactions and data flows
- Maintain changelog

## Python-Specific Rules
- Use 'seaborn-v0_8' instead of 'seaborn' for matplotlib styles
- Set `mpl.rcParams['pdf.fonttype'] = 42` for editable PDF text
- Use adjustText package to avoid label overlapping in scatter plots

## Reproducibility and Version Control
- Use Git for both code and datasets
- Implement proper experiment logging with all hyperparameters and results
- Use MLflow or Weights & Biases for experiment tracking
- Set random seeds and document full experimental setup

## Git Commit Prefixes
- `fix:` for bug fixes
- `feat:` for new features
- `perf:` for performance improvements
- `docs:` for documentation changes
- `style:` for formatting changes
- `refactor:` for code refactoring
- `test:` for adding missing tests
- `chore:` for maintenance tasks



## Key Lessons Learned

### Development Best Practices
- Always execute scripts after writing/editing them
- Read input data headings to confirm variable names before analysis


## Current Task Progress
*This section will be updated as tasks are completed*