# Science Fair Project & Passion Proposal

Science Fair Project & Passion Proposal is an innovative app that leverages advanced AI techniques to create personalized, comprehensive content for Student's science fair projects. This app goes beyond just providing a step-by-step blueprint of a project. It integrates user-specified variables to generate detailed content that expresses the student's genuine love for science and their commitment to contributing to its advancement. The content is artfully crafted with expertise to encompass areas like motivation, objectives, hypothesis, methodology, expected results, timeline, and conclusion. Additionally, the app ensures that the project's significance to the wider scientific world is well-articulated. Combining technical details alongside a clear depiction of the student's enthusiasm, the app engages a wide audience by offering scientific rigor without sacrificing readability.

To run this app online: [Science Fair Project & Passion Proposal Online](https://hero.page/app/science-fair-project-and-passion-proposal-customized-science-project-proposals/DuPX6wzDRaF1SgiY9aTF)

[![Run Science Fair Project & Passion Proposal Online](/assets/run.svg)](https://hero.page/app/science-fair-project-and-passion-proposal-customized-science-project-proposals/DuPX6wzDRaF1SgiY9aTF)

To learn more about AI Apps for Science Fair Participant use-cases in the High School Students - Sciences industry, read [How to Excel in Science Fair with AI-Powered Creation Tools](https://hero.page/blog/ai/high-school-students-sciences/how-to-excel-in-science-fair-with-ai-powered-creation-tools/170965)

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
npx hero run ./science_fair_project_and_passion_proposal.heroml
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
hero run ./science_fair_project_and_passion_proposal.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./science_fair_project_and_passion_proposal.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./science_fair_project_and_passion_proposal.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./science_fair_project_and_passion_proposal.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

