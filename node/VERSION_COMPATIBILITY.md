# Node.js Package Version Compatibility Matrix

This document lists the required package versions across all OpenCDx Node.js projects to ensure compatibility.

**Last Updated**: October 11, 2025  
**Release**: v1.0.1

## Core Dependencies

| Package | ui-library | opencdx-dashboard | ADR-gui | Notes |
|---------|------------|-------------------|---------|-------|
| **Node.js** | ≥20 | ≥20 | ≥20 | Recommended: 20.x LTS |
| **Next.js** | 15.4.2 | 15.4.2 | 15.4.2 | ✅ Aligned |
| **React** | 18.3.1 | 18.3.1 | 18.3.1 | ✅ Aligned |
| **React DOM** | 18.3.1 | 18.3.1 | 18.3.1 | ✅ Aligned |
| **TypeScript** | 5.5.2 | 5.7.3 | 5.5.2 | ⚠️ Minor variance acceptable |
| **framer-motion** | ~11.18.2 | ~11.18.2 | ~11.18.2 | ✅ Aligned |
| **Tailwind CSS** | 3.4.14 | 3.4.3 | 3.4.4 | ⚠️ Patch variance acceptable |
| **NextUI** | 2.6.11 | 2.6.11 | 2.4.2 | ⚠️ ADR-gui older (deprecated, stable) |

## UI Library Integration

| Consumer | Dependency Path | Version | Status |
|----------|----------------|---------|--------|
| **opencdx-dashboard** | `file:../../ui-library` | Local build | ✅ Correct |
| **ADR-gui** | `file:../ui-library` | Local build | ✅ Correct |

**Important**: All consumers must use the built ui-library package (not `/src`). See consumer README for setup workflow.

## Version Alignment Policy

### ✅ Must Match (Breaking if different):
- Next.js major/minor (15.x)
- React major/minor (18.x)
- framer-motion minor (~11.18.x)

### ⚠️ Should Match (Recommended):
- TypeScript major (5.x) - minor variance OK
- Tailwind CSS minor (3.4.x) - patch variance OK
- NextUI major (2.x) - minor variance acceptable (deprecated lib)

### ℹ️ Can Vary:
- Build tools (tsup, webpack, vite)
- Testing libraries (cypress, playwright)
- Dev dependencies

## Updating Dependencies

When updating a core dependency:

1. **Check this matrix** for required versions
2. **Update all affected repos** to maintain alignment
3. **Test all apps** after updates
4. **Update this document** with new versions
5. **Commit as a single PR** across repos

## Known Issues

- **NextUI deprecated**: Migrating to HeroUI in future release
- **TypeScript variance**: Minor versions differ but compatible
- **Package managers**: npm used (no yarn/pnpm mixing)

## Related Documentation

- [ui-library README](../../ui-library/README.md) - Library setup and usage
- [ui-library COMPONENT_GUIDELINES.md](../../ui-library/COMPONENT_GUIDELINES.md) - Component composition patterns
- [opencdx-dashboard README](../../opencdx-gui/opencdx-dashboard/README.md) - Dashboard setup
- [ADR-gui README](../../ADR-gui/README.md) - ADR GUI setup
