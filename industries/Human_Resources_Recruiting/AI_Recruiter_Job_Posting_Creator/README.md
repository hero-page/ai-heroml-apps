# AI Recruiter Job Posting Creator

AI Recruiter Job Posting Creator, an AI-driven personalized job listings app, empowers users to define variables for customized outputs. The smart app creates detailed recruiter job postings for the HR and recruitment sector. It amalgamates engaging job titles, company insights, role responsibilities, required qualifications, compensation details, and application processes. Its key feature is the incorporation of industry-specific data like role types, recruitment strategy, HR team structure, necessary HR software knowledge, and workspace details. Such unique detailing transforms a standard job listing into an informative guide for prospective candidates, providing clear insight into role requirements and company expectations.

To run this app online: [AI Recruiter Job Posting Creator Online](https://hero.page/app/ai-recruiter-job-posting-creator-ai-driven-personalized-recruiter-job-listings/7oDSD1MpkgCp70BZi8dO)

[![Run AI Recruiter Job Posting Creator Online](/assets/run.svg)](https://hero.page/app/ai-recruiter-job-posting-creator-ai-driven-personalized-recruiter-job-listings/7oDSD1MpkgCp70BZi8dO)

To learn more about AI Apps for Recruiter use-cases in the Human Resources & Recruiting industry, read [How to Automate HR Recruiting with AI-Generated Emails and Interviews](https://hero.page/blog/ai/human-resources-and-recruiting/how-to-automate-hr-recruiting-with-ai-generated-emails-and-interviews/170989)

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
npx hero run ./ai_recruiter_job_posting_creator.heroml
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
hero run ./ai_recruiter_job_posting_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_recruiter_job_posting_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_recruiter_job_posting_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_recruiter_job_posting_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

