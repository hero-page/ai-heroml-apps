# Fitness Blogger Workout Planner AI

Fitness Blogger Workout Planner AI is your ultimate AI-powered workout guide, specifically curated for fitness bloggers. This intuitive app creates custom workout plans based on your input. You can choose different aspects of your workout, from warm-up routines, strength training, to cooldown exercises. The AI generates high-quality content with detailed instructions, proper form tips, and a schedule that you can easily adjust. It offers nutritional advice tailored to your workout intensity and progression guidelines for advanced users. Each output is comprehensive and focused on your fitness goals. The app's distinct feature lies in its uniquely crafted plans catering specifically to fitness bloggers, taking into account every aspect, making it beneficial and comprehensive.

To run this app online: [Fitness Blogger Workout Planner AI Online](https://hero.page/app/fitness-blogger-workout-planner-ai-ai-powered-fitness-plan-generator/26mEKolGlCRhKWfv8Rde)

[![Run Fitness Blogger Workout Planner AI Online](/assets/run.svg)](https://hero.page/app/fitness-blogger-workout-planner-ai-ai-powered-fitness-plan-generator/26mEKolGlCRhKWfv8Rde)

To learn more about AI Apps for Fitness Blogger use-cases in the Health & Fitness Blogs industry, read [How to Accelerate Fitness Blogging with AI-Generated Workout and Nutrition Plans](https://hero.page/blog/ai/health-and-fitness-blogs/how-to-accelerate-fitness-blogging-with-ai-generated-workout-and-nutrition-plans/170936)

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
npx hero run ./fitness_blogger_workout_planner_ai.heroml
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
hero run ./fitness_blogger_workout_planner_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./fitness_blogger_workout_planner_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./fitness_blogger_workout_planner_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./fitness_blogger_workout_planner_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

