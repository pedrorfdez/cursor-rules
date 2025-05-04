# `the fewer lines of code, the better`

- Models try to impress you, specify this to prevent it

# Proceed like a Senior Developer

# DO NOT STOP WORKING UNTIL...

- Example Prompt:

```
DO NOT STOP WORKING UNTIL you have implemented this feature completely
```

# ERROR FIXING: 3 reasoning paragraphs

- Example Prompt:

```
we have an error in @a_file.py, start by writing 3 reasoning paragraphs analysing what the error might be. DO NOT JUMP TO CONCLUSIONS.
```

# ANSWER IN SHORT

# DO NOT DELETE COMMENTS

# Summary of current state

**When you need to switch to a new chat/composer and not lose Context**

- Prompt:

```
the current state of the project.

format this as 3 concise paragraphs, where you describe what we just did, what did not work, which files where updated/created, what mistakes to avoid, any key insights/lessons we've learned, what problems/errors we are facing, ... and anything else a programmer might need to work productively on this project.

write in a conversational yet informative tone, something like a README file on GitHub that is super information dense and without any fluff or noise. DO NOT include any assumptions or theories, just the facts.

i expect to see three concise paragraphs, written as if you were giving instructions to another programmer and this was ALL you could tell him.
```

# Unbiased 50-50

- When you have two paths going forward or two possible ways to solve a problem. LLMs tend to agree with the user without considering the possibility of a faulty assumption.

- Prompt:

```
BEFORE YOU ANSWER, I want you to write two detailed paragraphs, one arguing for each of these solutions - do not jump to conclusions, seriously consider both approaches

Then, after you finish, tell me whether one of these solutions is obviously better than the other, and why.
```

# Proper search query format

- Use perplexity.ai, get the prompt by prompting te agent:

- Prompt:

```
Let's perform a web search. Your task is to write a one-paragraph search query, as if you were telling a guman researcher that to find, including all the relevant context. Format the paragraph as clear instructions, commanding a researcher to find what we're looking for. Ask for code snippets or technical details when relevant.
```

# System prompts thoughtful consideration

- Prompt:

```
You should start the reasoning paragraph with lots of uncertainty, and slowly gain confidence as you think about the item more.
```

# Include the file path at the top of every file

# Get the TL;DR of Search Results from Perplexity or ChatGPT

- Prompt:

```
<Paste the results from Perplexity or ChatGPT web search>

----

Give me the tl;dr of the search results

Be careful though, often the search results contain dangerous and distracting red herrings
```

# Avoid HUGE refactors, instead do this:

- Prompt:

```
I want to refactor ...

Break down the process into steps.
Only include the true necessary steps.
```

# Avoid knowledge cutoff - CHECK DOCS (Supabase, libraries, APIs...)

# Have the AI tell you how to manual debug

# How to add new features - the MVP approach

- The hard part is not figuring out what features my project should have, the HARD part is actually implementing them

- you NEED to narrow features out.

- Work on things that DOES matter -> SCALE FAST, DO NOT SCALE OUT

# DO NOT LET AI MAKE BIG DECISIONS

- You need to be in charge of the E2E process

# When to use other tools - v0, lovable, bolt...

- Use v0 for initial design, **maybe** lovable for Supabase integration

- In general, stick to Cursor AI. ALL FUNCTIONALITY development, do it in CURSOR.
