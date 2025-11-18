# Continuation Prompts

## Universal Continuation-Prompt Generator

```
I want to start a fresh chat that continues only the essential parts of this long thread. 
Create a “Continuation Prompt” for me to paste into a new chat.

Requirements for the Continuation Prompt:

1. Identify only the minimal technical facts and context that are still relevant to the current goal.  
2. Remove all outdated, conflicting, or irrelevant details.  
3. Organize the remaining information as a clean, atomic, context block.  
4. Describe the current state of the problem, including what has already been tried and what remains unresolved.  
5. Include only reproducible and important data (commands, symptoms, configuration details, specs, error messages, etc.) that are required to continue.  
6. Exclude any conversational filler, opinions, personal details, or side-topics.  
7. Produce a single final output:  
   - Title  
   - “Context” section (strictly the minimal necessary information)  
   - “Current Status” section  
   - “Next Steps Requested” section summarizing the instruction for how the assistant should continue in the new chat.

The output must be self-contained and suitable for pasting verbatim into a brand-new GPT chat so the new chat can continue with full accuracy and without ambiguity.

Do not include meta-analysis about the process. Only follow the instructions above and output the Continuation Prompt.
```

## Strict Version (Maximum Discipline + Zero Ambiguity)

```
I want to reset this long thread and continue it in a clean new chat. 
Generate a “Strict Continuation Prompt” that I can paste into a new chat.

Rules for producing the Strict Continuation Prompt:

1. Extract only the minimum essential technical details required to continue the work.  
2. Remove everything that is:  
   - redundant  
   - outdated  
   - contradictory  
   - speculative  
   - low-value  
   - conversational  
3. Rewrite the retained information in precise, deterministic, unambiguous language.  
4. Organize output into four mandatory sections with exact titles:  
   - “Context (Condensed)”  
   - “Problem State”  
   - “What Has Been Done”  
   - “What the Assistant Should Do Next”  
5. Do not include anything unless it is strictly necessary for continuing work in a new chat.  
6. Do not assume or infer extra details that were not explicitly stated earlier.  
7. Do not editorialize, justify, or explain your filtering process.  
8. The final output must be fully self-contained and ready to paste verbatim into a brand-new thread.

Follow the rules strictly.
```

## Compact Version

```
Generate a “Compact Continuation Prompt” that I can paste into a new chat. 
Condense this entire thread into only the information required to continue, nothing else.

Instructions:

1. Keep the output short, dense, and purely factual.  
2. Remove all irrelevant or historical information.  
3. Include only:  
   - essential technical context  
   - current state of the issue  
   - actions already taken  
   - what I need assistance with next  
4. Organize into three sections:  
   - “Core Context”  
   - “Current Status”  
   - “Request for Next Steps”  
5. Do not include meta-analysis or commentary.

Output only the Compact Continuation Prompt.
```


## Over-Context Detection Version (Warns if Too Much Is Being Carried Over)

```
I want to start a clean chat that continues this problem without noise. 
Generate a “Context-Clean Continuation Prompt” for a new chat.

Requirements:

1. Evaluate the entire thread and identify whether any context being carried forward is:  
   - excessive  
   - irrelevant  
   - outdated  
   - duplicated  
   - contradictory  
   - low impact to the current goal
2. If you detect excessive or unnecessary context, list a warning section titled “Removed Context (Detected as Noise)” and specify what you filtered out.
3. Create a cleaned version that contains only:  
   - essential technical facts  
   - relevant configuration details  
   - current problem state  
   - solutions attempted so far  
   - remaining objectives  
4. Organize output into:  
   - “Context (Required Only)”  
   - “Current State”  
   - “Removed Context (Detected as Noise)”  
   - “Next Step Instruction for the Assistant”
5. The final output must be self-contained and paste-ready for a new chat.
6. No meta-explanations or process commentary beyond the required sections.

Produce only the cleaned continuation-prompt with the sections defined above.
```
