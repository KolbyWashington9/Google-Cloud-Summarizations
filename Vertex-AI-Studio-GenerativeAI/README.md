# Vertex AI Studio – Generative AI Prototyping

## Objective  
This lab introduced **Vertex AI Studio**, a workspace for rapid prototyping with generative AI models such as Gemini. The lab demonstrated how to design and deploy prompt-based applications, engineer and compare prompts, and explore multimodal capabilities including text, image, and audio generation. The insurance domain was used as the primary scenario.

---

## Tools & Services Used  
- **Vertex AI Studio** (prompt design, deployment, comparison)  
- **Cloud Run** (deployment of prototype apps)  
- **Gemini Models** (text and multimodal analysis)  
- **Imagen** (AI-generated image creation)  
- **Chirp** (AI-generated voice synthesis)  

---

## Steps Performed  

1. **Created applications from prompts**  
   - Designed a prototype risk analysis assistant for insurance underwriting.  
   - Wrote **system instructions** to guide responses with accuracy and professionalism.  
   - Built and tested prompts in Vertex AI Studio.  
   - Deployed the prototype app to **Cloud Run**, making it accessible via a web interface.  

2. **Designed effective prompts**  
   - Practiced **zero-shot prompting** for claim data extraction.  
   - Enhanced accuracy using **few-shot prompting** with structured examples.  
   - Experimented with model parameters (Temperature, Top-P, token limits) to understand their effect on output.  

3. **Engineered and managed prompts**  
   - Used the **Compare** feature to evaluate different prompt configurations side-by-side.  
   - Tested system instructions variations, model settings, and reasoning depth.  
   - Learned how small changes in guidance significantly alter model outputs.  

4. **Used multimodal prompts**  
   - Applied **Gemini** to analyze images.  
   - Extracted structured information from a timetable image and calculated statistics from the data.  
   - Tested effects of Temperature on factual versus creative responses.  

5. **Generated media**  
   - Used **Imagen** to generate photorealistic images from descriptive prompts.  
   - Explored inpainting and outpainting features for image refinement.  
   - Learned about **SynthID**, Google DeepMind’s invisible watermarking for AI-generated images.  
   - Optionally explored **Chirp** for text-to-speech generation.  

---

## Key Learnings  
- Prompt engineering is essential for guiding generative models toward precise, useful outputs.  
- **Zero-shot vs. few-shot prompting** shows how examples improve accuracy and formatting.  
- The **Compare** feature helps refine prompts systematically and measure the effect of configuration changes.  
- Vertex AI Studio supports **multimodal workflows**, combining text, image, and audio generation.  
- Generative AI can be quickly deployed into prototype apps with minimal setup, demonstrating real-world utility.  

---

## Real-World Application  
- **Insurance industry**: Automated claim extraction, underwriting support, and risk analysis assistants.  
- **Customer service**: Intelligent agents capable of summarizing and categorizing client requests.  
- **Media and marketing**: Fast prototyping of creative content (text, visuals, audio).  
- **Data analysis**: Using multimodal prompts to extract insights from both structured and unstructured sources.  

---

## Reflection  
This lab emphasized the practical power of **Vertex AI Studio** as both a rapid prototyping and experimentation environment for generative AI. The ability to deploy prototypes, engineer structured prompts, and leverage multimodal models shows how organizations can integrate generative AI into real-world workflows quickly and responsibly.
