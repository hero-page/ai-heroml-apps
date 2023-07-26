# AgTech Case Study Content Creator

AgTech Case Study Content Creator renders customized, comprehensive case studies within the agricultural tech industry. Users can specify variables in prompts, allowing AI features to generate high quality content inclusive of problem identification, technology solution, implementation process and impacts. This app will provide a rich narrative aiding content marketers.

To run this app online: [AgTech Case Study Content Creator Online](https://hero.page/app/agtech-case-study-content-creator-agtech-innovation-and-impact-insights/Yv3WoAMhGBa4GxDoTxE8)

[![Run AgTech Case Study Content Creator Online](/assets/run.svg)](https://hero.page/app/agtech-case-study-content-creator-agtech-innovation-and-impact-insights/Yv3WoAMhGBa4GxDoTxE8)

To learn more about AI Apps for Content Marketer use-cases in the Agricultural Technology industry, read [How to Elevate AgTech Content Marketing with AI Tools](https://hero.page/blog/ai/agricultural-technology/how-to-elevate-agtech-content-marketing-with-ai-tools/170724)

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
npx hero run ./agtech_case_study_content_creator.heroml
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
hero run ./agtech_case_study_content_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./agtech_case_study_content_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./agtech_case_study_content_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./agtech_case_study_content_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AgTech Case Study Content Creator
```
Begin by creating an introductory section for our "Case Study" in the "Agricultural Technology" industry aimed at a "Content Marketer". This introduction should provide an overview of the issue or problem experienced by farmers or agribusiness and how agricultural technology could provide potential solutions. Use {{problem_overview}} as a guide.

Here's some more context about the Case Study:
Problem Overview: {{problem_overview}}
Client Description: {{client_description}}
Implementation Process: {{implementation_process}}
Results Impacts: {{results_impacts}}
Reflective Summary: {{reflective_summary}}
Innovation Highlight: {{innovation_highlight}}

->>>>

For our "Case Study" for the "Agricultural Technology" industry, we have:

Introduction:
{{step_1}}

Next, write a detailed description of the client or group that is the focus of the case study. This should include their main challenges, the agricultural technology implemented, and the reasons for this decision. Use {{client_description}} for guidance.

->>>>

The introduction for our "Agricultural Technology" case study is written:

Introduction:
{{step_1}}

Now, we have a detailed description of the client or group:

Client Description:
{{step_2}}

Moving forward, let's detail the implementation process of the agricultural technology. This should include the steps taken, difficulties faced, the additional support required, and the timelines. Refer to {{implementation_process}} while writing this section.

->>>>

Our "Case Study" for the "Agricultural Technology" industry is evolving:

Introduction:
{{step_1}}

Client Description:
{{step_2}}

We have also added details on the implementation process of the agricultural technology:

Implementation Process:
{{step_3}}

Next, delve into the results and impacts of the agricultural technology on the problem or issue initially mentioned. Be specific and include both qualitative and quantitative results that could offer insights for readers. Refer to {{results_impacts}} for guidance.

->>>>

In our "Case Study", we have an introduction, client description, and implementation process:

Introduction:
{{step_1}}

Client Description:
{{step_2}}

Implementation Process:
{{step_3}}

And now, we have captured the results and impacts of the technology:

Results and Impacts:
{{step_4}}

Now, write a conclusion to summarize the case. This should involve a reflective analysis focusing on the role of agricultural technology in dealing with the problems of the client. It should also offer potential for similar solutions in other similar agriculture contexts. Use {{reflective_summary}} for guidance.


```

