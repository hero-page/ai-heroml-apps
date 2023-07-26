# Academic Memo AI Composer

Explore the vast application of AI in academics with the Academic Memo AI Composer app. Employing cutting-edge AI technology, the app aids users in crafting professional and industry-centric memos. Customize your memos by providing unique variables, receive updates on policy changes and get research insights. The AI curates content specifically for university administrators, incorporating a clear subject line, introduction, key updates, specific instructions, summary, and a formal conclusion. The final product is elegantly groomed, maintaining an official tone suitable for an academic environment. Harness the power of AI for your academic communication.

To run this app online: [Academic Memo AI Composer Online](https://hero.page/app/academic-memo-ai-composer-ai-powered-academic-memo-creation/FNZXo1jTBILdHQ1lsMYH)

[![Run Academic Memo AI Composer Online](/assets/run.svg)](https://hero.page/app/academic-memo-ai-composer-ai-powered-academic-memo-creation/FNZXo1jTBILdHQ1lsMYH)

To learn more about AI Apps for Administrator use-cases in the Academic & University industry, read [How to Streamline Academic Administration with AI Tools](https://hero.page/blog/ai/academic-and-university/how-to-streamline-academic-administration-with-ai-tools/170702)

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
npx hero run ./academic_memo_ai_composer.heroml
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
hero run ./academic_memo_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_memo_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_memo_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_memo_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Memo AI Composer
```
Your task is to write an "Internal Memo" for the "Academic & University" industry, specifically for an "Administrator". 

Let's start by crafting a welcoming, to-the-point salutation that addresses the intended recipients.

Here's some more context about the Internal Memo:
Salutation: {{salutation}}
Memo Subject: {{memo_subject}}
Purpose Of Memo: {{purpose_of_memo}}
Key Points Or Updates: {{key_points_or_updates}}
Required Actions: {{required_actions}}

->>>>

We now have a salutation for our Internal Memo:

Salutation:
{{step_1}}

Next, provide an engaging and clear subject line that captures the essence of the memo’s purpose.

->>>>

The salutation for our internal memo is:

Salutation:
{{step_1}}

We have generated a subject line for our memo:

Subject Line:
{{step_2}}

Now, begin by establishing the context and purpose of the memo in the introduction. The introduction should outline why the information is important for the recipients.

->>>>

For our internal memo, we have a salutation and subject line:

Salutation:
{{step_1}}

Subject Line:
{{step_2}}

Now, we have also established the context and purpose of our memo:

Introduction:
{{step_3}}

The next step is to provide the key points or updates in an organized and easy-to-follow manner. These points could include changes to policies or procedures, important dates, or status updates on ongoing initiatives.

->>>>

Up until now in our internal memo, we have the following components:

Introduction:
{{step_3}}

We are now presenting the key points or updates:

Key Points:
{{step_4}}

Include any relevant academic or University-specific information that might add more value and relevance to the memo. This could include curriculum changes, institutional goals, or research findings.

->>>>

In the internal memo, we have the key points and updates:

Key Points:
{{step_4}}

We have added academic or University-specific information:

Academic or University-specific Information:
{{step_5}}

Now, it's time to provide clear instructions or steps for any actions needed by parties reading the memo.

->>>>

Up until this point, our internal memo for the Academic & University industry includes:

Academic or University-specific Information:
{{step_5}}

The added instructions for the required actions are:

Required Actions:
{{step_6}}

In the conclusion, summarize the main points, and if applicable, specify a deadline for the required actions. Close the memo with a note of gratitude for the recipients' time and cooperation.


```

