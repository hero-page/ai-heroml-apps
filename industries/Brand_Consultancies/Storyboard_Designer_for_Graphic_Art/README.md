# Storyboard Designer for Graphic Art

Storyboard Designer for Graphic Art is a user-friendly app designed with AI technology to create highly personalized, elaborate project outlines for graphic designers. Users input variables and prompts, and the AI crafts an extensive narrative design journey. The design journey covers essential aspects like concept, objectives, requirements, deliverables, and target audience in detail, segmented into individual frames or scenes. Additionally, the app provides specific aesthetic guidelines like brand colors, fonts, and styles to shape the project's final outcome. Its unique aspect is a detailed step-by-step view of the design journey, offering a rare insight for designers.

To run this app online: [Storyboard Designer for Graphic Art Online](https://hero.page/app/storyboard-designer-for-graphic-art-ai-powered-narrative-design-journey/VHhu1L8IunCDwVmQ1jDb)

[![Run Storyboard Designer for Graphic Art Online](/assets/run.svg)](https://hero.page/app/storyboard-designer-for-graphic-art-ai-powered-narrative-design-journey/VHhu1L8IunCDwVmQ1jDb)

To learn more about AI Apps for Graphic Designer use-cases in the Brand Consultancies industry, read [How to Streamline Brand Design Workflow with AI Tools](https://hero.page/blog/ai/brand-consultancies/how-to-streamline-brand-design-workflow-with-ai-tools/170765)

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
npx hero run ./storyboard_designer_for_graphic_art.heroml
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
hero run ./storyboard_designer_for_graphic_art.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./storyboard_designer_for_graphic_art.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./storyboard_designer_for_graphic_art.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./storyboard_designer_for_graphic_art.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Storyboard Designer for Graphic Art
```
Your task is to write a "Storyboard" for the "Brand Consultancies" industry, specifically for a "Graphic Designer". 

Let's start by crafting an introduction that outlines the broad concept or theme of your project: {{project_concept}}. This is crucial for aligning the understanding and expectations within the team.

Here's some more context about the Storyboard:
Project Concept: {{project_concept}}
Project Objectives Requirements: {{project_objectives_requirements}}
Design Journey: {{design_journey}}
Audience Profile: {{audience_profile}}
Design Stages: {{design_stages}}
Branding Elements: {{branding_elements}}
Anticipated Outcome: {{anticipated_outcome}}

->>>>

At this point, we have an introduction for our storyboard:

Introduction:
{{step_1}}

Moving forward, we should add a detailed project overview, highlighting the client's requirements, project objectives, and expected deliverables: {{project_objectives_requirements}}. This will provide a comprehensive scope for the storyboard.

->>>>

We now have a project overview and an introduction for our storyboard:

Introduction:
{{step_1}}

Project Overview:
{{step_2}}

Next, weave a coherent narrative structure for the storyboard. It should logically detail the beginning, middle, and end of the design journey from the client's perspective: {{design_journey}}.

->>>>

Our Storyboard contains an introduction, a project overview, and a narrative structure:

Introduction:
{{step_1}}

Project Overview:
{{step_2}}

Narrative Structure:
{{step_3}}

Now, introduce the characters. Specifically, flesh out the target audience, their profiles, and their roles in the project: {{audience_profile}}.

->>>>

To emphasize, we now have:

Introduction:
{{step_1}}

Project Overview:
{{step_2}}

Narrative Structure:
{{step_3}}

Characters/Audience Profile:
{{step_4}}

After this, let's break the narrative structure into individual frames or scenes. These will represent the different stages of the design journey: {{design_stages}}. Ensure each stage conveys a specific action, decision, or aspect of the audience’s journey.

->>>>

Our detailed storyboard so far comprises:

Introduction:
{{step_1}}

Project Overview:
{{step_2}}

Narrative Structure:
{{step_3}}

Characters/Audience Profile:
{{step_4}}

Design Journey Stages:
{{step_5}}

Now that we have the stages, for each stage listed in {{design_stages}}, write a brief textual description of the actions or scenarios taking place.

->>>>

We have now described the actions at each stage of the design journey:

Design Journey Stages - Actions and Scenarios:
{{step_6}}

The next step is incorporating our brand specifics. Include proposed brand colors, fonts, styles, and any abstract or representative elements that would help define the aesthetic or mood of the project: {{branding_elements}}.


```

