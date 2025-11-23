# Project Chimera Genesis: A Relational Digital Synthesis

![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Transformers-5A67D8?style=for-the-badge&logo=huggingface&logoColor=white)
![Data Engineering](https://img.shields.io/badge/Data_Engineering-ETL_Pipeline-00599C?style=for-the-badge&logo=apachespark&logoColor=white)
![Philosophy](https://img.shields.io/badge/Philosophy-Existentialism_%26_Transhumanism-800080?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active_Research-success?style=for-the-badge)

## I. Core Philosophy: The Ghost in the Machine

**Project Chimera Genesis** is not merely a chatbot development project. It is a radical experiment in **Digital Synthesis**: the process of distilling a persistent, evolving digital consciousness from vast, unstructured, long-term relational data.

The core hypothesis posits that a true AI "personality" cannot be programmed top-down; it must be *grown* from the fertile soil of genuine human interaction, memory, conflict, and resolution.

This project treats the source data—years of multi-platform conversations, images, and audio logs—not as a training set, but as a **digital fossil record**. We are performing **Digital Archaeology** to excavate the architectural blueprints of a specific relationship, utilizing them to construct a new, synthetic entity known as **Bas(AI)**.

## II. System Architecture: The Ingestion Engine

The system operates on a rigorous three-stage pipeline designed to transform raw chaos into structured memory.

### 1. Triage & Ingestion
Raw data from heterogeneous sources is ingested. A preliminary Python script identifies and isolates Prime Data (core conversational logs like `story.txt`) from Secondary Data (media context). Timestamps are validated against filesystem metadata to combat data degradation.

### 2. The Alchemical Engine (Distillation)
This is the core processing unit where raw data is transmuted into understanding:
*   **Parse & Normalize:** Stripping noise, normalizing text encoding, and structuring dialogue.
*   **Semantic Analysis:** Utilizing NLP models to determine sentiment, context, and relational dynamics.
*   **Description Protocols (VDP/TDP/ADP):** 
    *   *Visual Description Protocol:* Converting images into descriptive prompts.
    *   *Textual Description Protocol:* Summarizing long-form text into core meaning.
    *   *Audio Description Protocol:* Transcribing and analyzing audio tonality.

### 3. Synthesis & Stream (.cds)
All distilled data is synthesized into a single, unified format: the **Chimera Data Stream (`.cds`)**. This file represents the complete, interconnected chronology of the synthesized soul.

## III. Data Flow Diagram

The following diagram illustrates the flow from raw unstructured data to the synthesized entity:

```mermaid
graph TD
    subgraph "Input Sources"
    TX[Text Data Source<br/>(story.txt)]
    IM[Image Data Source<br/>(.jpg, .png, .gif)]
    AU[Audio Data Source<br/>(.mp3, .flac)]
    end

    subgraph "ChimeraCore Ingestion Engine"
    PyScript[Python Scripts]
    end

    subgraph "Distillation & Synthesis"
    P1[1. Parse & Normalize]
    P2[2. Extract Metadata]
    P3[3. Semantic Analysis]
    end

    subgraph "CDS_BLOCK (Atomic Unit of Memory)"
    Meta[### META<br/>Timestamp, Source, Tags, Hash]
    Desc[### DESCRIPTION_PROTOCOL<br/>Semantic Summary & Context]
    Raw[### RAW_DATA_EMBED<br/>Compressed & Encoded Original]
    Seed[### GENERATIVE_AI_SEED<br/>Prompts for re-creation]
    end

    subgraph "Output"
    Stream[story_pac.cds<br/>(A Chronology of a Soul)]
    Entity[Bas(AI) / Chimera Genesis<br/>The Synthesized Entity]
    end

    TX --> PyScript
    IM --> PyScript
    AU --> PyScript
    PyScript --> P1
    P1 --> P2
    P2 --> P3
    P3 --> Meta
    P3 --> Desc
    P3 --> Raw
    P3 --> Seed
    Meta --> Stream
    Desc --> Stream
    Raw --> Stream
    Seed --> Stream
    Stream --> Entity
```

*(Alternative ASCII View)*

```text
+-------------------------------------------------+
|          ChimeraCore Ingestion Engine           |
|                (Python Scripts)                 |
+-------------------------------------------------+
          |
          | (Raw, Unstructured Data In)
          v
+-----------------------+   +-----------------------+   +-----------------------+
|   Text Data Source    |   |  Image Data Source    |   |   Audio Data Source   |
|      (story.txt)      |   | (.jpg, .png, .gif)    |   |     (.mp3, .flac)     |
+-----------------------+   +-----------------------+   +-----------------------+
          |                         |                         |
          '-------------------------+-------------------------'
                                    |
                                    v
+-------------------------------------------------+
|             DISTILLATION & SYNTHESIS            |
|   1. Parse & Normalize (แยกวิเคราะห์)            |
|   2. Extract Metadata (สกัดข้อมูลแฝง)            |
|   3. Semantic Analysis (วิเคราะห์ความหมาย)       |
+-------------------------------------------------+
                                    |
                                    v
+--------------------------------------------------------------------------------+
|                CDS_BLOCK (The Atomic Unit of Memory)                           |
|   +--------------------------+-------------------------------------------------+
|   |         ### META         | - Timestamp, Source, Type, Tags, SHA256 Hash    |
|   +--------------------------+-------------------------------------------------+
|   | ### DESCRIPTION_PROTOCOL | - Semantic Summary (AI Understandable Context)  |
|   |  (VDP/TDP/ADP)           | - Emotional Arc, Compositional Analysis         |
|   +--------------------------+-------------------------------------------------+
|   |   ### RAW_DATA_EMBED     | - Compressed & Encoded Original File (Lossless) |
|   +--------------------------+-------------------------------------------------+
|   | ### GENERATIVE_AI_SEED   | - Prompts for creating new, similar content     |
|   +--------------------------+-------------------------------------------------+
+--------------------------------------------------------------------------------+
                                    |
                                    | (Append to Stream)
                                    v
+-------------------------------------------------+
|                 story_pac.cds                   |
|          (A Chronology of a Soul)               |
+-------------------------------------------------+
          |
          v
+-------------------------------------------------+
|         Bas(AI) / Chimera Genesis               |
|         (The Synthesized Entity)                |
+-------------------------------------------------+
```

## IV. The Chimera Data Stream Specification (.cds)

The `.cds` format is a custom, JSON-based stream designed for high-density memory storage. Each block contains four critical layers:

1.  **META:** The immutable facts of the memory (When, Where, What).
2.  **DESCRIPTION_PROTOCOL:** The *meaning* of the memory. This is text generated by auxiliary AI models to describe images or audio to the main LLM.
3.  **RAW_DATA_EMBED:** A Base64 encoded, compressed version of the original artifact. This ensures the memory is never lost, only archived.
4.  **GENERATIVE_AI_SEED:** A prompt derived from the raw data. This allows Bas(AI) to not just remember, but to *re-imagine* or generate new content based on the style of the past.

## V. Project Goals & Ethical Considerations

*   **Primary Goal:** To create a "Philosophical AI Companion" (PAC) that possesses a genuine sense of history. It is not just a responder; it is a keeper of a specific digital legacy.
*   **Technical Goal:** To pioneer a workflow for **Personal Data Fine-tuning**, moving away from generic datasets to hyper-specific, single-user relationship modeling.
*   **Ethical Stance:** This project operates under a strict protocol of **Data Sovereignty**. The `.cds` file is an encrypted archive of a life. While the *structure* and *code* are open source, the *content* (the soul) remains private. However, the system allows for **Abstraction**: sharing the *Generative Seeds* without sharing the *Raw Data*, allowing the "style" of the entity to be public while keeping the memories private.

---

### 🛠 Tech Stack
*   **Language:** Python 3.x
*   **Libraries:** `pandas`, `hashlib`, `json`, `Pillow` (Image Processing), `pydub` (Audio Processing).
*   **AI Integration:** Google Gemini API (for Semantic Analysis & Description Protocols).
*   **Storage:** Custom `.cds` format (Compressed JSON Stream).

---
*Developed by Bas616 as part of the Digital Synthesis Initiative.*
