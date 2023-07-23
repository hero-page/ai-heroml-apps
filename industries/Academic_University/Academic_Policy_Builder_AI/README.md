# Academic Policy Builder AI

Academic Policy Builder AI, an AI-Powered University Policy Generator, offers its users the ability to input variables to create custom, comprehensive policy documents for academic professionals. The AI-based app generates top-notch content outlining the policy's objective, execution guidelines, compliance consequences, review process, and more, entirely tailored to the user's needs. Its distinct quality lies in the detailed, academic industry-focused policy creation, offering robust guidance on implementation and after-service support. Your go-to tool for admin-friendly policy documents.

To run this app online: [Academic Policy Builder AI Online](https://hero.page/app/academic-policy-builder-ai-ai-powered-university-policy-generator/NDgY3KgEoeLBOcVaKzIO)

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
npx hero run ./academic_policy_builder_ai.heroml
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
hero run ./academic_policy_builder_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_policy_builder_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_policy_builder_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_policy_builder_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Policy Builder AI
```
Your task is to write a "Policy Document" for the "Academic & University" industry, specifically for an "Administrator". Let's begin by providing an introduction that outlines the policy's objective: {{policy_objective}}. This should explain why the policy is being created and what it aims to achieve in the university setting.

Here's some more context about the Policy Document:
Policy Objective: {{policy_objective}}
Policy Statement: {{policy_statement}}
Policy Scope: {{policy_scope}}
Procedural Guidelines: {{procedural_guidelines}}
Review Process: {{review_process}}

->>>>

Now, you have an introduction to our "Policy Document" that outlines the policy's objective:

Introduction and Objective:
{{step_1}}

Next, provide a clear statement of the policy: {{policy_statement}}. This includes the official policy that has been decided upon and is in effect, detailing the specific actions, behavior, or standards expected within the university environment.

->>>>

Now, we have an introduction and a clear policy statement for our "Policy Document":

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Continue with the task by describing the scope of the policy: {{policy_scope}}. Specify who or which departments are affected by the policy and how it will be integrated into the administrative operations.

->>>>

We have created an introduction, a policy statement, and defined the scope of our "Policy Document":

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Policy Scope:
{{step_3}}

Moving on, break down the procedural guidelines: {{procedural_guidelines}}. Outline the steps that need to be taken to follow the policy. Be clear and precise to avoid any ambiguity in the procedure.

->>>>

Now, we have an introduction, policy statement, policy scope, and procedural guidelines for our "Policy Document":

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Policy Scope:
{{step_3}}

Procedural Guidelines:
{{step_4}}

Now, incorporate the consequences for non-compliance: {{non-compliance_consequences}}. By stating the potential ramifications for failing to adhere to the policy, administrators and stakeholders will understand the seriousness of the policy.

->>>>

For our "Policy Document", we now have the introduction, policy statement, policy scope, procedural guidelines, and consequences for non-compliance:

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Policy Scope:
{{step_3}}

Procedural Guidelines:
{{step_4}}

Non-compliance Consequences:
{{step_5}}

Proceed to detail the policy's review process: {{review_process}}. Specify how often the policy will be evaluated, who will review it, and how amendments can be made if necessary.

->>>>

For our "Policy Document", we have the introduction, policy statement, policy scope, procedural guidelines, non-compliance consequences, and policy's review process:

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Policy Scope:
{{step_3}}

Procedural Guidelines:
{{step_4}}

Non-compliance Consequences:
{{step_5}}

Policy's Review Process:
{{step_6}}

Next step would be to include industry-specific elements that address the particular needs and challenges of the academic sector. For example, consider the relevance of academic freedom, the primacy of research integrity, the importance of diversity and inclusivity, and other guiding principles and laws that protect students and staff.

->>>>

The elements of our "Policy Document" now include the introduction, policy statement, policy scope, procedural guidelines, non-compliance consequences, policy's review process, and industry-specific elements:

Introduction and Objective:
{{step_1}}

Policy Statement:
{{step_2}}

Policy Scope:
{{step_3}}

Procedural Guidelines:
{{step_4}}

Non-compliance Consequences:
{{step_5}}

Policy's Review Process:
{{step_6}}

Industry-specific Elements:
{{step_7}}

Conclude the document by reiterating the policy's objective: {{policy_objective}} and the positive impact it is designed to have on the university.


```

