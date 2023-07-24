# University Admissions Promo AI

Harness the power of AI with University Admissions Promo AI, designed to provide users with the ability to customize prompts for generating quality promotional content. This AI-driven app delivers unique insights, straight from the perspective of an Admissions Officer, propelling university admissions promotion to new heights. Experience high-quality content promoting university benefits, academic programs, testimonials from successful alumni, financial aid details, and compelling calls-to-action—all at your fingertips. Stand out with our tool's unique ability to demystify the admissions process and highlight university features potential students will love.

To run this app online: [University Admissions Promo AI Online](https://hero.page/app/university-admissions-promo-ai-ai-driven-admissions-insights-and-promotion/eHf3lXJLxsbmONoZJgCW)

To learn more about AI Apps for Admissions Officer use-cases in the Academic & University industry, read [How to Streamline University Admissions with 3 AI Tools](https://hero.page/blog/academic-and-university/admissions-officer/how-to-streamline-university-admissions-with-3-ai-tools/170703)

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
npx hero run ./university_admissions_promo_ai.heroml
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
hero run ./university_admissions_promo_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./university_admissions_promo_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./university_admissions_promo_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./university_admissions_promo_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for University Admissions Promo AI
```
First, let's start by creating an engaging introduction that briefly describes your university and its strengths relating to {{University_description}}.

Here's some more context about the Promotional Material:
University Description: {{University_description}}
Distinguished Programs: {{Distinguished_programs}}
Admissions Process: {{Admissions_process}}
Uniqueness And Benefits: {{Uniqueness_and_Benefits}}
Testimonials: {{Testimonials}}
Financial Assistance: {{Financial_assistance}}
Call To Action: {{Call_to_action}}

->>>>

Now, we have an introductory description of our university:

University Introduction:
{{step_1}}

Next, let's highlight distinguished programs, academic departments, or unique opportunities offered at your university using the content from {{Distinguished_programs}}.

->>>>

Our university has been introduced and we have highlighted distinguished programs:

University Introduction:
{{step_1}}

Highlighted Programs:
{{step_2}}

Moving on, let's break down the admissions process in a clear, step-by-step manner using the content from {{Admissions_process}}.

->>>>

For the university we have an introduction, highlighted programs and now the admissions process:

University Introduction:
{{step_1}}

Highlighted Programs:
{{step_2}}

Admissions Process:
{{step_3}}

Next, include compelling reasons why choosing your university is advantageous, with a focus on the benefits to the students and their career prospects. Use content from {{Uniqueness_and_Benefits}}.

->>>>

Our promotional material includes an introduction to the university, outlined programs, the admissions process, along with the unique benefits of choosing our university:

University Introduction:
{{step_1}}

Highlighted Programs:
{{step_2}}

Admissions Process:
{{step_3}}

Uniqueness and Benefits:
{{step_4}}

Now, we will focus on the students and alumni. Please narrate testimonials from successful students/alumni, focusing on how the university contributed to their success using content from {{Testimonials}}.

->>>>

In our promotional material we have inclusion of the university introduction, highlighted programs, admissions process, benefits of choosing our university, and testimonials from students and alumni:

University Introduction:
{{step_1}}

Highlighted Programs:
{{step_2}}

Admissions Process:
{{step_3}}

Uniqueness and Benefits:
{{step_4}}

Testimonials:
{{step_5}}

Let's discuss financial aid options. Promote financial aid options, scholarships, and grants available to students, if any, using {{Financial_assistance}} information provided.


```

