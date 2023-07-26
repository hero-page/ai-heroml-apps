# Career Guide Customizer AI

Discover the ultimate personalized career guide with Career Guide Customizer AI. Tailored to your specific needs, this AI-powered tool generates adaptable content to guide your occupational journey. Shape and refine the information based on your inputs for unique and insightful results. Whether you're a career counselor in the academic & university industry or a novitiate seeking direction, this savvy tool provides a complete guide from key competencies, ethical standards, to career progression and necessary resources. No one-size-fits-all approach, just precise, useful information uniquely fit to your career needs.

To run this app online: [Career Guide Customizer AI Online](https://hero.page/app/career-guide-customizer-ai-ai-powered-personalized-career-guidance/U5pdEUig9SGwSrEBFVKG)

[![Run Career Guide Customizer AI Online](/assets/run.svg)](https://hero.page/app/career-guide-customizer-ai-ai-powered-personalized-career-guidance/U5pdEUig9SGwSrEBFVKG)

To learn more about AI Apps for Career Counselor use-cases in the Academic & University industry, read [How to Enhance Career Development with AI in Academia](https://hero.page/blog/ai/academic-and-university/how-to-enhance-career-development-with-ai-in-academia/170707)

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
npx hero run ./career_guide_customizer_ai.heroml
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
hero run ./career_guide_customizer_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./career_guide_customizer_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./career_guide_customizer_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./career_guide_customizer_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Career Guide Customizer AI
```
Your task is to write a "Career Guide" for the "Academic & University" industry, specifically for a "Career Counselor". 

Let's begin by writing an introduction that explains the purpose of the career guide: {{purpose_of_guide}}. This introduction should provide an overview of what the Career Counselors are expected to get from the guide.

Here's some more context about the Career Guide:
Purpose Of Guide: {{purpose_of_guide}}
Recurrent Themes: {{recurrent_themes}}
Desired Competencies: {{desired_competencies}}
Selected Core Values: {{selected_core_values}}
Career Pathways And Challenges: {{career_pathways_and_challenges}}
Chosen Resources: {{chosen_resources}}

->>>>

So far, we have created the introduction for the our Career Guide:

Introduction:
{{step_1}}

Let's now write an overview of the "Career Counselor" role, highlighting duties and skills required. This section should incorporate the {{recurrent_themes}} identified from our research about the Career Counselor field.

->>>>

In our Career Guide, we have an introduction and a detailed overview of the "Career Counselor" role:

Introduction:
{{step_1}}

Role of a Career Counselor:
{{step_2}}

Next, we need to explore the key competencies and qualifications required in the Career Counseling field. This discussion should reference the {{desired_competencies}} provided by the user.

->>>>

So far in our Career Guide, we have provided an introduction, an overview of the "Career Counselor" role, and a comprehensive exploration of key competencies:

Introduction:
{{step_1}}

Role of a Career Counselor:
{{step_2}}

Key Competencies:
{{step_3}}

Given the nature of the Career Counseling job, it's important to include a section on ethics and professionalism that aligns with the {{selected_core_values}} chosen by the user.

->>>>

In our Career Guide, we have discussed the role of a Career Counselor, key competencies, and we have just added a section on ethics and professionalism:

Role of a Career Counselor:
{{step_2}}

Key Competencies:
{{step_3}}

Ethics and Professionalism:
{{step_4}}

Let's move on to present the possible career paths, advancement opportunities, and potential challenges faced by Career Counselors. Align this content with the user's input for {{career_pathways_and_challenges}}.

->>>>

So far in our Career Guide, we have outlined the role, competencies, and ethics of a Career Counselor, and we've just detailed the possible career paths:

Role of a Career Counselor:
{{step_2}}

Key Competencies:
{{step_3}}

Ethics and Professionalism:
{{step_4}}

Career Paths and Opportunities:
{{step_5}}

Next, we need to provide some resources such as relevant articles, publications, and associations for Career Counselors. Base this information on the {{chosen_resources}} supplied by the user. 


```

