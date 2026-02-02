# Changelog

All notable changes to the Shellback SVN extension will be documented in this file.

## [0.4.2] - 2026-02-03

### Improved
- Added demo GIFs to README showcasing Update, Commit, and Revert operations

## [0.4.1] - 2026-02-03

### Fixed
- Fixed file path handling issue that caused SVN command failures

## [0.4.0] - 2026-02-02

### Added
- Configuration option to show full or relative file paths in file lists

## [0.3.0] - 2026-02-02

### Added
- **Commit: Show Changes feature** - View and edit file differences before committing
- **Revert:** Added double-click and right-click menu to view file changes (BASE vs Working Copy)

### Improved
- **Unified UI design** across all webview pages (Commit, Revert, Log, Add, Conflict)
- **File status display** - Unversioned files now show as "U" instead of "?" for consistency

### Fixed
- Commit: Fixed file list alignment issues (checkbox and file name not aligned)
- Show Log: Fixed issue where viewing file changes opened multiple windows instead of a single diff view
- Show Log: Fixed issue where files without extensions showed empty content in diff view
- Revert: Fixed diff view showing empty content on both sides
- File Decorations: Fixed display issue on Windows
- File Decorations: Fixed frequent UI flashing issue when saving files
  - Added debouncing mechanism to prevent excessive refresh triggers
  - Only refreshes UI when SVN status actually changes
  - Added configuration options: `autoRefresh` and `debounceDelay`

## [0.2.0] - 2026-02-02

### Features
- **Icon Overlays/Status Badges**: Explorer now displays visual status indicators for SVN files (Modified, Added, Deleted, Conflicted, Unversioned, Missing)
- Letter badges (M/A/D/C/U/!) and color coding for instant status recognition
- Folders show indicators when containing modified files
- Compatible with standard version control color themes
- Customizable color scheme via configuration

### Configuration
- `shellback-svn.decoration.useStandardColors`: Use standard version control colors (recommended for consistency)

## [0.1.0] - 2026-01-31

Initial release.

### Features
- Context menu integration for SVN operations
- Update, Commit, Show Log, Revert, Add, Delete, Cleanup commands
- TortoiseSVN-style log viewer (three-pane layout)
- Pre-commit update check with one-click update
- Interactive conflict resolution panel
- Commit message history
- Auto-detection of new/deleted files during commit
- Dual-mode commands (Alt/Option for root operations)
- Configuration options for customizing behavior
