---
#icon: material/folder-open-outline
icon: material/medal
---

# Mission 3: Customize AI Agent Language. 

## Mission overview

In this mission, you will change the language of your AI agent for the voice channel. This feature allows flexibility for supporting customers in different languages.

---

## Build

### Task 1. Configure Global Varialbes in voice flow. 

1. Go to Flows and open up your voice flow **<copy>AutonomousAI_Flow_2000_<w class="attendee"></w></copy>** and click **Create Flow**
   ![Profiles](../graphics/Lab1_AI_Agent/2.76.gif)

2. Edit the flow.
   ![Profiles](../graphics/Lab1_AI_Agent/2.77.gif)

3. Click anywhere on the grey field and then, on the right side, select **Add Global Variables**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.78.gif)

4. Add Global Variables with name: **Global_VoiceName** and **Global_Language**. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.79.gif)

5. Review documentation with available languages and voices. <br/>
[Supported-languages-and-voices-for-AI-agents](https://help.webex.com/en-us/article/pdef2d/Supported-languages-and-voices-for-AI-agents){:target="_blank"}

6. Add **SetVariable** node. Select Variable as **Global_Language** and put the value of the language that you want to test. For example, to set up the AI agent to speak Spanish, you can enter **<copy>es-US</copy>**. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.80.gif)

7. Add one more **SetVariable** node. Select Variable as **Global_VoiceName**. Select the appropriate voice from the documentation. For example **<copy>es-US-Alonso</copy>**
   ![Profiles](../graphics/Lab1_AI_Agent/2.81.gif)

8. Connect the nodes in series. Validate and Publish the flow. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.82.gif)

9. Call the number that is related to your channel. You should hear the AI agent speaking still play the Welcom message in English but after you can continue the conversation in Spanish.



