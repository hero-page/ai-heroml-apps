# University Lab Safety Guideline Generator

The University Lab Safety Guideline Generator is a cutting-edge app that uses AI to create customized lab safety rules for university lab personnel. Users can specify variables in prompts for detailed guide creation, tailored to various lab disciplines like chemistry, biology, or physics. Building in safety procedures, equipment usage, emergency handling, or incorporating relevant regulations, the app generates a comprehensive safety document with clear language, informative content, and credible sources. This unique app meets the specific needs of the academic sector and contributes to safer lab practices.

To run this app online: [University Lab Safety Guideline Generator Online](https://hero.page/app/university-lab-safety-guideline-generator-comprehensive-university-lab-safety-guide/XSbjw8rQKBlrmKlH9Ekm)

[![Run University Lab Safety Guideline Generator Online](/assets/run.svg)](https://hero.page/app/university-lab-safety-guideline-generator-comprehensive-university-lab-safety-guide/XSbjw8rQKBlrmKlH9Ekm)

To learn more about AI Apps for Lab Technician use-cases in the Academic & University industry, read [How to Streamline Lab Procedures with AI in University Settings](https://hero.page/blog/ai/academic-and-university/how-to-streamline-lab-procedures-with-ai-in-university-settings/170711)

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
npx hero run ./university_lab_safety_guideline_generator.heroml
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
hero run ./university_lab_safety_guideline_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./university_lab_safety_guideline_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./university_lab_safety_guideline_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./university_lab_safety_guideline_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for University Lab Safety Guideline Generator
```
Your task is to write a "Lab Safety Rules" for the "Academic & University" industry, specifically for a "Lab Technician". 

Let's start with an introduction that outlines the significance of "Lab Safety Rules" in the "Academic & University" industry. This should help to convey to the lab technicians the value and importance of these rules.

Here's some more context about the Lab Safety Rules:
Significance Of Lab Safety Rules: {{significance_of_lab_safety_rules}}
General Safety Rules: {{general_safety_rules}}
Specific Lab Type: {{specific_lab_type}}
Equipment Safety Guidelines: {{equipment_safety_guidelines}}
Emergency Procedures: {{emergency_procedures}}

->>>>

Now that we have set the context for our Lab Safety Rules:

Introduction:
{{step_1}}

Next, let's compile general safety guidelines which are applicable to all types of labs. This section should include best practices for a safe lab environment, personal protective equipment, handling lab materials and dealing with emergencies or accidents.

->>>>

After presenting an introduction to our Lab Safety Rules:

Introduction:
{{step_1}}

We have now outlined the general safety rules:

General Safety Rules:
{{step_2}}

Now, let's move on to write specific lab safety rules, that reflect the unique needs and requirements of different types of labs (like chemistry, physics, or biology labs).

->>>>

We have general safety rules for a lab:

General Safety Rules:
{{step_2}}

And now, we also have specific rules for different types of labs:

Specific Lab Safety Rules:
{{step_3}}

Next, we need to include a section in the Lab Safety Rules that focuses on equipment safety. Let's outline guidelines on how to use, maintain, and dispose of various types of lab equipment safely.

->>>>

From the safety rules:

General Safety Rules:
{{step_2}}

Specific Lab Safety Rules:
{{step_3}}

Now, we have rules pertaining to equipment safety:

Equipment Safety Guidelines:
{{step_4}}

Now, let's compile a set of standard procedures that the lab technician must follow in case of a lab mishap or accident. This section should include action plans and emergency procedures for different types of adverse incidents.

->>>>

We now have safety guidelines for lab equipment:

Equipment Safety Guidelines:
{{step_4}}

Next, we provide procedures to follow in case of emergencies:

Emergency Procedures:
{{step_5}}

Let's now create a summary or conclusion that reiterates the importance of adhering to lab safety rules, potential risks of not following them, and reminders to update their knowledge of safety protocols regularly.

->>>>

We have compiled emergency procedures:

Emergency Procedures:
{{step_5}}

Now, here is the concluding summary of our "Lab Safety Rules":

Concluding Summary:
{{step_6}}

Lastly, we must include proper references to our sources of specific rules or regulations, to ensure the credibility and accuracy of our Lab Safety Rules.


```

