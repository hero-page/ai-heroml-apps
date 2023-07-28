# Adaptive E-Learning Lesson Planner

The Adaptive E-Learning Lesson Planner app utilizes AI to create highly customized lesson plans tailored to your specific e-learning platform. The app allows users to define variables in task prompts ensuring a personalized learning journey for students. The app generates high-quality, detailed content, from course objectives to evaluation criteria, making it a comprehensive tool for education and e-learning professionals. Its unique adaptability helps educators utilize platform-specific tools to maximum advantage, making teaching more effective. Additionally, lesson plans are designed for future updates, reflecting the evolving digital learning environment. Real-world examples incorporated into the plans make learning engaging and relatable for students.

To run this app online: [Adaptive E-Learning Lesson Planner Online](https://hero.page/app/adaptive-e-learning-lesson-planner-customized-platform-specific-lesson-planning/xj414hN12DoLaVHcafCm)

[![Run Adaptive E-Learning Lesson Planner Online](/assets/run.svg)](https://hero.page/app/adaptive-e-learning-lesson-planner-customized-platform-specific-lesson-planning/xj414hN12DoLaVHcafCm)

To learn more about AI Apps for Course Creator use-cases in the Education & E-learning Platforms industry, read [How to Elevate Course Creation with AI in E-Learning Platforms](https://hero.page/blog/ai/education-and-e-learning-platforms/how-to-elevate-course-creation-with-ai-in-e-learning-platforms/170852)

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
npx hero run ./adaptive_e_learning_lesson_planner.heroml
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
hero run ./adaptive_e_learning_lesson_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./adaptive_e_learning_lesson_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./adaptive_e_learning_lesson_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./adaptive_e_learning_lesson_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

