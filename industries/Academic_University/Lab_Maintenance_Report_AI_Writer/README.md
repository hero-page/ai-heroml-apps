# Lab Maintenance Report AI Writer

The Lab Maintenance Report AI Writer's innovative features allow a Lab Technician to customize inputs, creating finely detailed content. It not only generates a comprehensive maintenance report, evaluating the current state of all lab equipment but also includes industry-specific terminologies. Further, it concludes with a future strategy plan, improving maintenance tasks and suggesting equipment upgrades. It revolutionizes record-keeping, offering a unique depth of detail that's forward-oriented.

To run this app online: [Lab Maintenance Report AI Writer Online](https://hero.page/app/lab-maintenance-report-ai-writer-strategic-lab-equipment-maintenance-tracker/VccttfVW0JB4Xj53n29H)

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
npx hero run ./lab_maintenance_report_ai_writer.heroml
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
hero run ./lab_maintenance_report_ai_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./lab_maintenance_report_ai_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./lab_maintenance_report_ai_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./lab_maintenance_report_ai_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Lab Maintenance Report AI Writer
```
Start by writing the introduction for the "Maintenance Report" that states the purpose of the report and provides some context about the lab: {{lab_context}}.

Here's some more context about the Maintenance Report:
Lab Context: {{lab_context}}
Lab Equipment: {{lab_equipment}}
Maintenance Tasks: {{maintenance_tasks}}
Equipment Issues: {{equipment_issues}}
Equipment Evaluation: {{equipment_evaluation}}
Industry Specific Information: {{industry_specific_information}}
Future Plan: {{future_plan}}

->>>>

We are composing a "Maintenance Report" for the "Academic & University" industry for a "Lab Technician". So far, we have the introduction for the report:

Introduction:
{{step_1}}

Now, we need to write a general overview of the lab equipment functioning- {{lab_equipment}}.

->>>>

Having written our introduction, we proceed with the "Maintenance Report". We now have a general overview of the lab equipment functioning:

Introduction:
{{step_1}}

Equipment Overview:
{{step_2}}

The next step involves composing a detailed section highlighting all maintenance tasks performed during the reporting period, including dates, key findings, and works carried out: {{maintenance_tasks}}.

->>>>

With the equipment overview covered, let's look into the maintenance tasks done during the period:

Introduction:
{{step_1}}

Equipment Overview:
{{step_2}}

Maintenance Tasks:
{{step_3}}

Now, we have to elaborate on any encountered issues, malfunctions, or breakdowns during the maintenance routine or operation of the lab equipment: {{equipment_issues}}.

->>>>

After detailing the maintenance tasks, we have also highlighted the issues encountered during the process:

Introduction:
{{step_1}}

Maintenance Tasks:
{{step_3}}

Equipment Issues:
{{step_4}}

Now, we need to provide an evaluation of the current condition of all lab equipment, indicating which ones are in good condition, which require attention or reparations, and which have been or need to be replaced: {{equipment_evaluation}}.

->>>>

We have described the maintenance tasks performed and the equipment issues encountered. Now, we've evaluated the condition of all lab equipment:

Maintenance Tasks:
{{step_3}}

Equipment Issues:
{{step_4}}

Equipment Evaluation:
{{step_5}}

Next, incorporate specific academic, scientific, or technical information relevant to the lab and its functions into the report. These should pertain to the lab context, the usage of equipment, or the nature of the maintenance tasks: {{industry_specific_information}}.

->>>>

We have evaluated the condition of our lab equipment. We also added relevant academic, scientific, or technical information:

Equipment Evaluation:
{{step_5}}

Industry-specific Information:
{{step_6}}

Lastly, we need to conclude the report with a plan for future maintenance tasks, areas of improvement, proposed equipment upgrades or replacements, and a summary of any ongoing maintenance projects: {{future_plan}}.


```

