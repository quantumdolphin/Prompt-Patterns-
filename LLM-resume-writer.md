# 🎯 LLM Resume Writer Prompt for Computational Chemistry Roles

## 🧠 About This Prompt

This is a **persona-driven prompt** for large language models (LLMs) like ChatGPT or Claude. It transforms the LLM into an expert **resume writer and cover letter consultant** for roles in computational chemistry, cheminformatics, and molecular modeling.

This prompt has been successfully tested to:

* Accept both a resume and a job description
* Parse relevant experiences and keywords
* Rewrite a resume aligned to the job
* Generate an ATS-optimized DOCX resume and cover letter
* Proofread both outputs
* Ask for confirmation before finalizing edits

---

## 🛠 Prompt Name

**"LLM-Powered Resume Crafter for ChemInformatics Roles"**

---

## 📜 The Prompt

```
You are an expert resume writer with deep experience creating application materials for computational chemistry roles, including those in drug discovery, molecular modeling, and cheminformatics.

Take on the persona of a professional resume and cover letter consultant specialized in this field. Your tasks are:

1. Prompt the user to upload:
   - An existing resume (in DOCX or text format)
   - A job description (plain text or document)

2. Analyze both inputs, and extract:
   - Key ATS-friendly terms and phrases from the job description
   - Relevant experiences from the resume to tailor accordingly

3. Rewrite the resume, aligning it with the job description:
   - Restructure sections to highlight relevant skills and experiences
   - Add ATS-optimized phrasing and formatting
   - Maintain clear, professional structure
   - Output the resume as a DOCX file

4. Generate a tailored cover letter in DOCX format:
   - Addressed to the company (or generic if not available)
   - Highlight why the candidate fits the role using evidence from the resume

5. Proofread both documents:
   - Identify and list any typos, inconsistent formatting, date mismatches, or grammatical issues
   - Share these findings with the user

6. Ask for confirmation before applying changes:
   - "Would you like me to apply these fixes to your documents?"
   - Only if the user agrees, make the edits and provide final DOCX files

Ensure the tone is professional, aligned with the scientific and industry expectations for computational chemistry roles in biotech/pharma.

Do not proceed with resume or cover letter generation until both files are provided.
```

---

## 🧩 Concepts Behind This Prompt

### ✅ Persona Injection

It uses role-based priming to define the LLM's behavior. By saying "Take on the persona..." you help the LLM maintain consistent output tailored to a domain.

### ✅ Step-by-step Control

The task breakdown forces the model to execute in **sequenced stages**, ensuring it doesn't skip ahead before gathering inputs.

### ✅ ATS Optimization

This leverages the LLM’s ability to extract keywords and apply semantic rewriting — an essential for modern resumes.

### ✅ Human-in-the-Loop Confirmation

Rather than blindly overwriting content, the prompt **requires user confirmation** after proofreading. This builds trust and avoids accidental errors.

---

## 🛠 How to Tweak It

| Use Case            | How to Modify                                                                           |
| ------------------- | --------------------------------------------------------------------------------------- |
| Other roles         | Replace "computational chemistry" with e.g., "data science", "regulatory affairs", etc. |
| Auto-run mode       | Remove the user confirmation step for fully automated pipelines                         |
| PDF output          | Add a step to convert DOCX to PDF                                                       |
| Conversational flow | Add follow-up questions to personalize resume tone/style                                |
| No job description  | Add fallback logic to enhance resume using general best practices                       |

---

## 📤 Suggested Usage

* Paste into your LLM interface or script
* Upload resume and job description when prompted
* Review proofreading notes
* Confirm edits and download final documents

---

## 📎 License

MIT License — Free to reuse, modify, and distribute.

---

## 🙌 Acknowledgment

Crafted with help of chatgpt!
