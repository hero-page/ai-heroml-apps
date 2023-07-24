# Academic Grant Proposal Tailor

Academic Grant Proposal Tailor is a dynamic application that uses powerful AI technology to craft personalized academic grants for university projects. Users can incorporate specific factors in the app's prompts, ensuring an output attuned to each unique requirement. Delivering high-quality content, the app includes a project summary, research data, expected results, problem statement, project timeline, budget layout, and institutional capacity. A distinguishing feature is its focus on academia, incorporating specific terminologies, citation styles, and confidentiality norms corresponding to the academic field.

To run this app online: [Academic Grant Proposal Tailor Online](https://hero.page/app/academic-grant-proposal-tailor-tailored-academic-proposal-generator/yBva7rNnxGEAudtf9u5J)

To learn more about AI Apps for Grant Writer use-cases in the Academic & University industry, read [How to Streamline Grant Writing in Academia with AI Apps](https://hero.page/blog/academic-and-university/grant-writer/how-to-streamline-grant-writing-in-academia-with-ai-apps/170704)

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
npx hero run ./academic_grant_proposal_tailor.heroml
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
hero run ./academic_grant_proposal_tailor.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_grant_proposal_tailor.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_grant_proposal_tailor.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_grant_proposal_tailor.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Grant Proposal Tailor
```
Your task is to write a "Grant Proposal" for the "Academic & University" industry, specifically for a "Grant Writer". 

Let's start by writing an executive summary. This should provide a concise overview of the proposal, including the purpose, the connected research or project, its expected outcomes, and how it aligns with the goals of the funding body: {{funding_body_goals}}. 

Here's some more context about the Grant Proposal:
Funding Body Goals: {{funding_body_goals}}
Problem Statement: {{problem_statement}}
Project Aims: {{project_aims}}
Methodology: {{methodology}}
Anticipated Results: {{anticipated_results}}
Project Personnel Qualifications: {{project_personnel_qualifications}}
Project Timeline: {{project_timeline}}

->>>>

Now, we have an executive summary for our grant proposal:

Executive Summary:
{{step_1}}

Next, let's write an introduction. This part contains more background information about the problem statement or research question to be addressed: {{problem_statement}}. It should also focus on the significance of addressing this issue in the academic and university setting.

->>>>

So far, we have the executive summary and introduction for our grant proposal:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Next up, we need to present a detailed project description. This part should include information like the specific aims, methodology, and anticipated results: {{project_aims}}, {{methodology}}, and {{anticipated_results}}.

->>>>

At this point, we have the executive summary, introduction, and project description for our grant proposal:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Project Description:
{{step_3}}

Now, let's list who will be involved in the project and their roles. Detail the project personnel and their qualifications: {{project_personnel_qualifications}}. This part should highlight their expertise relevant to the project.

->>>>

So far in our proposal, we have detailed the executive summary, introduction, project description, and the project personnel:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Project Description:
{{step_3}}

Project Personnel and their Qualifications:
{{step_4}}

Next, let's outline a timeline for the project. This should include the key tasks, milestones, and expected completion dates: {{project_timeline}}.

->>>>

At this stage, our grant proposal contains the executive summary, introduction, project description, project personnel, and a comprehensive timeline:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Project Description:
{{step_3}}

Project Personnel and their Qualifications:
{{step_4}}

Project Timeline:
{{step_5}}

Next, provide a budget section. Detail the estimated total cost of the project and how funds will be allocated across different activities, materials, or personnel. Also outline any potential financial sustainability plan beyond the grant period.

->>>>

Our proposal has so far covered the executive summary, introduction, project description, project personnel, timeline, and budget:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Project Description:
{{step_3}}

Project Personnel and their Qualifications:
{{step_4}}

Project Timeline:
{{step_5}}

Budget:
{{step_6}}

Next, let's incorporate information about the institutional capacity: Describe how the university's facilities, resources, and environment support the successful completion of the project. This might include research labs, libraries, or experienced staff.

->>>>

With the addition of the preceding step, our proposal now includes the executive summary, introduction, project description, project personnel, timeline, budget, and information about the institutional capacity:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Project Description:
{{step_3}}

Project Personnel and their Qualifications:
{{step_4}}

Project Timeline:
{{step_5}}

Budget:
{{step_6}}

Institutional Capacity:
{{step_7}}

Lastly, conclude the proposal by emphasizing the impact and benefits of the proposed project to the academic community and the wider society.


```

