<div align="center">

# 🚀 AI Resume Analyzer & Job Matcher

## A cutting-edge career tool that transforms the job application process from a guessing game into a data-driven strategy.

This application leverages the power of Large Language Models to provide job seekers with instant, intelligent, and actionable feedback, helping them stand out in a competitive market.

</div>

---

# 🎯 The Problem & The Solution

In today's job market, applicants face three critical challenges:
1.  **Resume Uncertainty:** Is my resume good enough? What are its weak points?
2.  **Tailoring Fatigue:** Manually customizing a resume for every single job application is tedious and time-consuming.
3.  **The "ATS Black Box":** Will my resume be correctly read by automated screening systems?

This project directly addresses these pain points by offering a sophisticated, user-friendly platform that acts as a personal career coach. It provides both a general "health check" for a resume and a powerful tool to precisely align it with a specific job description, ensuring every application is as strong as it can be.

# ✨ Core Features

This application is built with a focus on providing a seamless and powerful user experience.

#### **1. AI-Powered Resume Grader**
* Upload any PDF resume for a comprehensive analysis.
* Receives an overall score on a 1-10 scale, providing a simple benchmark of quality.
* The AI identifies areas for improvement and suggests relevant skills to add, helping users strengthen their profile.

#### **2. Dynamic Job Description Matcher**
* Paste any job description and upload a resume to see how well they align.
* Get a precise **match score (1-100%)** that quantifies the fit between the resume and the role.
* The AI extracts **missing keywords** from the job description that should be included in the resume.
* Receive **actionable, tailored suggestions** on how to rephrase bullet points, highlight specific projects, and align the summary with the employer's needs.

#### **3. Interactive & Animated UI/UX**
* The interface is built with **React** and **Framer Motion** to deliver a fluid, engaging experience.
* Results are displayed in a stylish, modern modal with animations that guide the user's eye, including an animated score counter and staggered list reveals.
* The UI is fully responsive and designed for a clean, professional aesthetic.

#### **4. Session-Based History with localStorage**
* All resume analyses are automatically saved to browser **localStorage** during your session.
* Users can review and compare their analysis reports in the "Resume History" tab.
* Full **CRUD operations** - view, and delete analyses from history.
* **Privacy-First:** All data stays in your browser - nothing sent to external servers.
* **Session-Based:** History clears when you close the browser for automatic cleanup.

# 🛠️ Technical Architecture & Workflow

The project is built on a modern, client-side architecture that is efficient, private, and fast.

#### **Data Flow Diagram**
```
[User] --(1. Upload PDF & JD)--> [React Frontend]
   ^                                     |
   |                               (2. Extract Text w/ PDF.js)
   |                                     |
(5. Display Results) <------------------ v
   |                         [Google Gemini API] <--(3. Send Prompt)-- [Service Logic]
   |                                     |
[localStorage] <--(4. Save History)-----|--(4. Receive JSON)
```

#### **Technology Breakdown**

* **Frontend (React & Vite):** A modern, fast, and scalable foundation for the user interface.
* **AI Engine (Google Gemini 2.5 Flash):** Chosen for its powerful instruction-following capabilities and its ability to return structured, reliable JSON output, which is crucial for parsing and displaying the analysis results.
* **Storage (localStorage):** Browser-based storage for session history. Privacy-first approach - all data stays in your browser and clears on session end.
* **PDF Parsing (PDF.js):** Text extraction is handled entirely on the client-side for speed and privacy. This avoids the need to upload and store sensitive user files on a server.
* **Deployment (Netlify):** Connected via GitHub for seamless Continuous Integration and Continuous Deployment (CI/CD). Environment variables are managed securely through the Netlify UI.

<img width="1890" height="869" alt="image" src="https://github.com/user-attachments/assets/c7e94aef-974b-4a3a-bc72-97eeb93114d7" />
<img width="1910" height="851" alt="image" src="https://github.com/user-attachments/assets/2e1a9502-26b3-434b-a997-e88a592ea805" />
<img width="1877" height="866" alt="image" src="https://github.com/user-attachments/assets/1219ffdd-7cec-4804-a6fb-1a3b15963a01" />
<img width="1918" height="871" alt="image" src="https://github.com/user-attachments/assets/d425893e-dbf3-4e96-b588-fcce52052f81" />


---

# ✍️ Author

**Greeshmanth Reddy Bommireddy**

 [**GitHub**](https://github.com/GreeshmanthBommireddy) 

---

# 📄 License

This project is open source and available under the [MIT License](LICENSE).


# ⭐ Show Your Support

If you find this project helpful, please give it a ⭐ on GitHub!
