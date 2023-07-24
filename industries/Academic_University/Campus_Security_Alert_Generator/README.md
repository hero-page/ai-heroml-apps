# Campus Security Alert Generator

Discover a refreshing way to secure your campus with the Campus Security Alert Generator app, powered by advanced AI-technology. Easily specify your prompts and let the app generate specific, high-quality security alerts for potential incidents. Tailored for the university environment, it provides step-by-step safety precautions and actionable insight from a Campus Security Department perspective. Engage your campus community effectively and promote safety dynamically. Its emphasis on relevance makes the app uniquely suitable for academic settings.

To run this app online: [Campus Security Alert Generator Online](https://hero.page/app/campus-security-alert-generator-ai-powered-university-security-alerts/ZqQKpn7c8uHi05bfGTv5)

To learn more about AI Apps for Campus Security Officer use-cases in the Academic & University industry, read [How to Enhance Campus Security with AI-Driven Safety Procedures](https://hero.page/blog/academic-and-university/campus-security-officer/how-to-enhance-campus-security-with-ai-driven-safety-procedures/170712)

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
npx hero run ./campus_security_alert_generator.heroml
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
hero run ./campus_security_alert_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./campus_security_alert_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./campus_security_alert_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./campus_security_alert_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Campus Security Alert Generator
```
Your task is to write a security alert for the Academic & University industry, specifically for a Campus Security Officer. 

Start by creating an introduction that summarizes the purpose of the alert: {{security_issue}}.

Here's some more context about the Security Alert:
Security Issue: {{security_issue}}
Security Issue Details: {{security_issue_details}}
Precautionary Steps: {{precautionary_steps}}
Actions Taken: {{actions_taken}}
Security Contact Details: {{security_contact_details}}
Closing Note: {{closing_note}}

->>>>

In preparing our security alert, we have begun with an introduction:

Introduction:
{{step_1}}

The next step is to detail the nature of the security issue, including where and when it occurred, and who may be involved: {{security_issue_details}}.

->>>>

In the Security Alert, we have the introduction and the details of the security issue as follows:

Introduction:
{{step_1}}

Security Issue Details:
{{step_2}}

Next, provide instructions for the campus community members about the precautionary measures they should undertake: {{precautionary_steps}}.

->>>>

With the introduction and details of the security issue available for our Security Alert, let's lay out the precautionary steps:

Introduction:
{{step_1}}

Security Issue Details:
{{step_2}}

Precautionary Steps:
{{step_3}}

With that in place, present information about the involved entities and describe the actions being taken by the Campus Security Department: {{actions_taken}}.

->>>>

For the Security Alert, these are the details we have until now:

Introduction:
{{step_1}}

Security Issue Details:
{{step_2}}

Precautionary Steps:
{{step_3}}

Actions Taken:
{{step_4}}

Now, include contact information where community members can report any related suspicious activity or learn more about the issue: {{security_contact_details}}.


```

