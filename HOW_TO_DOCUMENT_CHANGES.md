# Guide to Documenting Changes and Adding References

Thank you for helping make this project better! Documenting changes and adding references or notes is essential for keeping contributions clear and understandable. This guide covers the main techniques to clarify your contributions and add references.

## Table of Contents
1. [Adding Inline Comments in Markdown](#adding-inline-comments-in-markdown)
2. [Using Footnotes for Additional Information](#using-footnotes-for-additional-information)
3. [Adding Reference Links for Citations](#adding-reference-links-for-citations)
4. [Creating Notes in YAML or Markdown Files](#creating-notes-in-yaml-or-markdown-files)
5. [Using Comments in Code Files or Data Scripts](#using-comments-in-code-files-or-data-scripts)
6. [Adding a References Section](#adding-a-references-section)

---

## 1. Adding Inline Comments in Markdown

For brief notes or clarifications, you can add inline comments directly in the Markdown text.

Example:
```markdown
This analysis builds on previous findings *(see reference [1])* and expands upon the initial dataset.
```

This keeps your explanations directly within the context of the text without taking up too much space.

---

## 2. Using Footnotes for Additional Information

Footnotes are a great way to provide extra context without cluttering the main text. You can add footnotes in Markdown using `[^1]` notation.

Example:
```markdown
This finding suggests a new approach to the problem.[^1]

[^1]: Additional details on this approach can be found in the referenced study.
```

Each footnote will appear at the bottom of the document, allowing readers to easily access more information without breaking their flow.

---

## 3. Adding Reference Links for Citations

When you need to reference specific studies or external sources, you can use inline links. This is helpful for citing articles, datasets, or other works directly.

Example:
```markdown
This approach aligns with recent research by Doe et al. [Doe et al., 2023](https://doi.org/10.1000/j.journal.2023.01).
```

This format provides readers with a direct link to the source for immediate reference.

---

## 4. Creating Notes in YAML or Markdown Files

For structured files like `references.yaml`, you can add notes as additional fields. This helps provide context for each entry in a separate file.

Example in `references.yaml`:
```yaml
- title: "Title of the first paper"
  author: "Author Name"
  year: 2023
  doi: "10.1000/j.journal.2023.01"
  notes: "This source discusses the primary methodology used in this project."
```

Using a “notes” field in YAML helps organize comments on each reference systematically.

---

## 5. Using Comments in Code Files or Data Scripts

If you’re working in code or data files, add comments to describe changes or explain specific sections. Use `#` for Python or `//` for JavaScript.

Example in Python:
```python
# This section loads additional datasets to support comparative analysis.
data = load_dataset("new_data.csv")
```

Comments make your code more readable and help others understand the purpose of each part.

---

## 6. Adding a References Section

If your contribution includes multiple references, you may want to add a “References” section at the end of the document. This section lists all citations in a standard format, which you can then reference by number in the text.

Example:
```markdown
## References
1. Doe, J., & Smith, A. (2023). "Title of the paper." *Journal of Research*, 50(3), 123-145. [DOI: 10.1000/j.journal.2023.01]
2. Lee, K. (2022). "Another important paper." *Science Advances*, 15(2), 33-47. [DOI: 10.1000/sciadv.2022.02]
```

In the main text, refer to these by number, like so:
```markdown
This methodology is based on established principles [1].
```

---

By following these techniques, you’ll keep your contributions organized and accessible, making it easier for others to understand and build upon your work. Thank you for documenting your contributions thoughtfully! 😊