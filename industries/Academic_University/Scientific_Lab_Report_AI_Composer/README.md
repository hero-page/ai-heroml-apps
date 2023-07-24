# Scientific Lab Report AI Composer

Scientific Lab Report AI Composer, a Data Analysis & Report Generator, allows users to define variables, which are then used by the AI to generate detailed, customized lab reports. The app delivers structured outputs that include an experiment overview, defined objectives, equipment and methods used, raw results, analytical discussions, and conclusions. Proper citation and academic ethics are also emphasized. What makes this app unique is its ability to present raw data thoughtfully, introducing a thorough analysis that adds depth, authenticity, and credibility to your scientific report.

To run this app online: [Scientific Lab Report AI Composer Online](https://hero.page/app/scientific-lab-report-ai-composer-data-analysis-and-report-generator/b1EXxE0yOVcmLHw8PfQb)

To learn more about AI Apps for Undergraduate Student use-cases in the Academic & University industry, read [How to Ace University Writing with AI Academic Assistance](https://hero.page/blog/academic-and-university/undergraduate-student/how-to-ace-university-writing-with-ai-academic-assistance/170701)

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
npx hero run ./scientific_lab_report_ai_composer.heroml
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
hero run ./scientific_lab_report_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./scientific_lab_report_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./scientific_lab_report_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./scientific_lab_report_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Scientific Lab Report AI Composer
```
You are tasked with writing a detailed "Lab Report" for an "Undergraduate Student" in the "Academic & University" industry. 

To start, develop an introduction that gives a brief overview of the experiment that was conducted.

Here's some more context about the Lab Report:
Experiment Overview: {{experiment_overview}}
Experiment Objectives: {{experiment_objectives}}
Equipment And Resources: {{equipment_and_resources}}
Experiment Results: {{experiment_results}}
Analysis Of Results: {{analysis_of_results}}
Experiment Conclusions: {{experiment_conclusions}}

->>>>

We've begun our Lab Report with an introduction:

Introduction:
{{step_1}}

Next, write a clear and concise description of the experiment's objectives. This should illustrate the purpose of the experiment and the scientific principles being tested.

->>>>

We now have an introduction and a description of the objectives for our Lab Report:

Introduction:
{{step_1}}

Objectives:
{{step_2}}

For the next step, create a materials and methods section that catalogs all the tools and resources used while also detailing the process followed during the experiment. Make it comprehensive enough for another student to replicate the experiment.

->>>>

We now have three sections for our Lab Report: an introduction, objectives, and a materials and methods section.

Introduction:
{{step_1}}

Objectives:
{{step_2}}

Materials and Methods:
{{step_3}}

Now, let's construct a results section where all the collected data from the experiment are presented objectively. Refrain from including any interpretation or analysis in this section.

->>>>

Our Lab Report now includes Introduction, Objectives, Materials and Methods, and a Results section:

Introduction:
{{step_1}}

Objectives:
{{step_2}}

Materials and Methods:
{{step_3}}

Results:
{{step_4}}

Next, we need to write an analysis or discussion section where the results are interpreted. Here, draw conclusions from your data, backing up any claims with evidence from your results.

->>>>

In our Lab Report, we now have Introduction, Objectives, Methods and Materials, Results, and an Analysis section:

Introduction:
{{step_1}}

Objectives:
{{step_2}}

Materials and Methods:
{{step_3}}

Results:
{{step_4}}

Analysis:
{{step_5}}

We're almost at the end. Now, pen down a conclusion that succinctly summarizes the key findings and conclusions of your experiment. Remember to link your conclusions back to your original objectives.

->>>>

Here's what our Lab Report consists of so far: 

Introduction:
{{step_1}}

Objectives:
{{step_2}}

Materials and Methods:
{{step_3}}

Results:
{{step_4}}

Analysis:
{{step_5}}

Conclusion:
{{step_6}}

Finally, remember to include a references section listing any resources you referred to when preparing for your experiment or writing your lab report. Adhere to the referencing style prescribed by your university. 


```

