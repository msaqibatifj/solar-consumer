Pull Request

Description
- Summary: Remove `nowcasting_datamodel` and strip code/tests that depend on it.
- Motivation and context: Remove an unused dependency and reduce maintenance burden.
- Dependencies: None added; one dependency removed.
- Fixes: (none)

How Has This Been Tested?
- Yes — I searched the repository for `nowcasting_datamodel` and updated or removed all usages.
- Reproduction: regenerate lockfile, install, then run tests:

```bash
pip install -e .
pytest
```

_If your changes affect data processing, have you plotted any changes?_ No

Checklist
- [ ] My code follows OCF's coding style guidelines
- [ ] I have performed a self-review of my own code
- [x] I have made corresponding changes to the documentation (`README.md`)
- [ ] I have added tests that prove my fix is effective or that my feature works
  - Reason: tests that depended on the removed datamodel were deleted to avoid import failures
- [ ] I have run the test suite locally and fixed any failures
- [x] I have checked my code and corrected any misspellings

If you want this as a GitHub PR template, I can create `.github/PULL_REQUEST_TEMPLATE.md` with the same content.