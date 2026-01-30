# Specification Reference

This directory contains the official specifications for MusicXML and Agent Skills as Git submodules.

## Included Specifications

### MusicXML
- **Directory**: `musicxml/`
- **Official Repository**: https://github.com/w3c/musicxml
- **Official Website**: https://www.musicxml.com/
- **Current Version**: 4.0 (W3C Community Group Final Report)
- **Key Files**:
  - `schema/musicxml.xsd` - XML Schema Definition
  - `docs/` - Specification documents

MusicXML is a standard open format for exchanging sheet music data.
It is maintained by the W3C Music Notation Community Group.

### Agent Skills
- **Directory**: `agent-skills/`
- **Official Repository**: https://github.com/agentskills/agentskills
- **Official Website**: https://agentskills.io/
- **Specification Document**: https://agentskills.io/specification
- **Key Files**:
  - `docs/specification.mdx` - Specification document

Agent Skills is an open format for giving AI agents new capabilities.
Developed by Anthropic and adopted by Microsoft, OpenAI, GitHub, and others.

## Updating Specifications

### Update all submodules to latest
```bash
git submodule update --remote
```

### Update individually
```bash
# Update MusicXML only
git submodule update --remote specs/musicxml

# Update Agent Skills only
git submodule update --remote specs/agent-skills
```

### Commit after updating
```bash
git add specs/
git commit -m "Update spec submodules to latest"
```

## First-time Clone Instructions

When cloning this repository, initialize the submodules with the following command:

```bash
git submodule update --init --recursive
```

Or use the `--recursive` flag when cloning:

```bash
git clone --recursive <repository-url>
```
