# Math-Coding Project Planner AI

Math-Coding Project Planner AI allows you to specify variables in prompts, using AI to generate high-quality, customized content. The aptitude to produce comprehensive plans for math-centric coding projects at a high-school level is remarkable. Outputs include an objective, the mathematical and coding context, project description, roles, progress metrics, learning outcomes, project timeline with milestones, benefits for the club, and wider impacts. The unique feature of combining mathematical and coding contexts within a high school club project sets it apart from generic project management tools, enhancing its effectiveness in academic clubs.

To run this app online: [Math-Coding Project Planner AI Online](https://hero.page/app/math-coding-project-planner-ai-ai-planning-for-maths-coding-projects/zKTPErYL6mbLmHO7ZJY2)

[![Run Math-Coding Project Planner AI Online](/assets/run.svg)](https://hero.page/app/math-coding-project-planner-ai-ai-planning-for-maths-coding-projects/zKTPErYL6mbLmHO7ZJY2)

To learn more about AI Apps for Coding Club Member use-cases in the High School Students - Mathematics industry, read [How to Elevate Coding Projects with AI-Assisted Math Apps](https://hero.page/blog/ai/high-school-students-mathematics/how-to-elevate-coding-projects-with-ai-assisted-math-apps/170961)

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
npx hero run ./math_coding_project_planner_ai.heroml
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
hero run ./math_coding_project_planner_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./math_coding_project_planner_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./math_coding_project_planner_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./math_coding_project_planner_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

