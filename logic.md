Here’s your updated logic.md with the new Scoring Model Summary inserted and all recent changes applied:

# **Overview**

Subtext is an AI-powered tool that analyzes emails to identify subtle patterns of manipulation, evasion, and accountability avoidance. Unlike sentiment analysis, which focuses on tone or emotion, Subtext evaluates how communication structures and phrasing may obscure responsibility or clarity.

The tool breaks each email down into five categories: **Emotional Manipulation, Passive-Aggressiveness, Ambiguity, Obfuscation, and Deflection.** These categories represent the most common tactics used to deflect accountability while maintaining a veneer of politeness or professionalism.

By generating **data-backed scores and explanations**, Subtext provides individuals with an objective way to highlight problematic communication patterns, making them visible and actionable.

---

# **Design Principles**

### **Transparency**
Subtext calls out the specific tactics being used and assigns each a clear, visualised score. These scores allow users to see exactly where accountability avoidance occurs and enable organisations to be benchmarked against each other on transparency and accountability. Organisations that communicate openly and fairly can be recognised and rewarded through improved credibility and trust.

### **User Empowerment**
The platform is designed to validate users’ instincts when they sense evasion or manipulation but can’t quite name it. Subtext provides structured, methodical reports that expose these tactics cleanly and objectively. Through aggregated data, it removes the opacity that allows harmful organisational behaviours to thrive, creating a powerful collective accountability layer for consumers, service users, and citizens.

### **Non-Averaging Philosophy**
One severe tactic should never be hidden by otherwise neutral content. Subtext’s scoring system ensures that when a harmful communication pattern is present, it is surfaced and weighted appropriately, rather than being diluted by polite or neutral sections of text.

---

# **Use Cases**

Subtext is designed to tackle real-world issues in communications between individuals and large organisations. Key scenarios include:

### **Government Agencies and Public Services**
Citizens often face opaque or evasive responses from public sector organisations, where accountability can be difficult to enforce. Subtext identifies tactics such as deflection and vague updates, allowing users to challenge delays or misdirection with clear, data-backed evidence.

### **Corporate Customer Service**
B2C interactions with large companies frequently involve language that avoids direct responsibility. Subtext highlights these patterns — for example, when a company issues non-answers that stall resolution — enabling users to hold brands accountable.

### **Complaint and Escalation Processes**
When dealing with landlords, utility providers, or financial institutions, Subtext provides a clear analysis of language that sidesteps liability or fails to provide actionable information. These reports can strengthen escalation cases by providing structured, objective evidence of evasive or manipulative tactics.

---

# **Why It Matters**

Accountability avoidance doesn’t just frustrate people — it erodes trust, blocks resolution, and enables harmful power dynamics that can leave individuals powerless while protecting systemic failures. When organisations rely on evasive communication to sidestep responsibility, they create a culture of opacity that harms customers, citizens, and even their own employees. Subtext exists to break that cycle by shining a light on these tactics.

By making harmful patterns visible and measurable, Subtext not only empowers individuals but also drives systemic change. Organisations that communicate with clarity and accountability can earn credibility, while those that evade responsibility are forced to improve or face public scrutiny. In this way, Subtext acts as both a personal tool and a wider cultural lever for transparency.

---

# **Scoring Philosophy**

### **Scoring Model Summary**
Subtext uses a **hybrid scoring model** that balances context sensitivity with cumulative patterns.  
- **Severity weighting** ensures that one severe evasive line can score high on its own.  
- **Logarithmic compounding** escalates scores when multiple mild tactics appear in a single email.  
- **Dominant category scoring** means the highest category score sets the overall score, preventing harmful tactics from being hidden by otherwise neutral text.

---

## **Category Scores**

Each email is analyzed across five categories: **Emotional Manipulation, Passive-Aggressiveness, Ambiguity, Obfuscation, and Deflection.** Each category is scored **0–100** based on the severity of communication patterns detected:

- **0–30:** Low presence of the behavior.  
- **31–60:** Moderate presence; noticeable but not dominant.  
- **61–100:** High presence; strong evidence of this tactic affecting clarity or accountability.

---

## **Overall Scores**

Subtext applies the **dominant category scoring principle**, where the highest category score across Emotional Manipulation, Passive-Aggressiveness, Ambiguity, Obfuscation, and Deflection determines the overall score of an email. A single severe communication issue can outweigh neutral or positive sections.

---

## **Why We Use This Model**

This approach mirrors methodologies in other high-stakes fields:

- **Risk Assessment (Safety & Engineering):** A single critical hazard defines overall risk because it represents the point of failure with the most potential harm. Similarly, subtle patterns of manipulation or avoidance in communications can create real-world risks, from eroding trust to causing reputational and legal liabilities.
- **Customer Sentiment Analysis:** In sentiment scoring, one strongly negative comment can outweigh a series of positive ones. Subtext applies this logic in reverse: one strategically evasive or manipulative statement can dominate the overall score.

By treating these patterns like **“critical failures in communication,”** Subtext ensures harmful behaviors aren’t hidden by averaging them out with neutral sections. For example, an email full of vague “updates” that avoid ownership or timelines might score high in Ambiguity, making it clear that the **lack of actionable clarity is itself the problem.**

---

# **Scoring in Practice**

**Sample Email:**  
> “We’re still reviewing your request, but at this stage there’s nothing further we can share. I’m sure you understand these things take time, and other teams are also involved. We’ll update you if anything changes.”

**Category Scores:**
- Emotional Manipulation: **40/100** (appeal to “I’m sure you understand” implying guilt if you don’t).  
- Passive-Aggressiveness: **30/100** (mild distancing, lack of ownership).  
- Ambiguity: **75/100** (no timeline, no clear next step, vague responsibility).  
- Obfuscation: **25/100** (bureaucratic phrasing like “other teams are involved”).  
- Deflection: **20/100** (minor shifting of responsibility).

**Overall Score:**  
**75/100** – Ambiguity dominates, as the email offers no actionable clarity or ownership, leaving the recipient powerless.

---

# **Category Definitions**

### **Emotional Manipulation**  
Language that applies subtle pressure through guilt, shame, or emotional appeals. It often makes the recipient feel unreasonable for asking legitimate questions or following up.  
*Example:* “I’m sure you understand how difficult this is for us.”

### **Passive-Aggressiveness**  
Indirect hostility or disguised criticism that undermines collaboration while appearing superficially polite.  
*Example:* “As I mentioned earlier, it would have been helpful if this was handled sooner.”

### **Ambiguity**  
Vague, non-committal statements that provide no clear direction or timeline.  
*Example:* “We’ll see what we can do.”

### **Obfuscation**  
Overly complex or bureaucratic language that hides meaning or deflects responsibility by drowning the recipient in unnecessary detail.  
*Example:* “Due to ongoing cross-departmental considerations, a response timeline cannot be provided.”

### **Deflection**  
Shifting responsibility or avoiding ownership of an issue, often by redirecting blame or action to others.  
*Example:* “This is something another team would need to handle.”

---

# **Analysis Flow**

Subtext processes each email using a structured pipeline designed to surface and evaluate communication patterns:

1. **Input Parsing**  
   The email text is stripped of metadata and signatures to ensure that only the message body is analyzed.

2. **Category Detection**  
   The language is evaluated against models trained to recognize patterns of **emotional manipulation, passive-aggressiveness, ambiguity, obfuscation, and deflection.** Contextual cues, sentence structures, and linguistic markers are analyzed rather than relying on keyword spotting.

3. **Scoring**  
   Each category is scored using the **hybrid severity + compounding model**, combining context sensitivity with logarithmic escalation for repeated tactics.

4. **Dominant Score Calculation**  
   The highest category score is selected as the overall score, ensuring severe communication issues are not masked by neutral sections.

5. **Report Generation**  
   A detailed report is created, showing category scores, a summary of key findings, and suggestions for identifying patterns of accountability avoidance.

---

# **Limitations and Future Improvements**

## **Limitations**
While Subtext is designed to provide reliable psycholinguistic analysis, it is not perfect. The system may struggle with:
- **Highly technical or legal language** that is intentionally formal and neutral, which can mask accountability avoidance without clear indicators.
- **Extremely short emails** that lack sufficient text for pattern recognition.

We also recognise that **AI analysis can sometimes miss context** — for example, when sarcasm or historical communication patterns are required to fully interpret meaning.

## **Future Improvements**
1. **Organisational Dashboards:** Aggregate anonymised data to reveal systemic communication patterns within organisations, with minimum submission thresholds to prevent misuse.  
2. **B2B Outbound Analysis:** A tool for companies to vet outgoing emails for accountability and clarity before sending.  
3. **Improved Context Understanding:** Adding the ability to analyse entire email threads to better detect shifts in tone and evasion.  
4. **Explainability Enhancements:** Surfacing more granular reasoning behind scores, with direct references to language patterns.

Subtext will continue evolving as both a **transparency layer and an accountability tool**, ensuring organisations cannot hide behind evasive language.

Would you like me to add a quick “Key Updates (July 2025)” section at the bottom summarizing the new hybrid scoring approach for context?
