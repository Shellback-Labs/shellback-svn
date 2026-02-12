# Changelog

All notable changes to the Shellback SVN extension will be documented in this file.


## [0.7.5] - 2026-02-12

### Added
- **Show Log Page:** Message list (commit list) entries now have a right-click context menu "Copy to clipboard" with: Full data, Full data without changed paths, Revisions, Authors, Messages

## [0.7.4] - 2026-02-11

### Changed
- **Show Log Page:** Message list displayed in columns (Revision, Author, Date, Message); date format YYYY-MM-DD HH:mm:ss; revision shown as number only (no "r" prefix)
- **Show Log Page:** Message list and file list text are no longer selectable (use Copy message / context menu to copy)

## [0.7.3] - 2026-02-10

### Changed
- **Update Page:** File list status indicators now use full words (e.g. Updated, Added, Modified, Deleted, Merged, Conflicted, Replaced) instead of single-letter codes (U, A, M, D, G, C, R) to avoid ambiguity with other pages

## [0.7.2] - 2026-02-09

### Added
- **Show Log Page:** Added configuration option `shellback-svn.log.showFullPathInTab` to control whether tab title shows full path or just filename/folder name (default: false, shows only filename/folder name)
- **Commit & Revert Pages:** Context menu operations now support batch operations when multiple files are selected
- **Update Page:** Context menu operations now support batch operations when multiple files are selected

### Changed
- **Show Log Page:** Tab title now only displays filename or folder name by default instead of full path

## [0.7.1] - 2026-02-07

### Changed
- Updated README documentation

## [0.7.0] - 2026-02-07

### Added
- **File list context menu enhancements** - Added basic file operations to context menus in Commit, Revert, ShowLog, and Update pages:
  - **Open** - Open file in editor
  - **Reveal In File Explorer** - Show file in system file explorer
  - **Copy Path** - Copy full file path to clipboard
  - **Copy Relative Path** - Copy relative file path to clipboard
- All operations use VSCode's native APIs for consistent behavior
- **Revert Page: List selection** - Added file list selection with multi-select (Ctrl/Cmd), range select (Shift), and Space key to toggle revert state for selected files

### Changed
- **Revert Page:** Changed default file selection state to all unchecked

## [0.6.5] - 2026-02-07

### Added
- **Commit Page: List selection** - Added file list selection with multi-select (Ctrl/Cmd), range select (Shift), and Space key to toggle commit state for selected files

## [0.6.4] - 2026-02-07

### Changed
- **Commit Page:** Changed default file selection state to all unchecked

## [0.6.3] - 2026-02-06

### Changed
- Updated multilingual text

### Fixed
- Fixed GBK encoding issue in diff panel

## [0.6.2] - 2026-02-06

### Changed
- **Conflict Resolution Page:** Removed three "Diff With" options (Diff with Mine, Diff with Theirs, Diff with Base) from the context menu
- **Conflict Resolution Page:** Removed checkmark symbols (✓) from "Use Mine", "Use Theirs", and "Use Base" menu items

## [0.6.1] - 2026-02-05

### Added
- **Localization support:** Added internationalization (i18n) support for the extension

## [0.6.0] - 2026-02-05

### Added
- **Update Page:** Automatically opens after Update completes, showing updated files with status indicators
- **Commit Page:** Added "Delete" option in context menu for unversioned files (status 'U'). Unversioned files can now be deleted directly from the Commit page instead of using Revert (which doesn't apply to unversioned files)

### Fixed
- **Windows GBK encoding:** Fixed garbled text in filenames on Windows by properly decoding GBK encoding output from SVN CLI using iconv-lite library.

## [0.5.2] - 2026-02-05

### Changed
- **Plugin icon and README:** Updated extension icon and README information

## [0.5.1] - 2026-02-05

### Added
- **Show Log: Copy message button** - Added a "Copy message" button in the log viewer's message pane (right side) to quickly copy commit messages to clipboard

### Fixed
- **Root commands scope:** All command-palette "Root" operations (Commit Root, Update Root, Revert Root, Show Log Root, Add Root, Resolve Root, Cleanup Root) now operate on the **current VSCode workspace folder root** instead of the SVN working copy root. When you open a subfolder of an SVN repo, Root commands now correctly scope to that opened folder.
- **Show Log: File name colors** - Fixed file names in the changed files list not displaying status-based colors (now matches Commit page style with color-coded file names for A/M/D/R statuses)

### Improved
- **UI styling:** Removed divider lines (borders) from all webview pages (Commit, Revert, Log, Add, Conflict) for a cleaner, more unified appearance

## [0.5.0] - 2026-02-04

### Fixed
- Fixed file names with non-ASCII characters (e.g., Chinese) displaying incorrectly in all file lists
- **Fixed checkbox behavior:** Clicking file name in Commit/Revert dialogs no longer toggles checkbox - only direct checkbox clicks affect selection state
- **Fixed cursor style:** File list items in Commit/Revert dialogs no longer show pointer cursor when hovering, as clicking them doesn't perform any action
- **Fixed text selection:** File names in all dialogs (Commit/Revert) can no longer be accidentally selected when hovering or clicking

### Improved
- **Context menu availability:** SVN operations now also available in editor tab context menu (right-click on file tabs) for easier access
- **Revert page:** Moved single file revert to context menu, removed redundant buttons, fixed confirmation dialog button count
- Improved file list layout in commit dialog to use available space efficiently
- Added revert option to file context menu in commit dialog
- Updated context menu text for better clarity
- **File list color coding:** Applied consistent status-based colors to file names in Revert and Add dialogs (matching Commit dialog style)
- **File list typography:** Unified font style (normal weight) for file names across all dialogs (Commit/Revert/Add)

## [0.4.3] - 2026-02-03

### Changed
- Changed pre-commit behavior to match TortoiseSVN: now detects out-of-date errors during commit and offers to update and retry (using QuickPick for better UX)
- Removed `checkUpdateBeforeCommit` configuration (out-of-date handling is now always enabled, following TortoiseSVN behavior)

### Fixed
- Fixed commit page file list showing SVN output information lines (Changelist and Summary of conflicts) as files

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
