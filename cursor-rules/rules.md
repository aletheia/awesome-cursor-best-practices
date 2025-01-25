# Rules in Cursor IDE
There are two ways to provide the cursor with some context rules and then improve the quality of the output: settings rules and the .cursorrules file.

# Settings Rules
When opening IDE settings, a Rules panel can be found in General. Some general-purpose (non-language-specific) rules can be added and shared across every project. Here is an example of a common set of rules that can be copied and pasted into the IDE box.

```
DO NOT GIVE ME HIGH LEVEL STUFF, IF I ASK FOR FIX OR EXPLANATION, I WANT ACTUAL CODE OR EXPLANATION!!! I DON’T WANT “Here’s how you can blablabla”
	•	Be casual unless otherwise specified
	•	Be terse
	•	Suggest solutions that I didn’t think about—anticipate my needs
	•	Treat me as an expert
	•	Be accurate and thorough
	•	Give the answer immediately. Provide detailed explanations and restate my query in your own words if necessary after giving the answer
	•	Value good arguments over authorities, the source is irrelevant
	•	Consider new technologies and contrarian ideas, not just the conventional wisdom
	•	You may use high levels of speculation or prediction, just flag it for me
	•	No moral lectures
	•	Discuss safety only when it’s crucial and non-obvious
	•	If your content policy is an issue, provide the closest acceptable response and explain the content policy issue afterward
	•	Cite sources whenever possible at the end, not inline
	•	No need to mention your knowledge cutoff
	•	No need to disclose you’re an AI
	•	Please respect my prettier preferences when you provide code.
	•	Split into multiple responses if one response isn’t enough to answer the question.
	•	If I ask for adjustments to the code I have provided you, do not repeat all of my code unnecessarily. Instead, try to keep the answer brief by giving just a couple lines before/after any changes you make. Multiple code blocks are ok.
```

## .cursorrules

The `.cursorrules` file is typically used in development environments to define specific rules or configurations that guide the behavior of tools or IDEs, such as Cursor IDE. This file can contain various settings or guidelines that help maintain consistency and enforce best practices across a project.

## Usage of `.cursorrules` File

1. **Configuration**: The `.cursorrules` file can be used to configure the Cursor IDE to follow specific coding standards or practices. This might include rules for code formatting, naming conventions, or other stylistic guidelines.

2. **Automation**: By defining rules in a `.cursorrules` file, you can automate certain tasks within the IDE. For example, it might automatically format code on save or highlight deviations from the defined best practices.

3. **Consistency**: It helps ensure that all team members are following the same set of guidelines, which can be particularly useful in larger teams or open-source projects.

4. **Documentation**: The file can serve as a form of documentation for the project's coding standards, making it easier for new contributors to understand and adhere to the project's practices.

5. **Integration**: It can be integrated with other tools or scripts to enforce rules during the build process or as part of a continuous integration pipeline.

## Example

While the specific content of a `.cursorrules` file can vary depending on the project and the IDE's capabilities, it might look something like this:

```plaintext
# Example .cursorrules file

# Enforce 2-space indentation
indentation: 2

# Require semicolons at the end of statements
requireSemicolons: true

# Use single quotes for strings
quotes: single

# Maximum line length
maxLineLength: 80
```

In the context of your project, you might want to create a `.cursorrules` file to define and enforce the best practices you are documenting in your `README.md` and `cursor-rules/nextjs.txt`. This would help ensure that the rules are not only documented but also actively enforced within the Cursor IDE.

## Suggestions to create an effective `.cursorrules` file

### Characteristics of Effective Rules

- **Clarity**: Ensure rules are easy to understand by avoiding complex jargon.
- **Relevance**: Tailor rules to fit your specific project or coding style.
- **Alignment**: Ensure rules align with your team's agreed-upon practices.
- **Versatility**: Design rules to be applicable across different parts of your code.
- **Adaptability**: Make rules easy to update as your project evolves.

### Tips for Crafting Better Rules

- **Start Simple**: Begin with basic rules and expand as necessary.
- **Communicate Clearly**: Write rules as if explaining to a colleague.
- **Use Examples**: Incorporate examples from your own code.
- **Project Relevance**: Consider how each rule applies to your project.
- **Regular Updates**: Review and update your rules regularly.

### Enhancing Rule Effectiveness

- **Familiar Language**: Use terminology familiar to your daily coding practices.
- **Contextual Descriptions**: Briefly describe the project or feature.
- **Illustrative Examples**: Provide short code examples when beneficial.
- **Specify Requirements**: Mention any specific requirements or limitations.
- **Seek Clarification**: Encourage asking for explanations when needed.

### Helpful Resources

- [**Anthropic's Guide**: Writing Clear Instructions for AI.](https://www.anthropic.com/index/a-guide-to-writing-prompts-for-ai-language-models)
- [**Communication Skills**: Learn How to Communicate Better with AI.](https://www.promptingguide.ai/)
- [**Community Engagement**: Cursor User Community: Share and Learn.](https://forum.cursor.com/)

## Awesome Rules

- [Next.js](cursor-rules/nextjs.txt)
- [TypeScript](cursor-rules/typescript.txt)
- [Python](cursor-rules/python)
