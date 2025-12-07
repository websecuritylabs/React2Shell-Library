# Contributing to React2Shell Library

We welcome contributions to the **React2Shell Library**! To maintain a high-quality resource for the community, please follow these guidelines.

## What we accept

- **New Research**: Blog posts or whitepapers detailing new findings about CVE-2025-55182.
- **Improved PoCs**: Scripts that demonstrate the vulnerability more clearly (must be safe/neutered).
- **Defense Tools**: Snort/Yara/Sigma rules, WAF configurations, or patching scripts.
- **Labs**: Dockerized environments or "Capture The Flag" rooms (like Vulhub/HackTheBox).

## Guidelines

1. **Relevance**: Ensure the link is directly related to **CVE-2025-55182** (React2Shell). Generic React tutorials will be rejected.
2. **No Duplicates**: Search the `README.md` to ensure your link hasn't already been added.
3. **Categorization**: Place your link under the most appropriate header (e.g., place Scanners under *Exploitation*, Patches under *Defense*).

### Adding Social Media Links
When adding a tweet or thread to the **Community** section:
1. **Format**: `[Author Name](Link to Tweet) - Description of the finding.`
2. **Quality**: Only add threads that contain *new* technical info, PoCs, or official vendor statements. Do not add generic "news" tweets.

## How to Submit

1. Fork this repository.
2. Create a new branch: `git checkout -b add-resource-name`.
3. Add your link in the following format:
   ```markdown
   - [Title of Resource](URL) - A brief description of what this resource covers.
Commit your changes: git commit -m "Add link to [Resource Name]".

Push to your branch and submit a Pull Request.