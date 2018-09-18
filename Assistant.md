
# Watson Assistant Tutorial: GUI

## Setup

In this method the user uses the Watson service to classify and train the system. The service is really simple to utilize. Even non-programmers can train Watson to detect the objects without coding. The following steps show how to create your own classifier.

1. **Create a Bluemix account.**

IBM Bluemix is a cloud platform with over 150 services, including all of Watson APIs. To get started visit [https://console.bluemix.net/](https://console.bluemix.net/) and create an account.

 ![Bluemix](/VisualRec_Images/ibmbluemix.png)

2. **Create Watson Assistant**

In this part, click on &quot;Create resource&quot; at the top right of the page and choose &quot;Watson&quot; from the left panel beneath &quot;Platform&quot;. Then choose &quot;Watson Assistant&quot; service.

 ![rgfrgfgfdg](/Assistant_Images/1_Create_a_resource.JPG)
![](/Assistant_Images/2_Watson_assistant.JPG)

Next step is to determine the name of the project and create it. Also at the bottom of the page the user can choose the lite (free) or paid account.

 ![](Assistant_Images/2.1_Watson_name.JPG)

In the next page the Watson Assistant service shows you the credentials &quot;apikey&quot; which will be used for programming in a language. These are unnecessary for completing the assignment with the tooling method. Now the user should press the &quot;launch tool&quot; button.

 ![](/Assistant_Images/3_Watson_assistant_credentials.JPG)

In the next page, the user can click &quote&;Workspaces&quote&; and &quote&;create&quote&; to create their unique workspace for their virtual assistant.
![](/Assistant_Images/4_Workspaces.JPG)
![](/Assistant_Images/5_create_workspaces.JPG)

There are three steps to complete to create a virtual assistant. They involve creating intents, entities, and dialogues. In the following example, we are going to create our own intents to toggle a light in a smart home.

## Intents
Intents define the action an assistant is meant to take. For example, you can instruct an assistant to turn an object on or to give the most recent Clemson football scores. In order to create an intent, click the &quote;Add intent&quote; button. 
![](/Assistant_Images/6_intents.JPG)

To define an intent, give it a name beginning with a &pound;. Next, give a few examples of phrases that will be recognized by the intent. For example, you can expect the assistant to recognize &quote;Turn on the lights&quote; and be motivated to turn the lights on. Give at least 5 examples before moving on to the next step.   

![](/Assistant_Images/7_intent_examples.JPG)

## Entities

Entities define the object as user is taking an action on. Entities are generally nouns such as light, chair, or Clemson. Entities are used to refine the action a user is motivated to act upon. For example in the sentence &quote;Turn on the lights&quote; the lights are what a user would like to turn on. Begin to add your own entities by clicking &quote;Add entity&quote;. 
![](/Assistant_Images/8_entities.JPG)

First, give the entity a name beginning with the @ symbol. Then add a value for that entity, and a few synonyms to that value. You can imagine an entity to be the overarching label, and the value to be the object. If you desire, you can have synonyms suggested for you. 
![](/Assistant_Images/9_add_entities.JPG)

## Dialogue
The dialogue is the flow of conversation which ties the intentes and entities together. To begin a new dialogue, click the &quote;Create&quote; button to add a new dialogue flow.
![](/Assistant_Images/10_dialogue.JPG)
There will alwasy be two dialogue nodes when a new dialogue is created the first is the &quote;Welcome&quote; node which is the first message that is displayed when a dialogue is initiated. The second node is the &quote;Anything else&quote; node which generate a response if no nodes are triggered. It is important to know that the assistant will try to trigger nodes from the top node down iteratively. To create a new node, click on the three vertical dots and select &quote;Add node below&quote;. Next, name the node. It is good practice to name the node with the intent or entity the node is being used to match. In the following example, the new node is called &quote;&pound;Turn_on&quote; and will trigger if the assistant recognizes the &pound;Turn on intent. For now, leave the text response blank.
![](/Assistant_Images/11_add_node.JPG)
![](/Assistant_Images/12_add_node.JPG)
![](/Assistant_Images/13_add_entity_to_node.JPG)
![](/Assistant_Images/14example_dialogue.JPG)


