# Wellness Guide AI for Academics

Wellness Guide AI for Academics is an AI-powered app providing customized, high-quality content for Student Affairs Officers. It generates a comprehensive wellness resource guide, covering the importance of health in a university setting, offering strategic solutions for common issues, and providing a tailored resource list for further understanding. The standout feature: content is meticulously curated to address unique challenges faced specifically by these officers in their role, ensuring a holistic approach to wellness.

To run this app online: [Wellness Guide AI for Academics Online](https://hero.page/app/wellness-guide-ai-for-academics-tailored-wellness-guide-for-officers/yq05orH8XV3Nl9b6g11l)

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
npx hero run ./wellness_guide_ai_for_academics.heroml
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
hero run ./wellness_guide_ai_for_academics.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./wellness_guide_ai_for_academics.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./wellness_guide_ai_for_academics.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./wellness_guide_ai_for_academics.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Wellness Guide AI for Academics
```
Your task is to write a "Wellness Resources" for the "Academic & University" industry, specifically for a "Student Affairs Officer". 

Start by defining the main reason behind creating and using these wellness resources. What is the purpose these resources are intended to serve?

Here's some more context about the Wellness Resources:
Purpose: {{purpose}}
Specific References: {{specific_references}}
Wellness Categories: {{wellness_categories}}
Common Issues: {{common_issues}}
Resource List: {{resource_list}}

->>>>

We now have a defined purpose for our "Wellness Resources" compiled for the "Academic & University" industry:

Purpose:
{{step_1}}

Now, let's describe the role of a "Student Affairs Officer" as it pertains to health, wellness, and the relevance to their job. Remember to make specific references on the importance of health and wellness in the academic and university setting.

->>>>

So, our "Wellness Resources" has a defined purpose:

Purpose:
{{step_1}}

Additionally, we have outlined the relevance of health and wellness to the role of a "Student Affairs Officer":

Specific References:
{{step_2}}

Moving on, we need to list the different aspects of health and wellness that will be covered in the resources. This may include mental health, physical wellbeing, nutrition, exercise, self-care, and any other relevant categories.

->>>>

The "Wellness Resources", compiled for the "Academic & University" industry, now consist of the following:

Purpose:
{{step_1}}

Specific References:
{{step_2}}

Health and Wellness Categories:
{{step_3}}

Next, for each wellness category, we need to discuss strategies, tips, and approaches in detail. Ensure to provide specific advice or best practices based on the role of a "Student Affairs Officer".

->>>>

Our "Wellness Resources" for a "Student Affairs Officer" in the "Academic & University" industry currently include:

Purpose:
{{step_1}}

Specific References:
{{step_2}}

Wellness Categories & Strategies:
{{step_4}}

Next, let's address common wellness issues encountered in the university setting. Make sure to provide practical solutions that a "Student Affairs Officer" can implement to mitigate these issues.

->>>>

The "Wellness Resources" for a "Student Affairs Officer" in the "Academic & University" industry now include:

Purpose:
{{step_1}}

Specific References:
{{step_2}}

Wellness Categories & Strategies:
{{step_4}}

Common Wellness Issues and Solutions:
{{step_5}}

Now, let's reinforce the purpose of these "Wellness Resources" by writing a summary that emphasizes the importance of a balanced approach to wellness for everyone involved in the "Academic & University" setting.

->>>>

Our nearly completed "Wellness Resources" for a "Student Affairs Officer" in the "Academic & University" industry include:

Purpose:
{{step_1}}

Specific References:
{{step_2}}

Wellness Categories & Strategies:
{{step_4}}

Common Wellness Issues and Solutions:
{{step_5}}

Importance of Balanced Approach to Wellness:
{{step_6}}

Finally, create an appendix or resource list for external reading or further information on the subjects covered. Include links or references to non-academic sources for a rounded perspective on wellness subjects.


```

