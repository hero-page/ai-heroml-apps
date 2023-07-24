# University Incident Report AI

University Incident Report AI, subtitled Campus Security Incident Reporting, is a robust application that uses advanced AI to generate accurate and highly detailed incident reports within an academic or university setting. The specialized application allows users to clearly specify variables, ensuring reports can be customized to cover all relevant details, including incident nature, time, location, sequence of events, involved parties, security actions, property inventory, evidence, and future preventative measures. The generated content is specifically tailored for Campus Security Officers in a unique context, underlining the importance of accuracy, confidentiality, and punctuality in reporting incidents.

To run this app online: [University Incident Report AI Online](https://hero.page/app/university-incident-report-ai-campus-security-incident-reporting/UQaTvUpnohXdNIOzn7O4)

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
npx hero run ./university_incident_report_ai.heroml
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
hero run ./university_incident_report_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./university_incident_report_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./university_incident_report_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./university_incident_report_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for University Incident Report AI
```
For generating an "Incident Report" in the "Academic & University" industry for a "Campus Security Officer", let's begin with drafting an initial summary that briefly describes the nature of {{nature_of_incident}}. Use clear, concise, and formal language suitable for official records. Accuracy and honesty are paramount.

Here's some more context about the Incident Report:
Nature Of Incident: {{nature_of_incident}}
Time Date Location: {{time_date_location}}
Detailed Description: {{detailed_description}}
Involved Parties: {{involved_parties}}
Immediate Action Taken: {{immediate_action_taken}}
Subsequent Action Taken: {{subsequent_action_taken}}
Property Involved: {{property_involved}}
Evidence Collected: {{evidence_collected}}
Incident Summary: {{incident_summary}}

->>>>

Having described the nature of the incident, we now have:

Incident Summary:
{{step_1}}

Next, specify the exact time, date, and location where the incident occurred: {{time_date_location}}.

->>>>

We have the time, date, and location of the incident:

Incident Time, Date & Location:
{{step_2}}

Now, using any quoted witness statements or other direct sources, let's provide an in-depth description of the incident, explaining what took place in a sequential manner: {{detailed_description}}.

->>>>

We have generated a detailed description of the incident:

Incident Description:
{{step_3}}

Let's go forward with listing any involved parties including witness, suspect, and victim information: {{involved_parties}}. Kindly, consider privacy guidelines and policies while mentioning any involved parties.

->>>>

Now we have the details about all parties involved in the incident:

Involved Parties:
{{step_4}}

Now, describe the immediate action taken by campus security after the incident was reported or observed: {{immediate_action_taken}}.

->>>>

We have detailed the immediate response by campus security:

Immediate Actions Taken:
{{step_5}}

Next, discuss any subsequent actions undertaken such as involving local law enforcement or campus administration: {{subsequent_action_taken}}.

->>>>

We have detailed the subsequent actions undertaken: 

Subsequent Actions Taken:
{{step_6}}

Now, take an inventory of any property that was lost, stolen, or damaged during the incident: {{property_involved}}. Keep track of the incident's impact in terms of both safety and cost to the university, which can be valuable for university policy consideration.

->>>>

Now we have outlined properties affected during the incident:

Property Involved:
{{step_7}}

Detail any evidence secured at the scene or from the CCTV footage with specifics about what the evidence indicates: {{evidence_collected}}.

->>>>

We have detailed the evidence, secured at the scene or from CCTV footage:

Evidence Collected:
{{step_8}}

As a final step, provide a conclusion that summarizes the incident, actions taken, and suggest preventative measures to avoid a similar instance in the future: {{incident_summary}}. 

Remember to complete and file the incident report in a timely manner with the correct authorities, reflecting your training in handling such incidents and using industry-specific terminology.


```

