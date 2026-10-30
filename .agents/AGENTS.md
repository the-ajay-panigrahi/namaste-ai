# Project Rules

- **Markdown Punctuation**: Do not use em dashes (`—`) or apostrophes (`'`) in Markdown notes. Use standard punctuation like colons (`:`), commas (`,`), standard hyphens (`-`), or separate sentences instead. Write contractions out in full (e.g. `does not` instead of `doesn't`).
- **No Checkboxes / Task Lists in Markdown**: Do not use `[x]` or checkbox-style task list indicators in Markdown files because they do not parse or render properly in Markdown previewers. Use standard clean bullet lists (`- `) instead.
- **Dictation & Note Creation**:
  - **Technical Accuracy**: Always technically verify that dictated or source content is accurate before writing.
  - **Preserve Key Phrasing & Important Content**: Retain the exact words and key phrasing from the source material wherever possible. Do not delete important or core information; almost all concepts from the source should be covered in the notes, while ensuring sentences are grammatically correct.
  - **Crisp & Concise Notes**: Keep notes very crisp, concise, and directly to the point. Avoid overly lengthy or verbose notes.
  - **Focus on Course Content**: Do not add separate external sources or research disclaimer sections. Keep notes strictly focused on the course material.
  - **No Summary Checklist**: Never write a summary checklist at the end of notes or episodes.
  - **First Principles Foundation**: Begin notes from first principles, clearly establishing why a technology is needed and explaining core meanings concisely.
- **Automatic Git Commits**: Automatically commit changes once a major portion of episode notes is complete or when meaningful milestones are reached, using clear and descriptive conventional commit messages.
- **Image Sizing**: Format all Markdown images using HTML `<img>` tags with a fixed width of 600 (`<img src="..." alt="..." width="600" />`) instead of standard Markdown image syntax (`![]()`), ensuring consistent display sizes across previewers.
- **Image Ordering**: Images provided for an episode must appear in the markdown notes in the exact numerical sequence provided (e.g. image 01, image 02, image 03, etc.).
- **Cleanup of Temporary Assets and Reference Files**: Once note generation and verification are complete, automatically delete temporary reference PDF files (such as `e1.pdf`) and temporary incoming asset folders (such as `assetsfors2ep1`) after their contents have been copied and renamed into the permanent `assets/` directory structure, unless explicitly instructed otherwise.
- **Rule Maintenance**: Automatically and proactively update `AGENTS.md` with new rules or preferences whenever established, without requiring an explicit reminder.
