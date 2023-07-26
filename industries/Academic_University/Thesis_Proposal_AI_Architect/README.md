# Thesis Proposal AI Architect

Thesis Proposal AI Architect is an AI-oriented app, helping users generate extensive, top-quality thesis proposals. By incorporating user-specified variables in prompts, our app expertly crafts well-rounded proposals, detailing research objectives, topics, and significance, literature reviews, methodologies, discussions on thesis's worth, timelines, and well-crafted abstracts. Its unique feature - the thorough, academic style, coupled with the proposal's all-encompassing nature, makes it invaluable in academia.

To run this app online: [Thesis Proposal AI Architect Online](https://hero.page/app/thesis-proposal-ai-architect-ai-powered-comprehensive-thesis-proposals/IxrqrRbYKXKJCgiBbzMM)

[![Run Thesis Proposal AI Architect Online](/assets/run.svg)](https://hero.page/app/thesis-proposal-ai-architect-ai-powered-comprehensive-thesis-proposals/IxrqrRbYKXKJCgiBbzMM)

To learn more about AI Apps for Graduate Student use-cases in the Academic & University industry, read [How to Elevate University Research with AI Assistance](https://hero.page/blog/ai/academic-and-university/how-to-elevate-university-research-with-ai-assistance/170700)

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
npx hero run ./thesis_proposal_ai_architect.heroml
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
hero run ./thesis_proposal_ai_architect.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./thesis_proposal_ai_architect.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./thesis_proposal_ai_architect.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./thesis_proposal_ai_architect.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Thesis Proposal AI Architect
```
Start by writing an introduction for the "Thesis Proposal". The introduction should clearly outline the research topic: {{research_topic}}. Additionally, explain the significance and relevance of the topic in relation to existing academic literature in the "Academic & University" industry.

Here's some more context about the Thesis Proposal:
Research Topic: {{research_topic}}
Research Objectives: {{research_objectives}}

->>>>

After having an introduction for our "Thesis Proposal" about the {{research_topic}}:

Introduction:
{{step_1}}

Proceed to write a literature review. This section should present a brief survey of previous studies and scholarly discussions related to the {{research_topic}} to establish a context for the proposal.

->>>>

In our "Thesis Proposal", we have an introduction and a literature review:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Now, let's state the research objectives {{research_objectives}}, detailing what you aim to achieve through your research. The objectives should be clear, concise, and offer a directed path to the proposal.

->>>>

We have progressed through the "Thesis Proposal" with an introduction, a literature review, and research objectives:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Research Objectives:
{{step_3}}

The next step is to provide details on the proposed methodology. This section should explicate how you plan to meet the {{research_objectives}}, detailing the intended approach, methods of data collection, anticipated challenges, and potential solutions.

->>>>

In our "Thesis Proposal", we now have an introduction, a literature review, clearly defined objectives, and a comprehensive methodology:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Research Objectives:
{{step_3}}

Proposed Methodology:
{{step_4}}

Next is to argue for the significance of the proposed thesis. You should explain how your study will contribute to the body of knowledge in your field, and how it will differ from other studies on the {{research_topic}}.

->>>>

Our progressing "Thesis Proposal" contains an introduction, a literature review, research objectives, a methodology, and an argument for the significance of the thesis:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Research Objectives:
{{step_3}}

Proposed Methodology:
{{step_4}}

Significance of the Thesis:
{{step_5}}

Now that you have the main part of your "Thesis Proposal", elaborate on an anticipated timeline that itemizes specific tasks and when they will be undertaken to successfully accomplish the {{research_objectives}}.

->>>>

In our "Thesis Proposal", we have an introduction, a literature review, clear objectives, a methodology, a description of the thesis's significance, and a timeline:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Research Objectives:
{{step_3}}

Proposed Methodology:
{{step_4}}

Significance of the Thesis:
{{step_5}}

Proposed Timeline:
{{step_6}}

Proceed to prepare a list of potential bibliographical references that you plan to utilize in your research. The references should be up-to-date, relevant, and adhere to your institution's citation style.

->>>>

Our "Thesis Proposal" now has an introduction, a literature review, research objectives, a methodology, a discussion on the significance of the thesis, a timeline, and a list of references:

Introduction:
{{step_1}}

Literature Review:
{{step_2}}

Research Objectives:
{{step_3}}

Proposed Methodology:
{{step_4}}

Significance of the Thesis:
{{step_5}}

Proposed Timeline:
{{step_6}}

References:
{{step_7}}

Finish the "Thesis Proposal" by writing a conclusion that doubles as an abstract. This section should encapsulate the scope, purpose, and methodology of the proposed study on the {{research_topic}} in a valuable and enticing manner.


```

