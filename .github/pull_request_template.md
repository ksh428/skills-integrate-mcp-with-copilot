## Description
This PR moves activity data from hardcoded Python dictionaries into a dedicated `activities.json` file, addressing issue #3.

## Changes
- Created `src/activities.json` with all activity data
- Updated `app.py` to load activities from JSON on startup
- Added `load_activities()` and `save_activities()` helper functions
- Modified signup and unregister endpoints to persist changes back to JSON

## Benefits
- Teachers can now modify activities without touching Python code
- Reduces fear of breaking the application when making changes
- Provides a clear data structure that's easy to understand

## Testing
The application loads activities from the JSON file and persists signup/unregister changes correctly.

## Related Issue
Fixes #3
