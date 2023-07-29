# Math Model Maker for High School

Develop your problem-solving skills with Math Model Maker for High School - your advanced math assistant. This comprehensive math problem solver uses AI to generate custom, high-quality content based on your specified variables. The app crafts a complete mathematical model that includes defining the problem, identifying variables, formulating equations, discussing assumptions, and comparing predictions. Ideal for high school math club members dealing with real-world problems or mathematical challenges relevant to Math Olympiads or college entrance exams. Enhance your learning experience with its detailed, engaging, and applicable models.

To run this app online: [Math Model Maker for High School Online](https://hero.page/app/math-model-maker-for-high-school-comprehensive-math-problem-solver/sym75sbf1JIg1ar5kRaY)

[![Run Math Model Maker for High School Online](/assets/run.svg)](https://hero.page/app/math-model-maker-for-high-school-comprehensive-math-problem-solver/sym75sbf1JIg1ar5kRaY)

To learn more about AI Apps for Math Club Member use-cases in the High School Students - Mathematics industry, read [How to Excel in Math Competitions with AI-Powered Apps](https://hero.page/blog/ai/high-school-students-mathematics/how-to-excel-in-math-competitions-with-ai-powered-apps/170960)

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
npx hero run ./math_model_maker_for_high_school.heroml
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
hero run ./math_model_maker_for_high_school.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./math_model_maker_for_high_school.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./math_model_maker_for_high_school.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./math_model_maker_for_high_school.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

