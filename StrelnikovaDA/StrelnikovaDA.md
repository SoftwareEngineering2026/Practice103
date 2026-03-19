# Refactoring Report: FundingRaised (Clean Code)
PR:https://github.com/SoftwareEngineering2026/103-refactoring-exercise/pull/3

## Summary
Refactored `FundingRaised` class to improve readability, maintainability, and remove duplication. Applied Clean Code principles: DRY, SRP, self-documenting code.

## Changes Made

### 1. Extract row mapping (`mapRow`)
- Removed duplicate row-to-object mapping
- Introduced `mapRow` function
- Commit: `Refactor: extract mapRow function (Clean Code: DRY)`

### 2. Extract filtering logic (`applyFilters`)
- Removed repeated filter checks
- Created reusable `applyFilters` function
- Commit: `Refactor: extract applyFilters function (Clean Code: SRP, reusable)`

### 3. Replace magic numbers with `COLUMNS` constants
- Replaced numeric indexes with descriptive constants
- Commit: `Refactor: replace magic numbers with COLUMNS constants (Clean Code: self-documenting code)`

### 4. Extract CSV filename to constant
- Centralized CSV filename as `FUNDING_FILE`
- Commit: `Refactor: extract CSV filename to constant FUNDING_FILE (Clean Code maintainability)`

## Overall Benefits
- Reduced duplication
- Clear responsibilities
- Easier extension of filter logic
- Better readability and maintainability

## Files Changed
- `node/funding_raised.js`