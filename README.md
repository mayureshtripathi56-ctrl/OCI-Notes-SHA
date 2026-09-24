# Package Instructions

This package keeps the tutorial and screenshots in the directory structure required by the Markdown image links.

## Contents

- `Simple-OCI-VCN-Structure.md` — GitHub Wiki tutorial page
- `assets/` — all screenshots and the final VCN diagram
- `OCI_VCN_Reference_Structure.drawio` — editable draw.io source

## Use in a GitHub Wiki repository

1. Extract the ZIP file.
2. Copy `Simple-OCI-VCN-Structure.md` to the root of the Wiki repository.
3. Copy the complete `assets` folder to the same root.
4. Commit and push both the Markdown page and the `assets` folder.
5. Do not rename or separate the image files unless you also update their paths in the Markdown.

The Markdown references screenshots using paths such as:

```markdown
![Step 1](assets/oci-vcn-simple-01-open-blank-editor.jpg)
```
