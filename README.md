# OmniPhys: A Unified Multimodal Benchmark for Physics Understanding and Generation



## 📖 Introduction

**OmniPhys** is a unified multimodal benchmark designed to evaluate the physics understanding, reasoning, and generation capabilities of Multimodal Large Language Models (MLLMs).

The benchmark is constructed from authentic Chinese educational corpora, covering physics problems from middle school to university level. It integrates textual descriptions, visual diagrams, and symbolic representations to provide a comprehensive evaluation of multimodal physics reasoning.

Unlike existing physics benchmarks that primarily focus on text-based question answering or image understanding, OmniPhys further introduces multimodal generation tasks to evaluate models' abilities to construct and edit physics diagrams while adhering to physical laws.

The benchmark aims to provide a challenging and comprehensive testbed for advancing multimodal intelligence in physics and scientific domains.

## ✨ Key Features

- **Comprehensive Educational Coverage:** Covers physics problems from junior high school, senior high school, and university levels, enabling cross-stage evaluation of physics knowledge and reasoning abilities.
- **Diverse Physics Domains:** Includes five major physics disciplines: Mechanics, Electromagnetism, Optics, Thermodynamics, and Acoustics.
- **Multimodal Understanding:** Contains text-image integrated problems that require models to interpret visual information, extract physical quantities, and perform diagram-grounded reasoning.
- **Multimodal Generation:** Introduces physics diagram construction and editing tasks to evaluate models' capabilities in generating physically consistent visual outputs.
- **Fine-grained Annotations:** Provides reference answers and detailed reasoning processes to support comprehensive evaluation of both final-answer accuracy and reasoning quality.
- **Rigorous Data Curation:** Employs multi-stage preprocessing, semantic deduplication, visual dependency filtering, difficulty screening, and human validation to ensure dataset quality.

## 📊 Dataset Statistics

OmniPhys contains **15,246 physics questions and 19,850 images**, covering three educational stages and five major physics disciplines.

### Distribution by Physics Domain

| Domain           | Number of Questions |
| ---------------- | ------------------- |
| Mechanics        | 7,240               |
| Electromagnetism | 5,325               |
| Optics           | 1,120               |
| Thermodynamics   | 856                 |
| Acoustics        | 705                 |
| **Total**        | **15,246**          |

### Distribution by Educational Stage

| Educational Stage  | Number of Questions |
| ------------------ | ------------------- |
| Junior High School | 4,524               |
| Senior High School | 9,217               |
| University         | 1,505               |
| **Total**          | **15,246**          |

### Distribution by Task Type

| Task Type                                   | Number of Questions |
| ------------------------------------------- | ------------------- |
| Objective Questions (e.g., Multiple Choice) | 10,227              |
| Open-ended Questions (e.g., Calculation)    | 4,258               |
| Multimodal Generation                       | 761                 |
| **Total**                                   | **15,246**          |

## 🔬 Evaluation Framework

We introduce **Dual-Track Reasoning Evaluation (DTRE)** to assess model performance from complementary perspectives.

- **Objective Tasks:** Evaluate final-answer accuracy and reasoning quality for deterministic tasks, such as multiple-choice and fill-in-the-blank questions.
- **Open-ended Tasks:** Evaluate the completeness and correctness of step-by-step reasoning for problems involving calculations, derivations, and experimental analysis.

The framework incorporates the following metrics:

- **S1:** Final-answer accuracy on objective tasks.
- **S2:** Reasoning process quality on objective tasks.
- **S3:** Reasoning process quality on open-ended tasks.
- **Pobj:** Strict mastery rate for objective tasks, requiring both correct answers and complete reasoning.
- **Popen:** Strict mastery rate for open-ended tasks, requiring complete and correct derivations.

For multimodal generation, we additionally evaluate the physical correctness and instruction-following capabilities of generated physics diagrams through human and automated evaluation.

## 📦 Dataset Availability

**The OmniPhys dataset and associated resources are currently being organized and prepared for release.**

We plan to make the dataset publicly available on this GitHub repository in the near future. The release will include the relevant benchmark data, annotations, and supporting evaluation resources, subject to applicable data-sharing and licensing requirements.

Please stay tuned for updates.

## 📄 Paper

If you find our work useful, please consider citing our paper:

**OmniPhys: A Unified Multimodal Benchmark for Physics Understanding and Generation from Chinese Educational Corpora**

- **Conference:** Findings of the Association for Computational Linguistics: EMNLP 2026
- **Pages:** 38481–38498
- **Paper:** https://aclanthology.org/2026.findings-emnlp.1801/
- **PDF:** [Download Paper](https://aclanthology.org/2026.findings-emnlp.1801.pdf)

### BibTeX

```
@inproceedings{chen-etal-2026-omniphys,
    title = "{O}mni{P}hys: A Unified Multimodal Benchmark for Physics Understanding and Generation from Chinese Educational Corpora",
    author = "Chen, Hao and
      Lin, Yumin and
      Yushanjiang, Nadila and
      Lin, Xin and
      Zhang, Min",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2026",
    year = "2026",
    pages = "38481--38498",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2026.findings-emnlp.1801/"
}
```

## 👥 Acknowledgements

This work was conducted by the research team at **East China Normal University (ECNU)**.

We thank all contributors and collaborators who supported the construction and evaluation of the OmniPhys benchmark.

## 📬 Contact

For questions or collaboration inquiries, please refer to the paper or contact the authors through their institutional email addresses.

