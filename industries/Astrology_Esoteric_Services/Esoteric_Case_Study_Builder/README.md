# Esoteric Case Study Builder

The Esoteric Case Study Builder app is a powerful tool for Tarot Readers. It uses advanced AI to create customized, high-quality narratives of successful Tarot readings where readers resolve clients' issues. Each case study intricately details every step - from the initial interaction, deep dive into the tarot reading, client's response, follow-up sessions to the final outcome. It brilliantly showcases a Tarot Reader's skills, professionalism, and expertise, with a unique focus on specifics like Tarot cards spreads, card interpretations, and astrological correlations. This creates an all-encompassing view of the reader's practice for prospects to understand and appreciate.

To run this app online: [Esoteric Case Study Builder Online](https://hero.page/app/esoteric-case-study-builder-narrating-tarot-success-stories/cqL61useyYzXlc5HuMRs)

To learn more about AI Apps for Tarot Reader use-cases in the Astrology & Esoteric Services industry, read [How to Elevate Tarot Readings with AI in Astrology Services](https://hero.page/blog/ai/astrology-and-esoteric-services/how-to-elevate-tarot-readings-with-ai-in-astrology-services/170735)

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
npx hero run ./esoteric_case_study_builder.heroml
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
hero run ./esoteric_case_study_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./esoteric_case_study_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./esoteric_case_study_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./esoteric_case_study_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Esoteric Case Study Builder
```
Your task is to write a "Reading Case Study" for the "Astrology & Esoteric Services" industry, particularly for a "Tarot Reader". 

Let's start by introducing a specific client scenario that the Tarot Reader helped resolve. Briefly mention the client's issue/problem: {{client_issue}}.

Here's some more context about the Reading Case Study:
Client Issue: {{client_issue}}
Plan Of Action: {{plan_of_action}}

->>>>

We're building a case study about a Tarot Reader, and we have our initial client scenario:

Client Scenario:
{{step_1}}

Next, describe the initial interaction between the Tarot Reader and the client. Elaborate on how the Tarot Reader drew up a plan of action tailored to this specific scenario.

->>>>

The initial scenario and Tarot Reader's plan of action now look like this:

Client Scenario:
{{step_1}}

Plan of Action:
{{step_2}}

Now, dive into the actual Tarot reading process. Highlight the specific Tarot card spreads used, the interpretation of drawn cards, and how the tarot reader addressed the client's issue.

->>>>

We have the scenario, plan of action, and Tarot reading process:

Client Scenario:
{{step_1}}

Plan of Action:
{{step_2}}

Tarot Reading Process:
{{step_3}}

Next, detail the client's reaction and their initial understanding of the reading. Also, provide examples of how they implemented the insights arising from the reading into their life.

->>>>

So far, we have the scenario, plan of action, Tarot reading process, and the client's reaction following the reading:

Client Scenario:
{{step_1}}

Plan of Action:
{{step_2}}

Tarot Reading Process:
{{step_3}}

Client's Reaction and Impact:
{{step_4}}

Now, document any follow-up sessions or additional support provided by the Tarot Reader. Discuss how these subsequent sessions helped reinforce and refine the guidance provided in the initial reading.

->>>>

We now have follow-up sessions that supplemented the initial Tarot reading:

Tarot Reading Process:
{{step_3}}

Client's Reaction and Impact:
{{step_4}}

Follow-up Sessions:
{{step_5}}

To conclude, review the overall impact of the Tarot reading on the client's situation. Illustrate how the resolution/improvement of the client's issue was a direct result of the Tarot Reader's guidance.

->>>>

We have the final impact of the Tarot reading:

Follow-up Sessions:
{{step_5}}

Final Impact:
{{step_6}}

Finally, prepare a brief summary re-emphasizing the skill and professionalism of the Tarot Reader. Highlight the utility of the Tarot reading service in aiding clients through challenging scenarios.


```

