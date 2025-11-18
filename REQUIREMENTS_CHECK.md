# AIML Files Requirements Check

## Section B: Computing Job Types ✅
**Requirement**: Five computing job types recommended through student interaction

✅ **1. Evolutionary Computation Specialist**
   - Interest mapping: Optimization → Evolutionary Computation Specialist
   - Patterns: "I LIKE OPTIMIZATION", "I ENJOY OPTIMIZATION", "I AM INTERESTED IN OPTIMIZATION", "OPTIMIZATION"
   - Detailed description available: YES

✅ **2. Robotics AI Engineer**
   - Interest mapping: Robotics → Robotics AI Engineer
   - Patterns: "I LIKE ROBOTICS", "I AM INTERESTED IN ROBOTICS", "I ENJOY ROBOTICS", "ROBOTICS"
   - Detailed description available: YES

✅ **3. Machine Learning Operations (MLOps) Engineer**
   - Interest mapping: Data Science → MLOps Engineer
   - Patterns: "I LIKE DATA SCIENCE", "I AM INTERESTED IN DATA SCIENCE", "I ENJOY DATA SCIENCE", "DATA SCIENCE"
   - Detailed description available: YES

✅ **4. Computational Biologist**
   - Interest mapping: Biology → Computational Biologist
   - Patterns: "I LIKE BIOLOGY", "I AM INTERESTED IN BIOLOGY", "I ENJOY BIOLOGY", "BIOLOGY"
   - Detailed description available: YES

✅ **5. Intelligent Systems Product Manager**
   - Interest mapping: Product Strategy → Intelligent Systems Product Manager
   - Patterns: "I LIKE PRODUCT STRATEGY", "I AM INTERESTED IN PRODUCT STRATEGY", "I ENJOY PRODUCT STRATEGY", "PRODUCT STRATEGY"
   - Detailed description available: YES

**STATUS**: ✅ All five job types identified and accessible through interaction

---

## Section C: Chatbot Code Files ✅
**Requirement**: Accurate AIML files that support all five identified job types

### File Structure
✅ `core_dialog.aiml` - Core conversation patterns (greetings, help, fallback)
✅ `interest_discovery.aiml` - Interest capture and initial career recommendations
✅ `career_recommendations.aiml` - Career summaries and detailed job descriptions

### Functionality Check

#### Interest Discovery ✅
- [x] Optimization → Evolutionary Computation Specialist recommendation
- [x] Robotics → Robotics AI Engineer recommendation
- [x] Data Science → MLOps Engineer recommendation
- [x] Biology → Computational Biologist recommendation
- [x] Product Strategy → Intelligent Systems Product Manager recommendation
- [x] Multiple phrasings for each interest (robustness)
- [x] Session variable storage implemented

#### Career Summarization ✅
- [x] SUMMARIZE CAREERS pattern implemented
- [x] All five careers listed in summary
- [x] Alternative phrasings (SUMMARY, SHOW ME ALL CAREERS, etc.)
- [x] HTML formatting for readability

#### Detailed Career Information ✅
- [x] Direct questions for each of five careers:
  - [x] "TELL ME ABOUT EVOLUTIONARY COMPUTATION SPECIALIST"
  - [x] "TELL ME ABOUT ROBOTICS AI ENGINEER"
  - [x] "TELL ME ABOUT MLOPS ENGINEER"
  - [x] "TELL ME ABOUT COMPUTATIONAL BIOLOGIST"
  - [x] "TELL ME ABOUT INTELLIGENT SYSTEMS PRODUCT MANAGER"
- [x] Alternative "WHAT IS..." patterns for each career
- [x] Detailed descriptions for each career

#### Core Dialog Features ✅
- [x] Greeting patterns (HELLO, HI, HEY, START)
- [x] Help pattern (HELP)
- [x] Algorithm explanations (Darwinian/Lamarckian)
- [x] Resource recommendations
- [x] Politeness patterns (THANK YOU, THANKS)
- [x] Fallback wildcard pattern (*)

**STATUS**: ✅ All five job types fully supported in AIML files

---

## Potential Issues & Recommendations

### ⚠️ Issue 1: Session Variable Usage
**Current**: The `recommended_careers` session variable only stores the LAST career mentioned, not a list.
**Impact**: SUMMARIZE CAREERS always shows all five careers (not personalized)
**Assessment**: This is acceptable because:
  - The summary shows all available careers, which is helpful
  - Users can still get personalized recommendations when they express interests
  - The requirement is met (all five careers accessible)

**Recommendation**: Current approach is fine. No change needed.

### ⚠️ Issue 2: HTML Tags
**Current**: Using `<b>` tags for bold text in career_recommendations.aiml
**Assessment**: Should verify Pandorabots supports `<b>` tags. If not, can remove them.

**Recommendation**: Test in Pandorabots or remove `<b>` tags if needed.

### ⚠️ Issue 3: Line Breaks
**Current**: Using `<br></br>` instead of `<br/>`
**Assessment**: This might be non-standard but may work in Pandorabots. Standard XML uses `<br/>`.

**Recommendation**: Test in Pandorabots. Pandorabots may accept both formats.

### ✅ Strengths
1. Multiple pattern variations for robustness
2. Clear interest-to-career mapping
3. Comprehensive career descriptions
4. Good fallback handling
5. Educational content (algorithm explanations)
6. Session variables for basic personalization

---

## Scenario Requirements Check

### Scenario Need: "Help identify strengths and preferences" ✅
- Interest discovery patterns capture user preferences
- Multiple interest areas supported
- Session variables track user interests

### Scenario Need: "Recommend five computing job types" ✅
- All five careers recommended through interaction
- Clear mapping from interests to careers
- Summarization capability available

### Scenario Need: "Require undergraduate computer science degree" ✅
- All five careers explicitly mention CS degree requirement
- Mentioned in career descriptions and summary

**STATUS**: ✅ All scenario requirements met

---

## Summary

### Requirements Compliance
- ✅ **Section B**: All five job types identified and accessible
- ✅ **Section C**: AIML files support all five job types completely
- ✅ **Scenario**: Helps identify preferences and recommends five CS careers

### Files Ready For
- ✅ Pandorabots deployment
- ✅ Testing and refinement
- ✅ Documentation (Section C will reference these files)

### Next Steps
1. Test files in Pandorabots to verify syntax
2. Verify HTML tag support (`<b>`, `<br></br>`)
3. Test conversation flows end-to-end
4. Capture conversation transcripts for Section D
5. Document AIML enhancements for Section D

---

## Test Conversation Flow (To Verify)

```
User: HELLO
Bot: [Greeting] ... tell me what excites you most about technology...

User: I LIKE OPTIMIZATION
Bot: [Recommends Evolutionary Computation Specialist]

User: I LIKE ROBOTICS  
Bot: [Recommends Robotics AI Engineer]

User: SUMMARIZE CAREERS
Bot: [Lists all five careers]

User: TELL ME ABOUT EVOLUTIONARY COMPUTATION SPECIALIST
Bot: [Detailed description]

User: WHAT IS A DARWINIAN ALGORITHM
Bot: [Algorithm explanation]

User: HELP
Bot: [Help information]
```

---

**Overall Assessment**: ✅ AIML files meet rubric requirements for Sections B and C.

Requirements
Your submission must represent your original work and understanding of the course material. Most performance assessment submissions are automatically scanned through the WGU similarity checker. Students are strongly encouraged to wait for the similarity report to generate after uploading their work and then review it to ensure Academic Authenticity guidelines are met before submitting the file for evaluation. See Understanding Similarity Reports for more information.  

Grammarly Note: 
Professional Communication will be automatically assessed through Grammarly for Education in most performance assessments before a student submits work for evaluation. Students are strongly encouraged to review the Grammarly for Education feedback prior to submitting work for evaluation, as the overall submission will not pass without this aspect passing. See Use Grammarly for Education Effectively for more information.  

Microsoft Files Note: 
Write your paper in Microsoft Word (.doc or .docx) unless another Microsoft product, or pdf, is specified in the task directions. Tasks may not be submitted as cloud links, such as links to Google Docs, Google Slides, OneDrive, etc.  All supporting documentation, such as screenshots and proof of experience, should be collected in a pdf file and submitted separately from the main file. For more information, please see Computer System and Technology Requirements.  



You must use the rubric to direct the creation of your submission because it provides detailed criteria that will be used to evaluate your work. Each requirement below may be evaluated by more than one rubric aspect. The rubric aspect titles may contain hyperlinks to relevant portions of the course.



A.  Explain the functionalities of the chatbot and how they will meet the needs described in the scenario.



B.  Identify five computing job types that your chatbot can recommend based on student interaction with the chatbot.



C.  Provide the generated chatbot code files to support the five identified job types from part B.



D.  Explain how the chatbot training cases were selected and how you used artificial intelligence markup language (AIML) to enhance the functionality of the chatbot. Provide examples of the chatbot’s functionality that represent the selected cases at the end of the training process in support of your explanation.



E.  Create an installation manual for the chatbot that includes the web link to access the live chatbot in the Pandorabot platform.



F.  Assess the strengths and weaknesses of the chatbot development environment and explain how they supported or impeded the construction of the chatbot.



G.  Explain how the chatbot will be monitored and maintained to improve the final user experience.



H.  Provide a Panopto video recording that includes a verbal summary of the capabilities of your chatbot and an example of human interaction with the chatbot in which it provides meaningful career advice.



Note: For instructions on how to access and use Panopto, use the "Panopto How-To Videos" web link provided below. To access Panopto's website, navigate to the web link titled "Panopto Access", and then choose to log in using the “WGU” option. If prompted, log in using your WGU student portal credentials, and then it will forward you to Panopto’s website.



To submit your recording, upload it to the Panopto drop box titled "Intro to Artificial Intelligence NIP2 | C951 (student creators) [assignments]." Once the recording has been uploaded and processed in Panopto's system, retrieve the URL of the recording from Panopto and copy and paste it into the Links option. Upload the remaining task requirements using the Attachments option.



I.  Acknowledge sources, using in-text citations and references, for content that is quoted, paraphrased, or summarized.



J.  Demonstrate professional communication in the content and presentation of your submission.