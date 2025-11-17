# Mini Casino Frontend

## Issue Fixed: Git Submodule Problem

The `client` directory was previously being tracked as a git submodule instead of a regular directory. This has been fixed.

### What Happened

When you had a separate git repository inside the `client` folder and committed it to the parent repository, Git automatically registered it as a submodule. This caused the client files to not appear in the repository.

### How to Add Your Client Files

1. Make sure you're in the repository root directory
2. Copy your client application files into the `client/` directory
3. Remove any `.git` directory from inside `client/` if it exists:
   ```bash
   rm -rf client/.git
   ```
4. Add the files to git:
   ```bash
   git add client/
   git commit -m "Add client files"
   git push
   ```

### Project Structure

```
MiniCasinoFrontend/
├── client/          # Frontend application files go here
└── README.md        # This file
```

## Development

Add your frontend application setup instructions here once the client files are added.
