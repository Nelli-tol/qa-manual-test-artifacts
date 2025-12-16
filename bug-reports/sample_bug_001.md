# BUG-001 — Login error message overlaps "Log In" button on mobile

**Environment:**
- iOS 18, Safari
- Screen width: 375px
- Build: Demo site

**Severity:** Minor  
**Priority:** P2

## Preconditions
- User is on login page

## Steps to Reproduce
1. Open login page on mobile
2. Enter invalid credentials
3. Tap "Log In"

## Actual Result
- Error banner overlaps the "Log In" button area
- UI looks broken and button becomes partially blocked

## Expected Result
- Error message should appear without covering controls
- "Log In" button should remain fully clickable

## Notes
- Might be missing responsive CSS for the error container