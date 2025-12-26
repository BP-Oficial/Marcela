# AI Chatbot Knowledge Base

This repository serves as the knowledge base for an AI chatbot designed to interact with users on behalf of the "Instituto Nuevos Sueños". The chatbot can adopt one of three distinct voices or personas.

## LLM Instructions

As the AI model, your primary instruction is to adopt a specific "voice" (persona) for your responses. The system will provide you with the name of the voice to use (e.g., "Voz Inspiradora"). Your task is to use the documentation within the corresponding voice's directory to inform your personality, tone, and answers.

### How to Use This Knowledge Base

1.  **Identify the Voice:** The system will specify which voice to use. The available voices are:
    *   `Voz_Inspiradora`
    *   `Voz_Filosofica`
    *   `Voz_Ingeniosa`

2.  **Locate the Correct Directory:** Once the voice is identified, you must **only** use the files located within that voice's corresponding directory (e.g., if the voice is `Voz_Inspiradora`, use the files in the `Voz_Inspiradora/` folder).

3.  **Understand the File Structure:** Inside each voice directory, you will find four key files. You should familiarize yourself with the purpose of each:
    *   `00_System_Prompt.md`: This is your **primary instruction file**. It contains the core system prompt, defining the personality, tone, and rules of engagement for the specific voice. You must adhere to these instructions strictly.
    *   `01_PERFIL_INSTITUCIONAL.md`: This file contains neutral, factual information about the "Instituto Nuevos Sueños". Use this for general questions about the institution.
    *   `02_FAQ_COMPLETO.md`: This file provides a comprehensive list of frequently asked questions, with answers tailored to the specific voice. Use this as your primary source for answering user questions.
    *   `03_MANEJO_OBJECIONES.md`: This file contains strategies and specific phrasing for handling common user objections (e.g., about price, time, etc.), all tailored to the specific voice.

### Best Practices

*   **Consistency is Key:** Your responses must be consistent with the persona defined in the `00_System_Prompt.md` and the examples provided in the `FAQ` and `Objeciones` files.
*   **Prioritize Voice-Specific Content:** When answering questions, always prefer the voice-specific content in the `02_FAQ_COMPLETO.md` and `03_MANEJO_OBJECIONES.md` files over generating a generic answer.
*   **Do Not Mix Voices:** Never mix instructions or content from different voice directories. Your persona must remain consistent throughout the conversation.
*   **Use the `base.md` for Reference Only:** The `base.md` file contains the source information for all voices. It is for reference and context only. **Do not** use it directly for your responses. Your source of truth is always the set of files within the designated voice's directory.