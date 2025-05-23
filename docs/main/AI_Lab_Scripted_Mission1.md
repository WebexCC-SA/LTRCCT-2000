---
#icon: material/folder-open-outline
icon: material/medal
---


### Mission Details

Your mission is to create a new Scripted AI Agent from the template and configure basic Scripted AI Agent functionalities by adding intents and responses.

### Build

#### Task 1. Creating a AI Agent using a Template

1. <span style="color: red;">[IMPORTANT]</span> Download the [Scripted Agent](https://cisco.box.com/shared/static/q636qc41q0brifn0h8anbfug7duq3536.json){:target="_blank"}.

2. Login into [Webex Control Hub](https://admin.webex.com){:target="_blank"} by using your Admin profile **wxcclabs+admin_ID<span class="attendee-id-placeholder">Your_Attendee_ID</span>@gmail.com**. You will see another login screen with OKTA on it where you may need to enter the email address again and the password provided to you.

3. Go to Contact Center from the left side navigation panel, and under Quick Links, click on **Webex AI Agent**

    ![Profiles](../graphics/AI_Track/AI_Scripted_OpenWebexAI.gif)  

3. Click on **Import agent** to create a new AI Agent by importing preconfigured template. Click on **Upload** button, locate and select **ScriptedAIAgent.json** you downloaded at the beginning of the mission.
4. Name your Agent as **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_Scripted_AI_Agent">Your_Attendee_ID</span>_Scripted_AI_Agent<span class="copy" title="Click to copy!"></span></span>** and click **Import**
5. Make the bot live by clicking on the **Publish** button on the top right.
6. Enter **v1** in the popup window, then click **Publish**.
    ![Profiles](../graphics/Lab1_AI_Agent/5.1.gif)

7. Click on the **Preview** button on the top right side to test the bot. Try the bot flow by typing ***"What is the store hours?"***<span class="copy-static" title="Click to copy!" data-copy-text="What is the store hours?"><span class="copy"></span></span>
    ![Profiles](../graphics/Lab1_AI_Agent/6.1.png) 

8. The initial response can be customized, and we also need to configure intents and responses to enable the Scripted AI Agent to answer questions about store hours.

#### Task 2. Update the initial greeting.  

1. As soon as the interaction reaches the Scripted AI Agent, the system initiates the **Welcome** response. To change the initial greeting, go to **Script** > **Responses** then open the **Welcome** response and update the response text there. Change the text to: ***Hi, my name is Blossom, the virtual assistant. I can help you with tracking your order or providing the store's business hours.***<span class="copy-static" title="Click to copy!" data-copy-text="Hi, my name is Blossom, the virtual assistant. I can help you with tracking your order or providing the store's business hours."><span class="copy"></span></span>. </br>
Please do it for **Web** and Voice **channels**. Aftger the change, Save and Publish the Scripted AI agent. 
    ![Profiles](../graphics/Lab1_AI_Agent/6.3.gif) 

2. Click on the **Preview** button on the top right side to test the bot. Check if the initial greeting was changed. 
    ![Profiles](../graphics/Lab1_AI_Agent/6.4.png) 

#### Task 3. Configure Scripted AI agent to answer questions about store hours. 

1. Before we move on with adjusting and configuring intents and responses, it is important for you to understand the flow of the Scripted AI Agent. Once a customer asks a question, the AI engine and Natural Language Understanding (NLU) service tries to match it to an intent based on the training phrases. The intent is then configured with a response. After the customer receives the response, they can ask another question, and the same process applies. The AI engine and NLU match the customer’s query to an intent, which is configured with a response. Additionally, fulfillment can also be configured as part of the response. This is the basic flow concept of the Scripted AI Agent.
    ![Profiles](../graphics/Lab1_AI_Agent/6.2.jpg) 

2. While on the **Script** configuration page, switch to **Intents** tab and click on the **Create Intent** button located in the top right corner.
3. Add a new intent by providing the intent name as ***store_hours***<span class="copy-static" title="Click to copy!" data-copy-text="store_hours"><span class="copy"></span></span> and include the following two utterances:

    - ***What is the store hours?***<span class="copy-static" title="Click to copy!" data-copy-text="What is the store hours?"><span class="copy"></span></span>
    - ***What is the business hours for this store?***<span class="copy-static" title="Click to copy!" data-copy-text="What is the business hours for this store?"><span class="copy"></span></span>
    ![Profiles](../graphics/Lab1_AI_Agent/6.3.gif) 

4. Click on the **Generate** button to utilize Generative AI for creating additional training phrases.

5. Enter a description such as ***Generate intents store business hours***<span class="copy-static" title="Click to copy!" data-copy-text="Generate intents store business hours"><span class="copy"></span></span> Set the Number of Variants to **10**, which will determine the number of new phrases to be generated.
    ![Profiles](../graphics/Lab1_AI_Agent/6.5.gif) 

6. Now we need to configure a response that would be related to this intent. Scroll down and click on **Create new**.
    ![Profiles](../graphics/Lab1_AI_Agent/6.6.gif) 

7. Name the response as ***store_hours***<span class="copy-static" title="Click to copy!" data-copy-text="store_hours"><span class="copy"></span></span>. Update Varient 1 test to ***The store hours is from 9 am to 5 pm. Please let me know if you have any other questions.***<span class="copy-static" title="Click to copy!" data-copy-text="The store hours is from 9 am to 5 pm. Please let me know if you have any other questions."><span class="copy"></span></span>.
    ![Profiles](../graphics/Lab1_AI_Agent/6.7.gif) 

8. Add one more varient and provide the text: ***The store is open from 9 am to 5 pm. Is there anything else I can do for you?***<span class="copy-static" title="Click to copy!" data-copy-text="The store is open from 9 am to 5 pm. Is there anything else I can do for you?"><span class="copy"></span></span>.
    ![Profiles](../graphics/Lab1_AI_Agent/6.8.gif) 

9. Add **Voice Channel**.
    ![Profiles](../graphics/Lab1_AI_Agent/6.9.gif) 

10. Configure **Voice Channel** with the same varients and click on **Create**. </br>
***The store hours is from 9 am to 5 pm. Please let me know if you have any other questions.***<span class="copy-static" title="Click to copy!" data-copy-text="The store hours is from 9 am to 5 pm. Please let me know if you have any other questions."><span class="copy"></span></span>.</br>
***The store is open from 9 am to 5 pm. Is there anything else I can do for you?***<span class="copy-static" title="Click to copy!" data-copy-text="The store is open from 9 am to 5 pm. Is there anything else I can do for you?"><span class="copy"></span></span>.
    ![Profiles](../graphics/Lab1_AI_Agent/6.10.gif) 

11. Now after we added the response to our intent we can complete the intent configuration. Click on **Add** on the right bottom corner. **Save** and **Publish** the Scripted AI Agent. 
    ![Profiles](../graphics/Lab1_AI_Agent/6.11.gif) 


12. Click on the **Preview** button on the top right side to test the bot. Try the bot flow by typing ***"What is the store hours?"***<span class="copy-static" title="Click to copy!" data-copy-text="What is the store hours?"><span class="copy"></span></span>
    ![Profiles](../graphics/Lab1_AI_Agent/6.12.png) 

<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>

