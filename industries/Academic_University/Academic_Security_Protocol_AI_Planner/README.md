# Academic Security Protocol AI Planner

Academic Security Protocol AI Planner is an advanced app designed for campus security officers. By inputting specific variables, the AI technology creates custom-tailored security content for educational institutions. The app focuses on providing detailed safety procedures specific to academic environments, including procedural importance, step-by-step actions, potential risks, emergency response methods, and review protocols. This ensures ongoing relevance and effectiveness, making it a comprehensive safety guide for educational security personnel.

To run this app online: [Academic Security Protocol AI Planner Online](https://hero.page/app/academic-security-protocol-ai-planner-ai-powered-campus-security-planning/gNx7mdgJ7p4QliiNQGGn)

To learn more about AI Apps for Campus Security Officer use-cases in the Academic & University industry, read [How to Enhance Campus Security with AI-Driven Safety Procedures](https://hero.page/blog/academic-and-university/campus-security-officer/how-to-enhance-campus-security-with-ai-driven-safety-procedures/170712)

### What is HeroML?
HeroML is an AI Prompt Chain/Workflow interpreter for Apps built on https://hero.page 

To see other apps, visit the [Hero Apps](https://hero.page/apps) page or explore [AI Apps for all industries](https://hero.page/blog) in the blog section

For more documentation, visit [Hero docs, and learn about AI App Workflows](https://hero.page/tutorials/introduction-to-heroml)

Download [VSCode Syntax Highlighter Ext. here](https://marketplace.visualstudio.com/items?itemName=hero-page.heroml)

## Run with HeroCLI (Requires OpenAI Token)

#### Installation

To install the HeroML CLI tool, you need to have Node.js and npm (comes with Node.js) installed on your machine. If you don't have these, please install them first. 

Then, run the following command in your terminal:

```bash
npm install -g heroml
```

This will install the HeroML CLI tool globally on your system, allowing you to use the `hero` command from any directory.

If you don't want to install it globally, you can run:

```bash
npm install heroml
```

and use it like:

```bash
npx hero run ./academic_security_protocol_ai_planner.heroml
```

We'll be using `hero run ...` in this tutorial for simplicity.

#### Configuration

Before using the HeroML CLI tool, you need to configure your OpenAI API key. 

Create a `heroconfig.json` file in your home directory with the following content:

```json
{
  "openaiApiKey": "your-openai-api-key"
}
```

Replace `"your-openai-api-key"` with your actual OpenAI API key.

#### Usage

To run a HeroML script, use the `run` command followed by the path to your script:

```bash
hero run ./academic_security_protocol_ai_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_security_protocol_ai_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_security_protocol_ai_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_security_protocol_ai_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Security Protocol AI Planner
```
Your task is to write a "Safety Procedure" for the "Academic & University" industry, specifically for a "Campus Security Officer". 

Start by writing an introduction that highlights the importance and purpose of the safety procedure as {{safety_importance}}. This will set the tone and reiterate why it's crucial to follow safety procedures.

Here's some more context about the Safety Procedure:
Safety Importance: {{safety_importance}}
Context Limitations: {{context_limitations}}
Procedure Steps: {{procedure_steps}}
Risks Challenges: {{risks_challenges}}
Emergency Response: {{emergency_response}}
Reviews Updates: {{reviews_updates}}

->>>>

You have given an introduction to the safety procedure:

Introduction:
{{step_1}}

Next, discuss the context and limitations within which the procedure is applicable. Consider {{context_limitations}} while crafting this part because this information helps the Campus Security Officer understand when and where they should apply the procedure.

->>>>

You've established the context and limitations for the safety procedure:

Introduction:
{{step_1}}

Context and Limitations:
{{step_2}}

Moving on, break down the safety procedure in detail, sequentially describing each step to be taken in a clear and understandable manner. Consider {{procedure_steps}} and provide specific actions to be taken by security personnel.

->>>>

You've detailed the safety procedure steps:

Introduction:
{{step_1}}

Context and Limitations:
{{step_2}}

Procedure Steps:
{{step_3}}

Now, elaborate on any potential risks and challenges associated with the procedure by considering {{risks_challenges}}. This encourages proactive planning and risk management.

->>>>

You've outlined potential risks and challenges:

Introduction:
{{step_1}}

Procedure Steps:
{{step_3}}

Potential Risks and Challenges:
{{step_4}}

Next, include a section for how to respond to emergencies or irregular situations that could arise during the procedure by considering {{emergency_response}}. This allows Campus Security Officers to anticipate and effectively respond to issues.

->>>>

The safety procedure now includes emergency response guidelines:

Procedure Steps:
{{step_3}}

Potential Risks and Challenges:
{{step_4}}

Emergency Response:
{{step_5}}

Finally, conclude with reviews and updates on the procedure. Consider {{reviews_updates}} to ensure the procedure remains relevant and effective.


```

