# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

The Groq key worked pretty well. I don't see anything that should not be there and I was happy to see that it did not just give me a list of names for the people but included position or a description as well. I think my news organization could use this to keep tabs on the people they have used as sources in each article. They could aslo have it keep track of how many times a particular topic has been covered or if it is a recurring topic, making sure it is covered within a certain frequency. Also if the same entities are coming up various times (especially in the organizations part), it would help to see why these organizations are coming up multiple times recently to see if there is something deeper they should be looking out for. It could also help to see the perspectives of a person that has been quoted or used as a source before in case the news organization is thinking of using them again.
