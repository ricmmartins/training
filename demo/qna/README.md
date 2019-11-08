# How to create a QnA Bot on Azure

Go to http://www.qnamaker.ai then click to sign in. Use the same credentials from Azure Portal.

<img src=../qna/pictures/1.png>

Now click to create the knowledge base

<img src=../qna/pictures/2.png>

The first step is the creation of the QnA Service, so click to create:

<img src=../qna/pictures/3.png>

After click on that, you will be redirected to Azure Portal:

<img src=../qna/pictures/4.png>

  Now fill the related fields:
		a. A name for the QnA Service
		b. Choose a subscription
		c. Choose the Pricing Tier (F0 is enough)
		d. Choose/Create a resource group
		e. Choose the resource group location if you are creating a new one
		f. Choose the Azure Search pricing tier (F is enough)
		g. Choose the location for the Azure Search Service
		h. Choose a name for the WebApp
		i. Choose a location for the WebApp
        j. Choose if you want Application Insights (not required)

<img src=../qna/pictures/5.png>

When finished the creation of the QnA Service, return to http://qnamaker.ai then click to refresh:

<img src=../qna/pictures/6.png>

Then choose the correct options and find the QnA service previously created:

<img src=../qna/pictures/7.png>

At the step 3 give a name for you knowledge base:

<img src=../qna/pictures/8.png>

At the step 4, populate your KB and choose the chit-chat for your bot:
*Note that in this case I'm using the [Microsoft Exam polices and FAQs](https://www.microsoft.com/en-us/learning/certification-exam-policies.aspx) to populate the knowledge base.*

<img src=../qna/pictures/9.png>

At the step 5 finally create your KB:

<img src=../qna/pictures/10.png>

<img src=../qna/pictures/11.png>

Then click to Save and Train:

<img src=../qna/pictures/12.png>

At the end, click to Publish tab and then Publish:

<img src=../qna/pictures/13.png>

Now that we already have our knowledge base, it's time to create the bot. To do this, click at Create bot to be redirected to Azure Portal:

<img src=../qna/pictures/14.png>

In the Azure Portal, all information already will be populated. My recommendation is only to disable the Application Insights, which for this demonstration purposes will not be required. Then click to Create:

<img src=../qna/pictures/15.png>

After the confirmation that the deployment was completed, go to resrouce group created and look for the bot:

<img src=../qna/pictures/16.png>

<img src=../qna/pictures/17.png>

Select the bot and then go to "Test in Web Chat" option to start the conversation:

<img src=../qna/pictures/18.png>

<img src=../qna/pictures/19.png>

# If you would like to use in Intelligent Kiosk, follow the below instructions:

Get the Kiosk for Windows: [https://www.microsoft.com/en-us/p/intelligent-kiosk/9nblggh5qd84](https://www.microsoft.com/en-us/p/intelligent-kiosk/9nblggh5qd84)

From the Azure Portal, go to your resource group, select the QnA service -> Keys. Then copy one of the keys available:

<img src=../qna/pictures/20.png>

Open the Intelligent Kiosk, go to Settings, look for QnA Maker and then paste the Key:

<img src=../qna/pictures/21.png>

Back to Demo Gallery and search for QnA Bot Explorer:

<img src=../qna/pictures/22.png>

Click to add:

<img src=../qna/pictures/23.png>

Give a name, a sample landing page to show the bot window over that and choose "Use a Knowledge Base from an existing QnA Maker project"

<img src=../qna/pictures/24.png>

To get the Knowledge Base ID, go to [https://www.qnamaker.ai/](https://www.qnamaker.ai/) and click at My Knowledge Bases:

<img src=../qna/pictures/25.png>

Click at View Code:

<img src=../qna/pictures/26.png>

The content highlighted is the Knowledge Base ID: a6f6a8fd-92ce-44c9-a099-09f4aa14473b

Copy and paste at Intelligent Kiosk:

<img src=../qna/pictures/27.png>

Immediately after click to create, the sample will be ready:

<img src=../qna/pictures/28.png>

Click at the below icon to expand:

<img src=../qna/pictures/29.png>

Then start the chat:

<img src=../qna/pictures/30.png>