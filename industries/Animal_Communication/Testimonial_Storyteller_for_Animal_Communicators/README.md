# Testimonial Storyteller for Animal Communicators

Testimonial Storyteller for Animal Communicators, an AI-powered app creating unique animal tales and transformations, is your companion for generating professionally curated client testimonials. Users can specify variables in prompts, allowing customization to create high-quality, detailed accounts of clients' experiences with animal communicators. The AI generates testimonials that include initial problem, process, results, and transformed beliefs, highlighting the practitioner's unique skills, empathy and professionalism. The intricate narrative includes direct client quotes, reinforcing the credibility of the practice and showcasing the transformational journey of clients. Enjoy crafting compelling animal communicator stories like never before.

To run this app online: [Testimonial Storyteller for Animal Communicators Online](https://hero.page/app/testimonial-storyteller-for-animal-communicators-ai-powered-animal-tales-and-transformations/vHkyI7b6F214KY7XRwj0)

[![Run Testimonial Storyteller for Animal Communicators Online](/assets/run.svg)](https://hero.page/app/testimonial-storyteller-for-animal-communicators-ai-powered-animal-tales-and-transformations/vHkyI7b6F214KY7XRwj0)

To learn more about AI Apps for Animal Communicator use-cases in the Animal Communication industry, read [How to Enhance Animal Communication Skills with AI Apps](https://hero.page/blog/ai/animal-communication/how-to-enhance-animal-communication-skills-with-ai-apps/170727)

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
npx hero run ./testimonial_storyteller_for_animal_communicators.heroml
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
hero run ./testimonial_storyteller_for_animal_communicators.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./testimonial_storyteller_for_animal_communicators.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./testimonial_storyteller_for_animal_communicators.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./testimonial_storyteller_for_animal_communicators.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Testimonial Storyteller for Animal Communicators
```
Let's create a "Client Anonymized Testimonial" for the "Animal Communication" industry for an "Animal Communicator". 

Start with writing a testimonial introduction:
1. Discuss the initial issue or reason that led to contacting the animal communicator (use the placeholder {{initial_issue}}). 
2. Incorporate any initial skepticism or apprehension (if present) the client had towards animal communication (using placeholder {{initial_apprehension}}).

Here's some more context about the Client Anonymized Testimonial:
Initial Issue: {{initial_issue}}
Initial Apprehension: {{initial_apprehension}}
Communication Process: {{communication_process}}
Positive Discoveries: {{positive_discoveries}}
Improvement Outcome: {{improvement_outcome}}
Client Relief: {{client_relief}}
Client Final Thoughts: {{client_final_thoughts}}
Future Plans: {{future_plans}}
Echo Key Points: {{echo_key_points}}
Direct Quote: {{direct_quote}}

->>>>

We now have a testimonial introduction:

Introduction:
{{step_1}}

Next, we need to describe how the Animal Communicator's intervention unfolded:
3. Describe the process the animal communicator used to connect with the animal (using the placeholder {{communication_process}}).
4. Highlight any unexpected or positive findings that emerged from the communicator's intervention, thereby showcasing their unique value (using the placeholder {{positive_discoveries}}).

->>>>

We've written the part about the Animal Communicator's intervention:

Animal Communicator's Intervention:
{{step_2}}

Now, let's talk about the improvement and resolution:
5. Discuss changes in the animals' behavior, health, or overall well-being after the intervention (with placeholder {{improvement_outcome}}).
6. Explain the resulting tranquility or resolution the clients' experienced due to the communicator's intervention (with placeholder {{client_relief}}).

->>>>

We now have the section about improvements and resolution:

Improvements and Resolution:
{{step_3}}

Next, let's express the client's final thoughts:
7. Narrate the client's newfound  belief in the effectiveness and value of the animal communication industry after experiencing the communicator's work (using placeholder {{client_final_thoughts}}).
8. Discuss any future plans the client has to continue collaborating with the animal communicator (use placeholder {{future_plans}}).


```

