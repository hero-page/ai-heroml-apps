# Art Project Planner for Educators

The Art Project Planner for Educators, a specialized Art Education Tool, equips users to tailor art project instructions. By utilizing AI, the app generates detailed, customised content for the children's art supplies industry. It sets out aim, benefits, materials, techniques, stepwise manual, educational objectives aligning with learning milestones, safety guidelines, and future learnings strategies. The quintessence of this app is its customizability, focusing on art educators, it provides not just a comprehensive guide but also curriculum-based educational objectives, well-crafted for the children's art industry.

To run this app online: [Art Project Planner for Educators Online](https://hero.page/app/art-project-planner-for-educators-customized-art-education-tool/d7jHpPNheH3msdTCBJwa)

[![Run Art Project Planner for Educators Online](/assets/run.svg)](https://hero.page/app/art-project-planner-for-educators-customized-art-education-tool/d7jHpPNheH3msdTCBJwa)

To learn more about AI Apps for Art Educator use-cases in the Children's Art Supplies industry, read [How to Elevate Children's Art Lessons with AI Planning Tools](https://hero.page/blog/ai/children's-art-supplies/how-to-elevate-children's-art-lessons-with-ai-planning-tools/170774)

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
npx hero run ./art_project_planner_for_educators.heroml
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
hero run ./art_project_planner_for_educators.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./art_project_planner_for_educators.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./art_project_planner_for_educators.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./art_project_planner_for_educators.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Art Project Planner for Educators
```
Your task is to write an "Art Project Description" for the "Children's Art Supplies" industry, specifically tailored for an "Art Educator". 

Let's begin with an engaging introduction that outlines the art project's purpose and its benefits for children's learning and skill development: {{art_project_purpose}}.

Here's some more context about the Art Project Description:
Art Project Purpose: {{art_project_purpose}}
Art Materials: {{art_materials}}
Art Techniques: {{art_techniques}}
Art Project Steps: {{art_project_steps}}
Educational Objectives: {{educational_objectives}}
Safety Instructions: {{safety_instructions}}
Reflection Guideline: {{reflection_guideline}}

->>>>

Now, we have an engaging introduction for our Art Project Description:

Introduction:
{{step_1}}

Let's move on to describe the type of art project. This should specify the main materials that will be used: {{art_materials}} and the specific art techniques that children will learn and apply: {{art_techniques}}.

->>>>

Upon describing the type of art project, we now have:

Introduction:
{{step_1}}

Art Project Description:
{{step_2}}

Next up, let's provide detailed steps for the completion of the art project. This should describe the process, starting from collecting materials to creating the final piece: {{art_project_steps}}.

->>>>

Having given detailed steps for the art project, we now have:

Art Project Description:
{{step_2}}

Detailed Steps:
{{step_3}}

We are not done yet. Now let's include a section on educational objectives. This should explain what learning milestones the art project aligns with according to children's learning: {{educational_objectives}}.

->>>>

After providing the educational objectives, we now have:

Detailed Steps:
{{step_3}}

Educational Objectives:
{{step_4}}

Next, let's conclude the project description with a safety and supervision section. This should outline how art educators can ensure safety while conducting the project and how to keep the process organized: {{safety_instructions}}.


```

