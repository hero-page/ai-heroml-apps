# Student-Tailored Website Plan AI

With Student-Tailored Website Plan AI, a AI-driven app, students can specify project variables for customized content, creating comprehensive website design plans specifically suited to their needs. The sophisticated AI generates high-quality content such as website's purpose, architecture, content plan, UI design, toolset, and strategy for student engagement, website security and accessibility, plus a maintenance plan. A unique feature is its focus on strategies, incorporating educational theory and design techniques, aimed at captivating and retaining student involvement for technology and computer science educational sites, ensuring a beneficial online learning experience.

To run this app online: [Student-Tailored Website Plan AI Online](https://hero.page/app/student-tailored-website-plan-ai-ai-driven-student-focused-web-design/2gvm8KV1B1Cf9ZZm6gy7)

[![Run Student-Tailored Website Plan AI Online](/assets/run.svg)](https://hero.page/app/student-tailored-website-plan-ai-ai-driven-student-focused-web-design/2gvm8KV1B1Cf9ZZm6gy7)

To learn more about AI Apps for Student use-cases in the High School Students - Technology & Computer Science industry, read [How to Excel in Tech Studies with AI-Assisted Code Documentation, Website Design Planning and Data Analysis](https://hero.page/blog/ai/high-school-students-technology-and-computer-science/how-to-excel-in-tech-studies-with-ai-assisted-code-documentation-website-design-planning-and-data-analysis/170973)

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
npx hero run ./student_tailored_website_plan_ai.heroml
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
hero run ./student_tailored_website_plan_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./student_tailored_website_plan_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./student_tailored_website_plan_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./student_tailored_website_plan_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

