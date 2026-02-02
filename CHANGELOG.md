# Changelog

All notable changes to the Shellback SVN extension will be documented in this file.

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
