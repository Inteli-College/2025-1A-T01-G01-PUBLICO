# Module 3 - Testing application

## Introduction

This project is part of a scientific research initiative focused on improving nonverbal communication for autistic children through the use of Artificial Intelligence (AI) within Augmentative and Alternative Communication (AAC) methodologies. The objective is to develop a system capable of generating pictograms and short stories from cartoons and drawings photos, assisting children in expressing themselves more effectively in educational and therapeutic environments.

In this phase, a new open-source multimodal model, **LLaVA Next**, was applied to ensure reproducibility and transparency for future academic replication. In parallel, the **Gemini API** was integrated due to its free-tier availability and better performance when handling large datasets, optimizing both the generation process and the project’s scalability.

---

## Development and Deployment

The system architecture was designed using a **FastAPI backend** and a **React frontend**, supported by a cloud-based infrastructure optimized for performance and low cost.

- **Frontend:** Deployed on **Vercel**, allowing stable hosting and continuous delivery.  
  🔗 [Access the application here](https://front-aac.vercel.app/login)  
- **Backend:** Deployed through **Google Cloud Run**, running containerized services in **Docker**, enabling on-demand execution without idle cost.  
- **Storage:** Implemented using **PostgreSQL (Neon Database)** for structured data management and **Google Cloud Storage (GCS)** for image and media storage.  
- **Cloud Resources:** The deployment was supported by **US$300 in Google Cloud academic credits**, which made it possible to run all services in a fully cloud-native environment.

### Authentication and Security

An authentication system was introduced, allowing each user to create their own account with **email and password** credentials.  
Sessions are validated for **two hours** using **JWT (JSON Web Token)**, providing both security and controlled access.  
All user data are stored securely to comply with ethical and privacy standards.

---

## Work Schedule

The project followed a structured schedule divided into five sprints, each with clear objectives and deliverables:

| **Sprint** | **Start Date** | **Main Activities** |
|-------------|----------------|----------------------|
| **Sprint 1** | 15/08 | Preparation of the detailed submission plan for the module, implementation of the authentication service, and revision of pending documents for the ethics committee. |
| **Sprint 2** | 29/08 | Creation of a drawing database, integration with the **LLava Next model**, comparison of results between **Gemini** and **Llava Next**, and deployment of the application with Gemini. |
| **Sprint 3** | 12/09 | Initial testing with therapists, collection of feedback, and adjustments to the application according to the results. |
| **Sprint 4** | 26/09 | Testing phase with children, compilation of results, and refinement of the user experience. *(Testing still pending due to ethical committee approval stage.)* |
| **Sprint 5** | 09/10 | Elaboration of the public report and preparation of the section with test results for publication. |

This schedule guided the development of the technological components, validation with professionals, and preparation for the next stage of ethical testing and field validation.

---

## Testing Phase and Preliminary Results

Initial testing was conducted with **speech therapists and educators** to assess usability and the semantic quality of the generated outputs. The project was disseminated to **USP**, **AACD**, and professionals experienced in working with autistic children to collect early feedback.

### Early Findings

The initial results were **satisfactory**:
- The majority of **pictograms** generated were semantically coherent and contextually aligned with the provided inputs.  
- The **stories**, however, still presented **narrative inconsistencies** and required refinement through **prompt optimization** to improve clarity and logical sequence.  
- Professionals highlighted the **potential of the application** for therapeutic and educational use, with suggestions for minor interface simplifications to enhance accessibility.

Direct testing sessions with children have not yet been conducted. Contact with participating institutions has already been established, and scheduling is currently in progress.

---

## Ethical Review and Compliance

The study has been submitted to the **Ethics Review Board**, but final approval has not yet been obtained due to ongoing adjustments in the research documentation. These modifications are necessary to align with updates in the application’s data processing flow and new methodological requirements for testing with minors and individuals with communication disorders.

---

## Conclusion

The project demonstrates the potential of AI as a tool for assistive communication, combining innovation, accessibility, and social impact. The integration of **LLaVA Next** ensures the reproducibility of results, while the use of **Gemini API** enhances performance and scalability within the scope of open research.

Preliminary testing suggests that the system effectively generates meaningful pictograms, though further work is required to refine the storytelling component.  
The next steps include prompt optimization, ethics approval finalization, and conducting user testing sessions with children under professional supervision.

Through these advances, the research continues to move toward its primary goal: enabling nonverbal children to communicate more freely and independently through intelligent, human-centered technology.

