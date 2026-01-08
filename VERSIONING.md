# Versioning Guide

This project follows [Semantic Versioning](https://semver.org/) (SemVer).

## Version Format

**MAJOR.MINOR.PATCH** (e.g., `1.2.0`)

- **MAJOR**: Breaking changes to skill structure or incompatible API changes
- **MINOR**: New features, patterns, or capabilities (backward-compatible)
- **PATCH**: Bug fixes, documentation updates, minor improvements

## Version History

### v1.2.0 (January 2026)
**OpenAI Codex Support & Platform Expansion**
- Added OpenAI Codex CLI/IDE compatibility
- Added Codex-specific installation and usage documentation
- Added Figma MCP integration guides for Claude and Codex
- Added GitHub Pages website with interactive demo
- Added Smithery badge and registry listing
- Added auto-rebuild workflow for skill ZIP distribution
- Various bug fixes and documentation improvements

### v1.1.0 (November 2025)
**Accessibility & Expanded Frameworks**
- Added comprehensive accessibility guidelines (`references/accessibility-guidelines.md`)
- Added research-backed benchmarks for content evaluation
- Expanded SKILL.md with additional patterns and frameworks
- Added CHANGELOG.md for tracking changes

### v1.0.0 (November 2025)
**Initial Release**
- Core UX writing skill framework
- Four quality standards: Purposeful, Concise, Conversational, Clear
- Common UX patterns: buttons, errors, empty states, forms, notifications, onboarding
- Voice and tone guidance
- Reference materials and templates
- CONTRIBUTING.md with contribution guidelines

## Creating a New Release

### 1. Update Version Number

Update the version in `README.md`:
```markdown
**Status**: Production-ready • **Version**: X.Y.Z • **Last updated**: Month Year
```

### 2. Update VERSIONING.md

Add a new entry to the Version History section above with:
- Version number and date
- Brief title describing the theme
- Bullet points of key changes

### 3. Commit Changes

```bash
git add README.md VERSIONING.md
git commit -m "Release vX.Y.Z: Brief description"
```

### 4. Create and Push Tag

```bash
# Create annotated tag
git tag -a vX.Y.Z -m "Release vX.Y.Z: Brief description"

# Push tag to GitHub
git push origin vX.Y.Z
```

### 5. Create GitHub Release

1. Go to [Releases](https://github.com/content-designer/ux-writing-skill/releases)
2. Click "Draft a new release"
3. Select the tag you just pushed
4. Add release title: `vX.Y.Z - Release Title`
5. Copy the version notes from VERSIONING.md into the description
6. Publish the release

GitHub automatically creates downloadable ZIP and tarball artifacts for each release.

## When to Bump Versions

### Bump MAJOR (1.x.x → 2.0.0) when:
- Changing SKILL.md structure in breaking ways
- Removing or renaming core reference files
- Changing the skill's fundamental approach

### Bump MINOR (x.1.x → x.2.0) when:
- Adding new reference documents
- Adding new pattern categories
- Adding support for new platforms (e.g., Codex)
- Adding significant new features

### Bump PATCH (x.x.1 → x.x.2) when:
- Fixing typos or errors
- Clarifying existing documentation
- Minor improvements to examples
- Bug fixes in templates

## Accessing Previous Versions

Users can access any version via GitHub:

- **Releases page**: https://github.com/content-designer/ux-writing-skill/releases
- **Direct download**: https://github.com/content-designer/ux-writing-skill/releases/tag/vX.Y.Z
- **ZIP archive**: https://github.com/content-designer/ux-writing-skill/archive/refs/tags/vX.Y.Z.zip
