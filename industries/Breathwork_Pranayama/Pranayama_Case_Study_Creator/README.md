# Pranayama Case Study Creator

Pranayama Case Study Creator is an AI-powered app that enables users to generate detailed, customized content, woven into an engaging case study. Users can fine-tune the prompts, defining the client's initial health state, objectives for Pranayama sessions, personalized instructions, challenges, and outcomes. The app's AI capability ensures high-quality content focused on the specific journey of Pranayama sessions, from its initiation to the transformation in client's health and lifestyle. The highlight is the client's testimonial and the reinforcement of Pranayama benefits. Unique in its approach, it offers an insightful experience.

To run this app online: [Pranayama Case Study Creator Online](https://hero.page/app/pranayama-case-study-creator-ai-powered-pranayama-journey-narrator/N1auMgevN9R8aLLhoKC7)

[![Run Pranayama Case Study Creator Online](/assets/run.svg)](https://hero.page/app/pranayama-case-study-creator-ai-powered-pranayama-journey-narrator/N1auMgevN9R8aLLhoKC7)

To learn more about AI Apps for Pranayama Instructor use-cases in the Breathwork & Pranayama industry, read [How to Elevate Pranayama Instruction with AI Tools](https://hero.page/blog/ai/breathwork-and-pranayama/how-to-elevate-pranayama-instruction-with-ai-tools/170767)

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
npx hero run ./pranayama_case_study_creator.heroml
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
hero run ./pranayama_case_study_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./pranayama_case_study_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./pranayama_case_study_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./pranayama_case_study_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Pranayama Case Study Creator
```
Let's create a "Client Anonymized Case Study" for the "Breathwork & Pranayama" industry, specifically for a "Pranayama Instructor". 

Start by writing an intriguing lead that draws the reader in. This could be a dramatic moment that took place during the client's training or a distinct problem they were facing. Fill out this variable: {{client_intro}}.

Here's some more context about the Client Anonymized Case Study:
Client Intro: {{client_intro}}
Client Background: {{client_background}}
Instruction Program: {{instruction_program}}
Challenges And Solutions: {{challenges_and_solutions}}
Results: {{results}}
Client Testimonial: {{client_testimonial}}

->>>>

We have a compelling introduction for our case study:

Client Introduction:
{{step_1}}

Next, introduce the client by setting their background. Describe their initial state of health, aspirations, and why they sought Pranayama instruction. Fill out this variable: {{client_background}}.

->>>>

Our case study now has an introduction and a detailed client background:

Client Introduction:
{{step_1}}

Client Background:
{{step_2}}

Moving on, provide an overview of the Pranayama instruction program that you designed for the client. Be sure to emphasize how it was tailored for that specific client's needs. Do not forget that we are keeping this anonymous. Use this variable: {{instruction_program}}.

->>>>

Our case study now includes details about the client's background and the instruction program:

Client Background:
{{step_2}}

Instruction Program:
{{step_3}}

Now, we want to highlight the challenges faced during the instruction period. Include difficulties in the client's learning pace, obstacles in implementing practices, or personal issues affecting their progress. Also, mention how you, as the Pranayama instructor, helped the client overcome these issues. Write this in the variable of {{challenges_and_solutions}}.

->>>>

At this point in our case study, we have discussed the instruction program and the challenges faced:

Instruction Program:
{{step_3}}

Challenges and Solutions:
{{step_4}}

Let's move onto the results. Showcase the end results by quantifying the changes in the client's health, stress levels, or overall life post-training. Illustrate how Pranayama has made a significant difference in their lifestyle. This should be filled in at {{results}}.

->>>>

For the case study, we have covered the challenges faced during the training and the end results:

Challenges and Solutions:
{{step_4}}

Results:
{{step_5}}

Let's focus on the testimonial. Conclude this section with anonymous feedback from the client about the instruction process and the changes they experienced. Write this in the variable named {{client_testimonial}}.


```

