# LUMI AI Factory — consolidated overview

Condensed from a snapshot of the 49 public pages of <https://lumi-ai-factory.eu/>, taken
2026-11-23 (© 2026 LUMI AI Factory). Each fact is followed by a link to the page it came from,
so that answers can point readers to the right page. Navigation, repeated boilerplate and
marketing prose were removed. Blog posts, news, success stories, trainings and events are listed
by title, date and link in §11. Only their titles were in the snapshot, not their full text. The
live website is authoritative. Dates, models and call deadlines go stale.

Key entry points:
- [Home](https://lumi-ai-factory.eu/)
- [Service catalogue](https://lumi-ai-factory.eu/service-catalogue/)
- [AI self-assessment survey](https://lumi-ai-factory.eu/ai-self-assessment-survey/)
- [Contact form](https://lumi-ai-factory.eu/contact-us/)
- [User support](https://lumi-ai-factory.eu/user-support/)
- [FAQ](https://lumi-ai-factory.eu/faq/)
- [Glossary](https://lumi-ai-factory.eu/glossary/)
- [Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)
- [Success stories](https://lumi-ai-factory.eu/success-stories/)
- [News](https://lumi-ai-factory.eu/about-us/news/)
- [Trainings](https://lumi-ai-factory.eu/trainings/)
- [Events](https://lumi-ai-factory.eu/events/)
- [Media gallery](https://lumi-ai-factory.eu/about-us/media/)

---

## 1. What it is

Sources: [About us](https://lumi-ai-factory.eu/about-us/) ·
[FAQ](https://lumi-ai-factory.eu/faq/) ·
[Enter the LUMI AI Factory](https://lumi-ai-factory.eu/enter-the-lumi-ai-factory/) ·
[Your AI Journey](https://lumi-ai-factory.eu/your-ai-journey/)

The **LUMI AI Factory (LUMI AIF)** is one of Europe's first AI Factories: a one-stop shop that
combines **supercomputing, curated data and AI expertise** to help organisations develop AI, from
first idea to proof of concept to scaling. It runs on the LUMI supercomputer today and will
move to the AI-optimised **LUMI-AI** system, with an experimental quantum platform called
**LUMI-IQ**. Its services are designed as one connected "AI journey" that you can join at any
stage.

- **Why it exists:** the European Commission's *AI Innovation Package* (January 2024) created AI
  Factories to give startups, SMEs and researchers easy access to compute, data and expertise,
  and to strengthen European competitiveness and technological sovereignty
  ([FAQ](https://lumi-ai-factory.eu/faq/); EuroHPC's
  [AI Factories FAQ](https://www.eurohpc-ju.europa.eu/ai-factories/faqs-ai-factories_en)).
- **Funding and operation:** EU funding plus national contributions from the consortium
  countries. It is hosted by CSC and run as a non-profit service platform
  ([FAQ](https://lumi-ai-factory.eu/faq/)).
- **Purpose of use:** research, development and innovation (RDI), not production services
  (see §9).
- **Focus sectors:** Health and Life Sciences, Manufacturing, and Communication Technologies and
  Networks. Other sectors are also welcome
  ([Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)).
- **Speed:** from first contact to active work in **as little as 2–5 days**
  ([Enter the LUMI AI Factory](https://lumi-ai-factory.eu/enter-the-lumi-ai-factory/)).
- **Part of a network:** LUMI AIF belongs to Europe's
  [network of AI Factories](https://www.eurohpc-ju.europa.eu/ai-factories_en).

### Who runs it

Sources: [EuroHPC JU](https://lumi-ai-factory.eu/about-us/eurohpc-ju/) ·
[LUMI AIF Consortium](https://lumi-ai-factory.eu/about-us/lumi-aif-consortium/) ·
[Computing infrastructure](https://lumi-ai-factory.eu/about-us/computing-infrastructure/) ·
[Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)

| Role | Who |
|---|---|
| Funder, and owner of LUMI | **[EuroHPC Joint Undertaking](https://www.eurohpc-ju.europa.eu/index_en)** (EU + participating countries + private partners; founded 2018, based in Luxembourg; 37 countries have signed the EuroHPC Declaration; legal basis Council Regulation (EU) 2021/1173, amended by 2024/1732). EuroHPC JU grants access to half of LUMI's resources. |
| Host and coordinator | **[CSC – IT Center for Science](https://www.csc.fi/en/)** (Finland): a non-profit company owned by the Finnish state and Finnish higher-education institutions |
| LUMI AIF consortium (6 countries) | **Finland:** CSC, [Aalto University](https://www.aalto.fi/en/), [AI Finland](https://aifinland.fi/en/front-page/), [University of Helsinki](https://www.helsinki.fi/en) · **Czechia:** [IT4Innovations](https://www.it4i.cz/) (VSB – Technical University of Ostrava) · **Denmark:** [DeiC](https://deic.dk/) · **Estonia:** [University of Tartu](https://ut.ee/en) · **Norway:** [Sigma2](https://www.sigma2.no/) · **Poland:** [ACC Cyfronet AGH](https://www.cyfronet.pl/pl) |
| AI Factory Antennas linked to LUMI AIF | Belgium, Iceland, Latvia, Switzerland ([news, 2025-10-13](https://lumi-ai-factory.eu/articles/eurohpc-ju-ai-factory-antennas/)) |
| LUMI supercomputer consortium (11 countries, a different group) | Finland, Belgium, Czechia, Denmark, Estonia, Iceland, the Netherlands, Norway, Poland, Sweden, Switzerland |

---

## 2. Computing infrastructure

Main source: [Computing infrastructure](https://lumi-ai-factory.eu/about-us/computing-infrastructure/)

### LUMI (available now)
- Owned by EuroHPC JU and located in CSC's data centre in **Kajaani, Finland**
  ([LUMI website](https://www.lumi-supercomputer.eu)).
- **380 petaflops** sustained (HPL), about the combined power of 1.5 million laptops.
- **2,978 GPU nodes with 11,912 AMD GPUs** (the LUMI-G partition, **AMD MI250X**), plus a CPU-only
  partition, cloud services (**LUMI-K**, a Kubernetes/OpenShift container cloud) and object storage
  (**LUMI-O**, Ceph-based and S3-compatible)
  ([Glossary](https://lumi-ai-factory.eu/glossary/)).
  Architecture details:
  [LUMI's full system architecture](https://www.lumi-supercomputer.eu/lumis-full-system-architecture-revealed/).
- Around 3,500 projects have run on it, and over half of its compute has gone to AI. Up to 20% of
  its capacity is reserved for industry.
- Has a mature integration with quantum processors, has won multiple industry awards, and is
  ISO 27001 certified.

### LUMI-AI (scheduled for the second half of 2027)
- Will gradually **replace LUMI**. It is expected to bring **10× the AI capacity** and nearly 2×
  the HPC capability.
- Built by **Bull** on the liquid-cooled **BullSequana XH3500**, with **AMD Instinct MI430X GPUs**
  and 6th-gen **AMD EPYC 256-core CPUs**. IBM supplies storage (Storage Scale), Nokia supplies
  data-centre networking, and the interconnect is Bull's BXI.
- Will be located in CSC's new data centre in Kajaani. It is designed to be **multi-tenant** with
  extensive **API-based access**. Design images are in the
  [media gallery](https://lumi-ai-factory.eu/about-us/media/).
- Until LUMI-AI is available, all AIF services run on LUMI
  ([Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)).

### LUMI-IQ (experimental quantum platform, end of 2027)
Also: [Quantum services](https://lumi-ai-factory.eu/services/quantum-services/)
- First system: **IQM Halocene H4**, a superconducting quantum computer with a **150-qubit** QPU
  that combines quantum error correction (QEC) with NISQ-era qubits. It will be upgraded in phases
  towards early fault-tolerant computing, with more qubits and better error correction.
  Press releases:
  [IQM selected to deliver LUMI-IQ](https://lumi-ai-factory.eu/articles/iqm-selected-to-deliver-the-lumi-iq-quantum-computer/)
  (2026-07-08) and
  [towards Europe's first superconducting quantum computer with logical qubits](https://lumi-ai-factory.eu/articles/lumi-ai-factory-advances-toward-europes-first-superconducting-quantum-computer-with-logical-qubits/)
  (2026-09-10).
- Will include a modular QEC stack, and a software library with examples for adding quantum AI to
  existing workflows.
- Goals: build a European HPC+AI+QC infrastructure, explore quantum advantage for AI and AI for
  quantum, and create commercial activity.
- Until LUMI-IQ arrives, quantum users get the **VLQ** quantum computer (EuroHPC, connected to LUMI).

### Sustainability
Sources: [Sustainability](https://lumi-ai-factory.eu/about-us/sustainability/) ·
[LUMI: sustainable future](https://www.lumi-supercomputer.eu/sustainable-future/)

LUMI runs on **100% renewable electricity**. Its waste heat warms hundreds of Kajaani households,
and the data centre was built as a brownfield site. Finland offers low industrial electricity
prices and a stable environment. LUMI-AI will follow the same model. Related blog post:
[AI and environmental sustainability hand in hand](https://lumi-ai-factory.eu/articles/ai-and-environmental-sustainability/).

---

## 3. Who can use the services

Source: [Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)

**Organisation types** (individuals and temporary teams are **not** eligible):

| Type | Definition |
|---|---|
| SME / startup | < 250 employees and turnover ≤ €50 M and/or balance sheet ≤ €43 M (EU definition) |
| Large enterprise | > 250 employees and turnover > €50 M |
| Public service organisation | Government or publicly funded body serving society (healthcare, transport, administration…) |
| Research performing organisation (RPO) | Universities, research institutes, think tanks |

**Countries.** Services are primarily for the six consortium countries. Other EU member states
and Horizon Europe–associated countries are also eligible: Albania, Austria, Belgium, Bulgaria,
Croatia, Cyprus, Czechia, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Iceland,
Ireland, Israel, Italy, Latvia, Lithuania, Luxembourg, Malta, Moldova, Montenegro, Netherlands,
North Macedonia, Norway, Poland, Portugal, Romania, Serbia, Slovakia, Slovenia, Spain, Sweden,
Switzerland, Türkiye and the United Kingdom. Official references: the
[Horizon Europe associated-country list](https://ec.europa.eu/info/funding-tenders/opportunities/docs/2021-2027/common/guidance/list-3rd-country-participation_horizon-euratom_en.pdf)
and EuroHPC's
[supercomputer access policy](https://www.eurohpc-ju.europa.eu/supercomputers/supercomputers-access-policy-and-faq_en).

- **Consortium-country customers** can use both EuroHPC JU calls and national access routes.
- **Other eligible countries** can get compute **only through EuroHPC JU calls**.

---

## 4. What "free of charge" means

Sources: [Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/) ·
[FAQ](https://lumi-ai-factory.eu/faq/) ·
[Powerful AI computing](https://lumi-ai-factory.eu/services/powerful-ai-computing/)

For eligible startups and SMEs (and researchers and the public sector through the science calls),
**the EU and national funders pay for compute time, training, data access and expert
consultation**. The customer contributes their own ideas, people and time.

- It is not unlimited. LUMI AIF helps you **estimate the resources** you need and **apply** for
  them. A small pilot usually comes first.
- **IPR, data, models and outputs remain the customer's.** LUMI AIF takes no IPR and no equity.
- **Reporting:** EU calls need a short, non-confidential final report and an acknowledgement of
  LUMI AIF / EuroHPC JU. Trade secrets don't have to be disclosed, and an NDA can cover sensitive
  parts.
- **State aid:** national free access (e.g. a
  [Business Finland computing-capacity grant](https://www.businessfinland.fi/globalassets/finnish-customers/02-build-your-network/digitalization/quantum-computing/laskentatuki-computing-grant.pdf))
  counts as state aid. The company must check that it has not used up its de minimis allowance
  (max **€300,000 over three years**) and must report the value of the resources used, which
  LUMI AIF provides.
- **Large companies** don't get free access as a rule. They can pay, join an EU- or nationally
  funded collaborative R&D project, or use Fast Lane for open science (see §5).
- **Paid (commercial) access**, currently for Finnish companies, is faster, has **no publication
  requirement**, and is priced from the
  [CSC/LUMI service price list](https://csc.fi/en/about-us/customers/high-performance-computing-for-companies/#service-price-list).
- **Openness:** because the service is publicly funded, LUMI AIF publishes success stories, while
  respecting trade secrets and IPR ([FAQ](https://lumi-ai-factory.eu/faq/)).
- **Prices for consultation** follow the price list of whichever consortium country delivers it.
  Commercial customers are invoiced for actual use. Free customers are told the value of what
  they used, for state-aid reporting.
- **Datasets** are free, but you need a LUMI project to use them. External data providers may
  invoice you directly.
- **Training** is free for participants from eligible countries. Large companies should
  [ask](https://lumi-ai-factory.eu/contact-us/).

---

## 5. Compute access options

Category page: [Powerful AI computing](https://lumi-ai-factory.eu/services/powerful-ai-computing/).
All EuroHPC access modes use LUMI's GPU partition (AMD MI250X), come with onboarding and technical
support, and have **rolling applications**. EuroHPC's overview:
[AI Factories access modes](https://www.eurohpc-ju.europa.eu/ai-factories/ai-factories-access-modes_en).

| Access mode | For whom | Compute | Duration | Selection and time to access | Cost |
|---|---|---|---|---|---|
| **[Playground](https://lumi-ai-factory.eu/playground-access-to-lumi-ai-factory/)** ([EuroHPC](https://www.eurohpc-ju.europa.eu/playground-access-ai-factories_en)) | EU SMEs and startups | **5,000 GPU h** | 1, 2 or 3 months | Short template application, first come first served, eligibility + technical check; **access within ~2 working days** | Free |
| **[Fast Lane](https://lumi-ai-factory.eu/fast-lane-access-to-lumi-ai-factory/)** ([EuroHPC](https://www.eurohpc-ju.europa.eu/fast-lane-access-ai-factories_en)) | EU SMEs and startups; large enterprises only for open science with published results | **Up to 50,000 GPU h** | 1, 2 or 3 months | Short template application; one system only | Free for SMEs; free for large firms doing open science, otherwise paid |
| **[Large Scale](https://lumi-ai-factory.eu/large-scale-access-to-lumi-ai-factory/)** ([EuroHPC](https://www.eurohpc-ju.europa.eu/large-scale-access-ai-factories_en)) | SMEs and startups with mature projects | **Over 50,000 GPU h** (up to millions) | Up to 12 months | Peer review by LUMI AIF's Industry Innovation Group (innovation, impact, ethics); two cut-offs per month; access within 10 working days of a cut-off. **No resources left for 2026.** | Free |
| **[AI for Science & Collaborative EU Projects](https://lumi-ai-factory.eu/ai-for-science-and-collaborative-eu-projects-access-to-lumi-ai-factory/)** ([EuroHPC call](https://www.eurohpc-ju.europa.eu/eurohpc-ju-call-proposals-ai-science-and-collaborative-eu-projects_en)) | Scientific users, universities, research organisations, public sector, and industry partners in Horizon Europe / Digital Europe projects | Node hours according to the approved workload | 6 months | Technical + expert peer review (excellence, innovation and impact, quality of implementation); cut-offs (remaining in 2026: 30 Oct and 11 Dec, 10:00 CET); access up to 1 month after a cut-off | Free |
| **[Try&Buy](https://lumi-ai-factory.eu/trybuy/)** | **Finnish companies only** (Finnish business ID, trade-sanctions / export / dual-use checks) | 1,000 GPU h + 10,000 CPU h + 10,000 TiB units; 2 users; 1 day of expert support | 3 months (or until used up) | Meeting with a customer manager; access within a few working days; **no application and no public report** | Free, then pay as you go |

- Academia and the public sector are **not** eligible for Playground, Fast Lane or Large Scale.
  They use the *AI for Science* call. Large enterprises use paid or national access.
- The three industry modes are EuroHPC's **"AI for Industrial Innovation"** call. Their final
  report is due **within 3 months** after the allocation ends and covers: a project summary,
  services used, a non-confidential technical outline (plus benchmarks for Fast Lane, and
  scalability results for Large Scale), and an acknowledgement. *AI for Science* also needs a
  Scope & Plan and a Progress Report.
- **Typical workloads by size:** Playground covers first experiments, fine-tuning, NVIDIA→AMD
  portability tests and prototyping. Fast Lane covers iterative training, benchmarking,
  medium-scale training and inference optimisation. Large Scale covers foundation-model training,
  hyperparameter sweeps, distributed training and production-inference benchmarking.
- Other national routes: in Finland, nationally funded RDI projects with academia, and the
  Business Finland computing-capacity grant
  ([Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)).
- Further reading: [Why supercomputing and LUMI?](https://lumi-ai-factory.eu/articles/blog-why-supercomputing-and-lumi/)
  (blog, 2026-03-19). The [Enter the LUMI AI Factory](https://lumi-ai-factory.eu/enter-the-lumi-ai-factory/)
  page shows an example comparing training times on LUMI and on a laptop.

---

## 6. Other services

Consultation is **free for startups and SMEs** from EU or Horizon-associated countries. Requests
go through the [contact form](https://lumi-ai-factory.eu/contact-us/), where you choose an inquiry
type. A **Customer Manager** then follows up.

### Getting started and business development
Category page: [Expert support for AI business development](https://lumi-ai-factory.eu/services/expert-support-for-ai-business-development/)
- **[Start Your AI Journey](https://lumi-ai-factory.eu/start-your-ai-journey/)**: a needs
  analysis based on the [AI self-assessment survey](https://lumi-ai-factory.eu/ai-self-assessment-survey/)
  or a direct consultation. For startups, SMEs, large enterprises, research and the public
  sector. No technical preparation is needed.
- **[AI Starter Pack](https://lumi-ai-factory.eu/ai-starter-pack/)**: a guided path for SMEs and
  startups, completed **within 3 months**. It runs from needs mapping, through training
  suggestions, consultation and trustworthy-AI and AI Act basics, to applying for Playground (or
  Try&Buy) and building a proof of concept. Needs mapping and consultations take about a month.
  Inquiry type: "AI Starter Pack".
- **[Resource access proposal support](https://lumi-ai-factory.eu/resource-access-proposal-support/)**:
  finds the right resource route (EuroHPC, national), provides templates and a preparation
  checklist, and reviews drafts. Also available for proposals that don't target LUMI. You need
  technical details of your stack, a goal and a work plan with a Principal Investigator.
- **[Grant proposal consultation](https://lumi-ai-factory.eu/grant-proposal-consultation/)**:
  technical validation of the AI/HPC parts of Horizon Europe, Digital Europe or national grant
  applications. LUMI AIF may even join the consortium as a partner. Bring a draft, a resource
  estimate and your deadline.

### Expert support for AI development
Category page: [Expert support for AI development](https://lumi-ai-factory.eu/services/expert-technical-support-for-ai-development/).
Explainer: [What is LUMI AI Factory's AI expert consultation?](https://lumi-ai-factory.eu/articles/ai-expert-consultation/)
(blog, 2026-04-22). Support is available before you have LUMI access and until the agreed amount
is used, online or on site. Experts work office hours in Finnish time (EET/EEST).
Inquiry type: "Expert technical support for AI development".
- **[Implementing an HPC & AI project](https://lumi-ai-factory.eu/expert-support-for-implementing-an-hpc-ai-project/)**:
  planning, software installation and project setup, especially for first-time users. Large
  businesses pay (in Finland).
- **[Consultation on AI methods](https://lumi-ai-factory.eu/consultation-on-ai-methods/)**:
  choosing and implementing methods, mainly deep neural networks that need GPUs or HPC. For
  larger assignments beyond the service desk.
- **[Training distributed AI models](https://lumi-ai-factory.eu/expert-support-on-training-distributed-ai-models/)**:
  framework configuration, scaling laws, optimisation and debugging for runs on hundreds or
  thousands of GPUs. Pair it with Large Scale access. Results must be open unless you pay for
  compute. Large companies pay.
- **[AI or HPC optimisation](https://lumi-ai-factory.eu/consultation-on-ai-or-hpc-optimisation/)**:
  profiling and tuning your own or third-party code, for problems such as GPU utilisation, I/O
  bottlenecks, multi-node scaling, memory and portability.

### Data lab
Category page: [LUMI AI Factory data lab](https://lumi-ai-factory.eu/services/lumi-ai-factory-data-lab/).
Inquiry type: "LUMI AI Factory data lab".
- **[LUMI Datasets as a Service (DaaS)](https://lumi-ai-factory.eu/dataset-as-a-service/)**:
  curated, AI-ready datasets stored next to LUMI, run in cooperation with EOSC Finland. Datasets
  are free, but you need a LUMI project with resources to use them. Some datasets are restricted
  and need an application. **Data providers** publish a *use copy* while keeping ownership and
  control, at no cost to them, and the catalogue is curated.
  [Data catalogue](https://lumi-aif.fairdata.fi/) ·
  [User guide](https://docs.lumi-supercomputer.eu/laif/data/daas_guide/) ·
  [Terms of use](https://lumi-ai-factory.eu/terms-of-use-of-lumi-ai-factory-dataset-as-a-service/) ·
  [News: data close to compute](https://lumi-ai-factory.eu/articles/dataset-as-a-service/) (2026-04-01)
- **[Initial risk analysis – EU AI Act Compliance Checker](https://lumi-ai-factory.eu/initial-risk-analysis-consultation-eu-ai-act-compliance-checker/)**:
  one 1-hour online session using the EU AI Office's
  [Compliance Checker](https://ai-act-service-desk.ec.europa.eu/en/eu-ai-act-compliance-checker)
  to find your system's likely risk class and obligations.
- **[Expert consultation on Trustworthy AI development](https://lumi-ai-factory.eu/expert-consultation-on-trustworthy-ai-development/)**:
  a series of 1-hour online sessions covering scoping and risk analysis, guidance on the AI Act,
  GDPR and trustworthy-AI principles, a risk and gap review (e.g. bias), and recommendations.
  Related blog posts:
  [Trustworthy AI: Turning compliance into competitive advantage](https://lumi-ai-factory.eu/articles/trustworthy-ai-turning-compliance-into-competitive-advantage/)
  (2026-07-01) and
  [Machine learning on sensitive data](https://lumi-ai-factory.eu/articles/real-4-reg/) (2025-10-24).
- Both AI Act services are **non-binding guidance, not legal advice**. They are open to all
  organisation types and free for SMEs and startups.

### AI software and solutions
Category page: [AI software and solutions](https://lumi-ai-factory.eu/services/ai-software-and-solutions/)
- **[AI Software Environment](https://lumi-ai-factory.eu/ai-software-environment/)**: ready-to-use,
  layered **containers** built on ROCm, MPICH and libfabric, with PyTorch for AMD, MPI and a full
  AI/ML stack (DeepSpeed, Flash Attention, vLLM, xFormers, Hugging Face, Jupyter, MLflow, NumPy,
  pandas, SciPy). They are optimised for LUMI and meant to be extended. All recipes, build logs,
  SBOMs and images are public. On LUMI they are in `/appl/local/laifs/containers/`. Elsewhere:
  [Docker Hub](https://hub.docker.com/u/lumiaifactory) ·
  [GitHub recipes](https://github.com/lumi-ai-factory/laifs-container-recipes/releases) ·
  [Documentation](https://docs.lumi-supercomputer.eu/laif/software/ai-environment/) ·
  [LUMI AI Guide](https://github.com/Lumi-supercomputer/LUMI-AI-Guide) ·
  [Blog: benefits of the LUMI AI Software Environment](https://lumi-ai-factory.eu/articles/benefits-of-the-lumi-ai-software-environment/)
- **[Aitta ML inference service](https://lumi-ai-factory.eu/aitta-ml-inference-service/)** (by CSC):
  R&D inference on LUMI through a web UI, an **OpenAI-compatible REST API**, a Python client or
  CSC's Noppe.
  - Requires a LUMI project with compute
    ([how to get one](https://docs.lumi-supercomputer.eu/firststeps/accessLUMI/)). During the
    pilot, users needed an invite, requested via
    [user support](https://lumi-ai-factory.eu/user-support/). Free for invited pilot users. Large
    businesses can't use it free of charge.
  - **Not** for production services, for sensitive or personal data, or for use cases that need
    an instant response (resources are allocated on demand).
  - Models listed on the page: Gemma-4-31b-it, Llama-3.3-70B-Instruct, OLMo-7B, gpt-oss-120b,
    Poro-34B-chat, Llama-Poro-2-70B-Instruct, TinyLlama-1.1B, Qwen3.6-27B, Qwen3.6-35B-A3B,
    Qwen3-Coder-Next, Ministral-3-14B-Reasoning, Tower-Plus-9B (translation), and
    Apertus-70B/8B. There are also embedding, reasoning and coding models.
- **Infrastructure for AI agents:** an OpenCode coding-agent container for LUMI, and a public
  **MCP server** that answers questions about LUMI
  ([AI software and solutions](https://lumi-ai-factory.eu/services/ai-software-and-solutions/)).
- Also: the **EXA4MIND** inference service, containerised workflows (text and image
  processing), and **LUMI HPC-APIs**. An MLOps environment (MLflow, Kubeflow) is planned.

### Quantum services
Category page: [Quantum services](https://lumi-ai-factory.eu/services/quantum-services/).
Inquiry type: "Quantum services".
- **[Quantum computing resource access](https://lumi-ai-factory.eu/quantum-computing-resource-access/)**:
  hybrid quantum + HPC + AI pipelines, simulators and a development stack. Uses VLQ and LUMI now,
  and LUMI-IQ and LUMI-AI later. Academics apply via national or EuroHPC allocations, industry via
  EuroHPC. Free for eligible users.
- **[Quantum expert support and consulting](https://lumi-ai-factory.eu/quantum-expert-support-and-consulting/)**:
  checks whether a problem suits quantum, helps with the LUMI-IQ software stack and with
  applications, and provides training material. Free for academics, SMEs and startups.

### Training
Category page: [Training and skills development](https://lumi-ai-factory.eu/services/training-skills-development/) ·
service: [Customer training on large-scale AI & HPC](https://lumi-ai-factory.eu/customer-training-on-large-scale-ai-hpc/) ·
[training catalogue](https://lumi-ai-factory.eu/trainings/)

Courses on deep learning and efficient HPC, from AI fundamentals to quantum machine learning.
They are delivered online, on site, as workshops, webinars and hackathons, and as self-paced
modules, including domain tracks (e.g. health). Training can be combined with consultation, and
you can suggest topics. **Free** for participants from eligible countries. Courses are listed in §11.

### Ecosystem and networking
Category page: [AI ecosystem and networking](https://lumi-ai-factory.eu/services/ai-ecosystem-and-networking/).
Related blog post: [Towards a competitive European AI ecosystem](https://lumi-ai-factory.eu/articles/towards-a-competitive-european-ai-ecosystem/) (2025-12-04)
- **[AI Factory Hubs](https://lumi-ai-factory.eu/hubs/)**, physical co-working spaces:
  - **Otaniemi** (Espoo, Aalto, TUAS building, Maarintie 8, 4th floor): 121 m², visits on
    request, courses, hackathons, reading clubs and PhD breakfasts. Contact: otaniemi.hub@aalto.fi
    ([Finland hubs](https://lumi-ai-factory.eu/finland-lumi-ai-factory-hubs/#otaniemi))
  - **Kumpula** (Helsinki, University of Helsinki, Exactum, Pietari Kalmin katu 5): an AI for
    Science focus,
    [online research-software-engineering help sessions](https://tapahtumat.helsinki.fi/en-FI/page/68df95bc281b450007745e56/research-software-engineering-online-help-sessions)
    for PhD students and postdocs, and collaboration with research groups
    ([Finland hubs](https://lumi-ai-factory.eu/finland-lumi-ai-factory-hubs/#kumpula))
  - **Ostrava** (Czechia, VIVA building, Technologická 375/5, near IT4I): 32 workstations,
    residencies of 3–12 months or day passes, 2+ events a month and an AI Campus for students.
    Members are selected on mission relevance (10%), technical depth (20%), community potential
    (20%) and other criteria. Applicants must be registered companies in EuroHPC countries.
    Contact: ai-factory-hub@it4i.cz
    ([Czechia hub](https://lumi-ai-factory.eu/czechia-lumi-ai-factory-hub/))
  - Companies, student groups and research groups can host events at the hubs. A code of conduct
    applies, covering respect, data protection, labelling synthetic content, verifying model
    output and respecting licences ([Hubs](https://lumi-ai-factory.eu/hubs/)).
- **[AI expert talks](https://lumi-ai-factory.eu/ai-expert-talks/)**: free speakers (5–30 min,
  in English) for your event. Travel costs are agreed case by case.
- **[AI Matchmaking for Finland](https://lumi-ai-factory.eu/ai-matchmaking-for-finland/)**:
  AI Finland's [10x platform](https://10x.aifinland.fi), which matches AI needs with partners.
  Finnish organisations only, free.
- **[AI Expert Tour](https://lumi-ai-factory.eu/ai-expert-tour/)**: informal expert meetups in
  European cities, especially for startups and SMEs.
- **[Venture Incubation program](https://lumi-ai-factory.eu/incubation-program/)** (with
  [28DIGITAL](https://28digital.eu) and [Multilayer](https://multilayer.io)): free, no equity
  taken, 12 weeks online (Feb–May 2027), for 10 early-stage AI startups. Includes LUMI compute,
  technical and business mentoring, and a Demo Day in Espoo. Open to companies in the consortium
  and Antenna countries. **[Apply via F6S](https://www.f6s.com/lumi-ai-factory-x-28digital/apply)
  by 11 January 2027, 17:00 CET.**
  - Info sessions:
    [30 Nov](https://events.teams.microsoft.com/event/f76fa151-afcc-4f4e-b3c4-7bcdac7ad8f1@7c3574d4-f2c2-4447-bd77-d3c3cc68be6e)
    and
    [14 Dec](https://events.teams.microsoft.com/event/302d65dd-5e97-4a02-aa8c-4f5e1d25138f@7c3574d4-f2c2-4447-bd77-d3c3cc68be6e).
  - Questions: Christian.Kunze@28digital.eu

---

## 7. Security, data and compliance

Source for everything in this table: the [FAQ](https://lumi-ai-factory.eu/faq/), which links to
the relevant LUMI documentation pages.

| Topic | Answer |
|---|---|
| Data location | LUMI data centre, Kajaani, Finland, operated by CSC |
| Certifications | CSC is ISO 27001 certified since 2013, with LUMI hosting in scope. National security authority approval for physical security and security management. |
| NIS2 | LUMI is critical IT infrastructure and is NIS2 compliant (via ISO 27001 scope and incident reporting to the national authority) |
| GDPR | [LUMI privacy notice](https://www.lumi-supercomputer.eu/privacy-notice-for-processing-of-user-data-on-the-lumi-service/) |
| Encryption at rest | **Not automatic.** Encrypt your data yourself if needed ([storage docs](https://docs.lumi-supercomputer.eu/storage/)). |
| Encryption in transit | Depends on the protocol. TLS and SSH encrypt by default. SSH keys must be RSA-4096 or **ed25519** (preferred) ([SSH keys](https://docs.lumi-supercomputer.eu/firststeps/SSH-keys/)). |
| Access control | Private home directory, plus a project directory visible only to project members (Unix/POSIX permissions) |
| Visibility to others | All users can see basic Slurm queue metadata: user name, project, node count and output directory |
| Identity | Federated, token-based authentication. Time-limited, revocable credentials. Usernames may reveal some details. |
| Admin access to your data | Only at your request or during an incident, which is handled under a certified incident-response process with notification |
| Training on your data | **Never.** |
| Backups | **No backups of user data.** Keep your own copies outside LUMI ([storage docs](https://docs.lumi-supercomputer.eu/storage/)). |
| After the project ends | Data stays accessible for **90 days**, then it is deleted |
| Data transfer | rclone, s3cmd, restic via LUMI-O ([clients](https://docs.lumi-supercomputer.eu/storage/lumio/clients-general/), [sharing](https://docs.lumi-supercomputer.eu/storage/lumio/advanced/)). Login nodes have internet access. |
| Containers | Singularity / Apptainer ([docs](https://docs.lumi-supercomputer.eu/software/containers/singularity/)) |
| Logs | Security logs in CSC central storage for 6 months to 5 years, admins and security team only |
| Monitoring | [Public status dashboard](https://metrics.hpc.csc.fi/grafana/d/-8RWOzyVz/lumi-public-status) |
| NDAs | Not needed for standard projects; can be negotiated case by case via the [contact form](https://lumi-ai-factory.eu/contact-us/) |
| Liability | Use is at the user's own risk ([LUMI General Terms of Use](https://www.lumi-supercomputer.eu/lumi-general-terms-of-use_1-0/)) |

---

## 8. Getting started and support

Sources: [Enter the LUMI AI Factory](https://lumi-ai-factory.eu/enter-the-lumi-ai-factory/) ·
[Start Your AI Journey](https://lumi-ai-factory.eu/start-your-ai-journey/) ·
[User support](https://lumi-ai-factory.eu/user-support/)

1. Fill in the [AI self-assessment survey](https://lumi-ai-factory.eu/ai-self-assessment-survey/)
   or the [contact form](https://lumi-ai-factory.eu/contact-us/), choosing an inquiry type.
2. A **Customer Manager** contacts you, maps your needs and suggests services and funding routes.
3. Apply for compute (often **Playground**, or **Try&Buy** in Finland), with proposal support if
   you need it.
4. Get onboarded and start working, with expert support available along the way.

**User support:**
- [Support ticket form](https://lumi-ai-factory.eu/user-support/)
- [LUMI documentation](https://docs.lumi-supercomputer.eu)
- [LUMI service status](https://www.lumi-supercomputer.eu/lumi-service-status/)
- [Accounts and projects](https://docs.lumi-supercomputer.eu/firststeps/accessLUMI/)

---

## 9. Road to production: "train on LUMI, serve elsewhere"

Source: [Road to production](https://lumi-ai-factory.eu/user-support/road-to-production/), a guide
for startups. LUMI is an R&D system. It is not suitable for production because Slurm queues give
no guaranteed start time, there are maintenance breaks, latency depends on its location in
Kajaani, and the [terms of use](https://lumi-supercomputer.eu/termsandpolicies/) limit it to the
purpose your project was granted for. The guide recommends these steps for moving a workload
off LUMI.

1. **Know your workload:** what kind it is (an API, batch jobs, a data pipeline, an interactive
   app), its resource profile (inference needs far less than training, and quantised models need
   less still), and its dependencies (watch out for **ROCm-specific code**, since
   [LUMI-G uses AMD MI250X](https://docs.lumi-supercomputer.eu/hardware/lumig/) and most clouds
   run NVIDIA/CUDA). Decide what data moves (often just the weights), which new production data
   you will collect (user inputs, logs; watch GDPR), and how you will retrain to deal with drift.
2. **Decision criteria:**
   - *Performance:* measure latency and throughput. Older or smaller GPUs, quantisation (8/4-bit),
     and an inference server such as **vLLM** that batches requests often matter more than the
     newest hardware.
   - *Availability:* the SLA you need (99% ≈ 3.7 days of downtime a year, 99.9% ≈ 8.8 h,
     99.99% ≈ 53 min), demand peaks and autoscaling, and where your users are.
   - *Security and compliance:* GDPR, the AI Act's phased obligations, ISO 27001, and sector rules.
     For sovereignty, note that the US CLOUD Act applies to US providers even in EU regions. Model
     weights can
     [leak training data](https://not-just-memorization.github.io/extracting-training-data-from-chatgpt.html),
     so protect them like the data.
   - *Cost:* look at total cost of ownership, including idle GPUs, operations staff, monitoring,
     storage and **egress** traffic. Spot capacity is cheaper but can be taken away; reserved
     capacity is cheaper for steady load. Over a model's life, serving usually costs more than
     training, so distillation or a smaller fine-tuned model pays off.
   - *Other:* vendor lock-in (keep an exit strategy and an open stack), the model's licence, the
     provider's energy mix, and the support available.
3. **Deployment options**, from least work to most control: **managed inference** (usually the
   best first step), **cloud** VMs or managed Kubernetes, **own or co-located or bare-metal
   hardware** (even a desktop GPU under €2,000 can work for small batch jobs), and
   **multi-cloud / hybrid** (only for very high availability or regulatory needs; use
   Kubernetes and Terraform/OpenTofu).
4. **Migration and operation:**
   - Don't reuse the LUMI containers. Use `pip freeze` to get their package versions and build a
     slim serving image.
   - Compare outputs on both systems. PyTorch moves from ROCm to CUDA easily, but flash-attention,
     bitsandbytes and vLLM need the correct build for the GPU vendor.
   - Export data via [LUMI-O](https://docs.lumi-supercomputer.eu/storage/lumio/) (S3) with rclone,
     and use checksums to verify the files. Common model formats are safetensors, ONNX and GGUF.
   - Run the model as a service with vLLM; see
     [chapter 10 of the LUMI AI Guide](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/blob/main/10-LLM-inference/).
     Automate builds and deployments, run load tests and do a security review.
   - Once live, set up monitoring and alerting, rate limiting, prompt-injection protection,
     continuous evaluation, careful rollouts with rollback, and an on-call rota.

The guide credits an [ENCCS article](https://enccs.se/2025/09/news/from-supercomputer-to-cloud)
for the discussions that started it.

---

## 10. Glossary highlights

Source: [Glossary](https://lumi-ai-factory.eu/glossary/). Terms specific to LUMI AIF:

- **Access model:** a way to get LUMI-AI time, such as a call, grant, challenge or pay-per-use.
- **AI Factory:** an entity providing AI supercomputing service infrastructure, introduced by the
  European Commission's AI Innovation Package.
- **AI Factory Hub:** a physical or virtual co-working space.
- **Aitta:** CSC's AI inference service.
- **LUMI-G:** the GPU partition (MI250X).
- **LUMI-K:** the Kubernetes/OpenShift container cloud.
- **LUMI-O:** Ceph object storage.
- **LUMI-IQ:** the upcoming quantum computer.
- **Try&Buy:** limited-scale trial before full adoption.
- **Petascale / pre-exascale / exascale:** 10¹⁵ / 10¹⁷–10¹⁸ / 10¹⁸ operations per second.

The glossary also defines general terms (CV, DaaS, Data Act, FAIR, federated learning,
fine-tuning, foundation model, GDPR, GenAI, RAG, RDI, multitenancy, trustworthy AI, etc.).

---

## 11. Blog posts, news, success stories, trainings and events

Only titles, dates and links were in the snapshot; the full texts are on the linked pages.
Dates are publication dates (YYYY-MM-DD). Full lists:
[news](https://lumi-ai-factory.eu/about-us/news/) ·
[success stories](https://lumi-ai-factory.eu/success-stories/) ·
[trainings](https://lumi-ai-factory.eu/trainings/) ·
[events](https://lumi-ai-factory.eu/events/).

### Blog posts
- [When one computing method is not enough](https://lumi-ai-factory.eu/articles/when-one-computing-method-is-not-enough/) (2026-11-09)
- [Trustworthy AI: Turning compliance into competitive advantage](https://lumi-ai-factory.eu/articles/trustworthy-ai-turning-compliance-into-competitive-advantage/) (2026-07-01)
- [What is LUMI AI Factory's Artificial Intelligence expert consultation?](https://lumi-ai-factory.eu/articles/ai-expert-consultation/) (2026-04-22)
- [AI and environmental sustainability hand in hand](https://lumi-ai-factory.eu/articles/ai-and-environmental-sustainability/) (2026-04-09)
- [Why supercomputing and LUMI?](https://lumi-ai-factory.eu/articles/blog-why-supercomputing-and-lumi/) (2026-03-19)
- [Towards a competitive European AI ecosystem](https://lumi-ai-factory.eu/articles/towards-a-competitive-european-ai-ecosystem/) (2025-12-04)
- [Machine learning on sensitive data](https://lumi-ai-factory.eu/articles/real-4-reg/) (2025-10-24)
- [Benefits of the LUMI AI Software Environment](https://lumi-ai-factory.eu/articles/benefits-of-the-lumi-ai-software-environment/) (date not in snapshot)

### News and press releases
- [Strengthening AI innovation in Northern Finland](https://lumi-ai-factory.eu/articles/strengthening-ai-innovation-in-northern-finland/) (2026-11-05)
- [LUMI is supporting new Czech research at the intersection of HPC, AI and quantum computing](https://lumi-ai-factory.eu/articles/lumi-is-supporting-new-czech-research-at-the-intersection-of-hpc-ai-and-quantum-computing/) (2026-10-30)
- Press release: [LUMI AI Factory advances toward Europe's first superconducting quantum computer with logical qubits](https://lumi-ai-factory.eu/articles/lumi-ai-factory-advances-toward-europes-first-superconducting-quantum-computer-with-logical-qubits/) (2026-09-10)
- Press release: [IQM selected to deliver the LUMI-IQ quantum computer](https://lumi-ai-factory.eu/articles/iqm-selected-to-deliver-the-lumi-iq-quantum-computer/) (2026-07-08)
- [LUMI AI Factory Hub Ostrava is officially open](https://lumi-ai-factory.eu/articles/lumi-ai-factory-hub-ostrava-is-officially-open/) (2026-05-13)
- [Advancing AI-driven health and research innovation](https://lumi-ai-factory.eu/articles/csc-and-terkko-health-hub/) (2026-04-28): CSC and the Terkko health hub
- [Dataset-as-a-Service from the LUMI AI Factory – data close to compute](https://lumi-ai-factory.eu/articles/dataset-as-a-service/) (2026-04-01)
- [LUMI AI Factory Hub opens in the Kumpula Campus in Helsinki](https://lumi-ai-factory.eu/articles/kumpula-campus/) (2026-02-18)
- Press release: [LUMI AI Factory Hub opens in Finland – innovation and AI expertise for all](https://lumi-ai-factory.eu/articles/lumi-ai-factory-hub-opens-in-fi/) (2025-12-02)
- [Research shows LUMI AI Factory drives AI innovation for start-ups and SMEs](https://lumi-ai-factory.eu/articles/market-survey-2025/) (2025-11-14): 2025 market survey
- [EuroHPC JU selects AI Factory Antennas – four Antennas to the LUMI AI Factory](https://lumi-ai-factory.eu/articles/eurohpc-ju-ai-factory-antennas/) (2025-10-13)

### Success stories (customer cases)
| Story | Topic | Date |
|---|---|---|
| [Data streaming pilot paves the way for autonomous vehicles](https://lumi-ai-factory.eu/stories/data-streaming-pilot-smart-car/) | Real-time vehicle data with the University of Oulu. Quote: processing power in the vehicle, connectivity, cloud capacity and storage can all become limiting factors. | 2026-05-26 |
| [Dokport](https://lumi-ai-factory.eu/stories/dokport/) | Online doctor appointments, using expert support (not necessarily HPC) | 2026-03-30 |
| [Data streaming pilot with SeaBee](https://lumi-ai-factory.eu/stories/data-streaming-pilot-with-seabee/) | Seabird monitoring | 2026-03-11 |
| [AI-TRANSPWOOD](https://lumi-ai-factory.eu/stories/ai-transpwood/) | AI modelling for wood materials | 2026-02-20 |
| [TildeOpen](https://lumi-ai-factory.eu/stories/tildeopen/) | Europe's flagship open-source multilingual LLM | 2026-02-09 |
| [QMill](https://lumi-ai-factory.eu/stories/qmill/) | Record-breaking quantum circuit compression on LUMI | 2026-01-27 |
| [SICS AI](https://lumi-ai-factory.eu/stories/sics-ai/) | HPC access for AI and robotics | 2025-12-15 |
| [DigiFarm](https://lumi-ai-factory.eu/stories/digifarm/) | AI in agriculture | 2025-09-19 |
| [Bris](https://lumi-ai-factory.eu/stories/bris/) | High-resolution data-driven weather forecasting | 2025-09-19 |
| [Top Data Science](https://lumi-ai-factory.eu/stories/top-data-science/) | AI innovation on LUMI | 2025-09-19 |
| [Gosta Labs](https://lumi-ai-factory.eu/stories/gosta-labs/) | Efficiency of healthcare client encounters | 2025-09-19 |
| [ICEYE](https://lumi-ai-factory.eu/stories/iceye/) | Space technology; praises step-by-step LUMI user support | 2025-09-19 |
| [Supersight](https://lumi-ai-factory.eu/stories/supersight/) | Real estate | 2025-09-19 |
| [ComPatAI](https://lumi-ai-factory.eu/stories/compatai/) | AI learning model for pathology | 2025-09-19 |

### Trainings (as listed on 2026-11-23)
| Training | Level | When | Where |
|---|---|---|---|
| [LUMI related training opportunities](https://lumi-ai-factory.eu/trainings/lumi-related-training/) | Beginner–intermediate | 2025-11-13 – 2027-12-03 (ongoing) | Online / hybrid / on site |
| [LUMI AI Factory onboarding](https://lumi-ai-factory.eu/trainings/lumi-ai-factory-onboarding/) | Beginner | 2026-10-14 – 2027-10-31 (self-paced) | Online |
| [AI-ready data and FAIR data management for industry](https://lumi-ai-factory.eu/trainings/ai-ready-data-and-fair-data-management-for-industry/) | Beginner | 2026-10-14 – 2027-10-31 | Online |
| [Run AI Agents with LUMI workshop](https://lumi-ai-factory.eu/trainings/run-ai-agents-with-lumi-workshop/) | Intermediate | 2026-11-23 | Espoo, Finland |
| [Moving your AI training jobs to LUMI: a hands-on workshop](https://lumi-ai-factory.eu/trainings/moving-your-ai-training-jobs-to-lumi-a-hands-on-workshop-2/) | Intermediate | 2026-11-25 – 26 | Riga, Latvia / online |

### Events (as listed on 2026-11-23)
| Event | When | Where |
|---|---|---|
| [Vibecoding & AI Engineering Festival](https://lumi-ai-factory.eu/events/vibecoding-ai-engineering-festival/) | 2026-11-26 | Ostrava, Czechia |
| [Europe in the loop](https://lumi-ai-factory.eu/events/europe-in-the-loop/) | 2026-11-30 | Espoo, Finland |
| [Venture Incubation program info sessions](https://lumi-ai-factory.eu/incubation-program/) | 2026-11-30 and 2026-12-14 | Online |
| *Health Tech Meets AI* (Otaniemi hub; mentioned on the [Finland hubs](https://lumi-ai-factory.eu/finland-lumi-ai-factory-hubs/) page) | March 2026 (past) | Espoo, Finland |
| [AI Expert Tour](https://lumi-ai-factory.eu/ai-expert-tour/) | Dates to be announced | Various European cities |

---

## Inconsistencies and stale items in the source pages

- [Playground](https://lumi-ai-factory.eu/playground-access-to-lumi-ai-factory/)'s intro says
  "(5.000 GPUs)", but its feature list says **5,000 GPU hours**. The latter is meant.
- The [Trustworthy AI consultation](https://lumi-ai-factory.eu/expert-consultation-on-trustworthy-ai-development/)
  says "three 1-hour sessions" but lists four steps.
- Free use by large companies: [Pricing and eligibility](https://lumi-ai-factory.eu/pricing-and-eligibility/)
  says free services are *not* available to large companies, while
  [Fast Lane](https://lumi-ai-factory.eu/fast-lane-access-to-lumi-ai-factory/) allows it for open
  science with published results.
- [Try&Buy](https://lumi-ai-factory.eu/trybuy/) lists its target group as "SMEs and startups",
  but its text says "Finnish companies".
- [Aitta](https://lumi-ai-factory.eu/aitta-ml-inference-service/)'s pilot invite period ended
  **September 2026**, before the snapshot date.
- The *AI for Science* cut-off of 30 Oct 2026 had already passed (the next was 11 Dec 2026).
  Large Scale had no resources left for 2026.
- Typos in the source: "EuroHOC" (EuroHPC) on the quantum page. The Ostrava hub email link points
  to `it4i-factory-hub@it4i.cz` while its text says `ai-factory-hub@it4i.cz`.
- The [Hubs](https://lumi-ai-factory.eu/hubs/) page links the Ostrava hub as `/czechia-hub/`,
  while the page itself is at `/czechia-lumi-ai-factory-hub/`.
