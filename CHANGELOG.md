# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.6] - 2025-08-28

### Fixed
- **Critical**: Fixed MCP framework API compatibility issue with `get_capabilities()` method
- **Critical**: Added proper `NotificationOptions` import from `mcp.server.lowlevel.server`
- **Enhancement**: Added connection retry mechanism with exponential backoff for improved reliability
- **Enhancement**: Improved error handling and logging for network connection issues
- **Bug**: Resolved uvx deployment issues caused by MCP framework API changes

### Technical Details
- Updated `Server.get_capabilities()` call to include required `notification_options` and `experimental_capabilities` parameters
- Added 3-retry mechanism with exponential backoff for Obsidian API connections
- Fixed import path for `NotificationOptions` class
- Enhanced error messages for better debugging

### Added
- Initial project setup
- Core MCP server functionality
- Obsidian vault management features
- Comprehensive documentation

## [0.1.0] - 2024-01-XX

### Added
- Initial release of ObsidianReaderMCP
- Core CRUD operations for Obsidian notes
- MCP (Model Context Protocol) server implementation
- Extended functionality with ObsidianExtensions
- Template system for note creation
- Batch operations support
- Link analysis and vault statistics
- Comprehensive test suite
- Documentation and examples
- PyPI publishing configuration
- uvx deployment support

### Features
- **Core Operations**:
  - Create, read, update, delete notes
  - List notes and search functionality
  - Tag management
  - Vault information retrieval

- **Extended Features**:
  - Batch note operations
  - Template system with variable substitution
  - Link analysis and broken link detection
  - Orphaned note identification
  - Vault statistics generation
  - Date range and word count filtering
  - Backup management

- **MCP Integration**:
  - Full MCP protocol support
  - Async/await architecture
  - Comprehensive error handling
  - Rate limiting and connection management
  - Tool registration for AI assistants

- **Developer Experience**:
  - Type hints throughout codebase
  - Comprehensive test coverage
  - Code formatting with Black
  - Import sorting with isort
  - Type checking with mypy
  - Automated CI/CD with GitHub Actions

### Technical Details
- Python 3.10+ support
- Built with modern async/await patterns
- Pydantic models for data validation
- httpx for HTTP client functionality
- Comprehensive logging and error handling
- Environment-based configuration

### Documentation
- Complete README with usage examples
- Chinese translation (README_zh.md)
- API reference documentation
- Publishing and deployment guides
- Contributing guidelines

[Unreleased]: https://github.com/QianJue-CN/ObsidianReaderMCP/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/QianJue-CN/ObsidianReaderMCP/releases/tag/v0.1.0
