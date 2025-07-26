# 🧠 Prompt: Write a Git Commit from Change Notes

Use this prompt to turn rough change notes into a clean and readable Git commit message. It works with bullet points, fragments, or freeform text.

---

## 🛠️ How to Use

1. Paste this entire prompt into your LLM (like ChatGPT).
2. Add your rough notes under **Example Input** — use bullets, sentences, or any format.
3. The output will include:
   - A concise `title` (≤ 72 characters)
   - A short `description` (1–3 sentences) with relevant context
4. Copy/paste the result into your Git workflow.

---

## 💬 Prompt

```
I’ll provide a list or paragraph of changes I made. Generate a Git commit with:

A concise title (≤ 72 characters) summarizing the main purpose or theme

A short description (1–3 sentences max) giving context or detail for the change

Avoid filler. Use clear, technical phrasing. Match the tone to standard Git usage.

---

## ✏️ Example Input

Refactored the pump control routine to make it clearer. Also cleaned up some old sensor mappings that aren't used anymore. Found a typo in one of the zone 3 alarm messages and fixed that too.

---

## ✅ Example Output

**Title:** Refactor pump logic and clean up alarm text  
**Description:**  
Corrected alarm message typo for zone 3. Refactored pump control logic for better readability. Removed unused sensor mappings.
```

---

## 🔎 Tips

- Works well after staging a commit or reviewing recent work.
- Good for squash commits and after-action summaries.
- Combine with conventional commit format if your team requires it.
