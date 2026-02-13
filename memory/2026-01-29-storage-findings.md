# Storage Discrepancy Findings - 2026-01-29

## The Issue

Frank saw **458.75 GB free** in Settings.
I reported **388.1 GB free** from diskutil.

Difference: ~70 GB

## Root Cause

**APFS container has purgeable space:**
- Not allocated = truly free (388.1 GB)
- Available = free + purgeable (~458 GB)

## Purgeable Space Breakdown

| Source | Size | Type |
|--------|-------|-------|
| ~/Library/Caches | 18 GB | Application cache |
| ~/.npm (npm cache) | 5.2 GB | Package cache |
| /System/Volumes/Preboot (snapshots) | 40 GB | OS snapshots |
| /private/var/vm/sleepimage | 2 GB | Hibernation file |
| **Total purgeable** | **~65 GB** | Reclaimable |

## How macOS Reports Storage

**Settings (system_profiler):**
- Shows "Available" = free + purgeable
- Includes space that can be reclaimed automatically

**diskutil:**
- Shows "Not allocated" = truly free only
- Doesn't count purgeable space

## Lesson

When user asks about storage:
1. Use `system_profiler SPStorageDataType` for Settings-accurate view
2. Use `diskutil apfs list` for detailed breakdown
3. Explain difference between "free" vs "available" if discrepancy

## Commands

```bash
# Settings-accurate view
/usr/sbin/system_profiler SPStorageDataType

# Detailed breakdown
/usr/sbin/diskutil apfs list

# Caches breakdown
du -sh ~/Library/Caches
```

---

*Documented: 2026-01-29 05:48 CST*
