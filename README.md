<h1 align="center">Hi, I'm Divvij</h1>

<p align="center">
  <b>Full-stack &amp; AI developer</b> — web platforms, multi-agent systems and ML pipelines<br/>
  Tech team · <a href="https://github.com/ecellbits">E-Cell, BITS Pilani Hyderabad</a>
</p>

<p align="center">
  <a href="https://saul-goodman-courtroom.vercel.app"><img alt="Live demo" src="https://img.shields.io/badge/live_demo-saul--goodman--courtroom-0d1117?style=flat-square&logo=vercel&logoColor=white"/></a>
  <a href="https://github.com/ecellbits/Ecell_Web"><img alt="E-Cell website" src="https://img.shields.io/badge/E--Cell_website-%232_contributor-0d1117?style=flat-square&logo=github&logoColor=white"/></a>
</p>

---

### About

- I build products end to end: **React / Next.js** front ends, **Python** and **Node** back ends, shipped on **Vercel** and **Firebase**.
- Currently exploring **computer vision for pathology, multi-agent systems, game theory, retrieval-augmented generation** and **applied deep learning**.
- I care about correctness you can prove: deterministic simulations, exact arithmetic and test suites that fail loudly.

### Featured work

#### 🔬 [AI Pathologist](https://github.com/Divvij0202/ai-pathologist) · OpenCV AI Competition 2026

An agent that reads gigapixel lymph-node slides the way a pathologist does: it surveys the slide at low zoom, zooms in only where the tissue looks suspicious, follows tumour to its edges and stops when it has enough evidence.

- **OpenCV 5** does all the pixel work: tissue detection (HSV, Otsu, morphology, contours), Reinhard and Macenko stain normalisation, lesion measurement with `minAreaRect`, and the ONNX tile classifier through `cv.dnn`
- ResNet-18 tile classifier trained on PatchCamelyon (262k training patches) and temperature-calibrated: **0.958 test AUC**; on a held-out slide it found all 4 macrometastases while viewing **8% of the tissue**
- Slides stream from the public CAMELYON16 bucket on S3 by HTTP range reads, so a 3 GB slide is never downloaded; Claude on Amazon Bedrock chooses the search strategy, while the look budget and safety rules live in code
- Research prototype and second reader only, not a diagnostic tool

`Python` `OpenCV 5` `PyTorch` `ONNX` `Claude / Bedrock` `FastAPI`

#### ⚖️ [Saul Goodman Courtroom](https://github.com/Divvij0202/saul-goodman-courtroom) · [live demo](https://saul-goodman-courtroom.vercel.app)

Prosecution and defense AI agents compete to build the strongest case from structured evidence, in front of a fully deterministic judge.

- The judge rules on objections and weighs evidence element by element in **exact rational arithmetic** (no floats in any decision), with a **SHA-256 hash-chained audit trail**
- A game-theory layer estimates payoff matrices by Monte Carlo and solves them for **exact pure and mixed Nash equilibria**
- Terminal dashboard, web UI + FastAPI server, a bit-for-bit determinism verifier and a 2,500-trial fuzz harness, backed by **483 tests**

`Python` `FastAPI` `Pydantic` `Game theory` `Multi-agent simulation`

#### 🚀 [E-Cell BITS Pilani Hyderabad website](https://github.com/ecellbits/Ecell_Web) · [live](https://ecell-web-vercel.vercel.app)

**#2 all-time contributor (78 commits)** to the official website of the campus entrepreneurship cell.

- Built the passes and ticketing flow (KonfHub integration), the Campus Ambassador programme, and the accommodation and corporate-pass pages
- Ran a performance pass across the site: image optimisation, lazy loading and smooth scrolling, while keeping Vercel CI builds green

`React` `Tailwind CSS` `Framer Motion` `GSAP` `Vercel`

#### 🎓 [CampusFlow ERP](https://github.com/Divvij0202/erp-portal-frontend)

An ERP platform for educational institutions that covers the whole academic lifecycle.

- Role-based dashboards for admins, staff and students, with approval workflows for registrations and requests
- Departments, courses, sections and personalised timetables; session-based attendance and assignments
- Reporting with Recharts, PDF export (jsPDF) and CSV export (PapaParse)

`React` `Vite` `Firebase Auth / Firestore / Storage` `Tailwind CSS`

#### 🌊 [AntarBodh](https://antarbodh-demo.vercel.app) · Smart India Hackathon

A deep-learning framework that reconstructs subsurface ocean temperature at 15 depths (0–1000 m) across the North Indian Ocean from surface observations. I contributed to the model training pipeline.

`Python` `Deep learning` `Oceanographic data`

#### 📈 [ACM Quant](https://github.com/Divvij0202/ACM_Quant)

Quant finance exercises: SMA-crossover trading signals, rolling return and volatility analysis, and portfolio valuation on live market data.

`Python` `pandas` `yfinance` `matplotlib`

### Tech stack

| | |
|---|---|
| **Languages** | <img height="36" src="https://skillicons.dev/icons?i=python,cpp,js,ts&theme=dark"/> |
| **Frontend** | <img height="36" src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite&theme=dark"/> |
| **Backend & data** | <img height="36" src="https://skillicons.dev/icons?i=fastapi,nodejs,express,mongodb,firebase,supabase&theme=dark"/> |
| **ML** | <img height="36" src="https://skillicons.dev/icons?i=pytorch,opencv&theme=dark"/> |
| **Tooling** | <img height="36" src="https://skillicons.dev/icons?i=git,github,vercel,vscode&theme=dark"/> |
