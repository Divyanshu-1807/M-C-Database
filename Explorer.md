# File Explorer

Given an array of file objects, this component displays them in a hierarchical tree format.

### Object Types
- **Files**: 
  - Leaf nodes of the tree with no children.
- **Directories**: 
  - Can contain other objects (files or directories).

> **Note**: IDs and names within the same directory are unique.

## Requirements

### Naming and Structure
- Display the names of directories and files.
- Indent the contents of a directory to indicate hierarchy.

### Directory Functionality
- Directories can be expanded and collapsed.
- Clicking on a directory toggles its expanded/collapsed state.
- Directories should appear before files.
- All items must be sorted alphabetically within their respective categories.
- Style the expand/collapse functionality clearly.

### File Functionality
- Files are not expandable and cannot be interacted with.
- The focus is on functionality rather than styling.
- Directories can be empty.

## Data Format
```typescript
interface FileObject {
  id: number;
  name: string;
  children?: FileObject[];
}

