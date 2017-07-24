## After defining intense and entities as a chatbot creator you would typically focus on designing the dialogue

## Creating a dialogue defines how your bot will respond to what the user is asking
## Dialogues in Watson conversation are defined visually through a user interface their structure around the concept and nodes
## Each node has a name condition and one or more responses

### There are a few more bells and whistles available, but if its core
### We're talking about name condition and responses the dialogue starts executing from the first node at the top if the condition is met
### it will reply to a user with a response specified in that node and stop the

Execution until the user has entered some new input if the condition is not met
It will skip the response and proceed to consider the next node below if this second knows condition is met by the users input
The nodes response will be sent to the user if the condition is not met. We continue to the next node and so on
essentially the execution from top to bottom
Continues while the node conditions fail to me what the user inputs are centered for the condition
You can use intense entities a specific entity value
And if you reserve conditions like welcome anything else true and false
You can also combine intents and entities with Endon or logical combinations?
Typically you'd want to greet the user as they arrived so the first node may use a special word
Welcome at the condition
Ensuring that the particular node is executed the first time that the user starts
Interacting with the chatbot the response we configure in that particular node will be our initial prompt a grid see user
Inviting them to chat with our chat
Bot if the user input doesn't match any of the known
Conditions by default no response will be provided to the user and this isn't great from a user
Experience Standpoint because nobody likes to be ignored
So it's a good idea to have also a node at the very bottom of the dialog
There is always executed if the user input failed
Satisfy the conditions of any of the other nodes involved the failover condition for this node is called any thing underscore elves
When will this note be executed in?
Practice when our bot has failed to understand the user so in this node
we should have an appropriate response that invites the user to rephrase or
Maybe suggest some queries that we know our bot can handle if we only included a single response in this node
The ball could get annoying rather quickly
Imagine seeing I don't understand over and over again
Hopefully our user one triggered a anything else no too often but it would be good to have multiple responses
With some variation to them unis they always press the same concept it's a small detail that can affect the user experience
And now intelligent our chat what appears to be these responses are executed sequentially by default so the first time the user
Asks for something that our chat, bot doesn't understand our
Anything else node will be hit
And it will show the first response to the user when this happens again
Because the user enters something else that we don't understand the second response will be shown instead
And so on it's also possible to set the order as random by clicking the set to random link
Under the responses block these two nodes endow such common scenarios that they appear by default when you create a new dialogue
That's quite
Enemy since you all you have to do is then customize them with what you want in a prompt?
And what kind of I don't understand responses you want to include and send to the user
It's also possible to create children nodes these are considered for execution only when the parent nodes condition is met first
normally the flow of
Execution for a particular user input is stopped once the condition is met by one node
With them better responds with from our input, and then we start a cycle
Evaluating this new input against the conditions in our nodes top to bottom however if the matching node has children nodes
The execution continues with its children not with the main nodes if a parent node has multiple children
They're considered top to bottom it turns out
This is quite useful in practice in fact it's common to have a parent node ask for further
Clarification to the user in its response and then in specific information provided by the user in its children notes
For example the parent node might be triggered by the user asking I'd like flower suggestions for a special occasion
It doesn't provide information about which specific occasion
so the response from the node may be which occasion when the user replies with say
Birthday the child know the matches the birthday condition will be executed and into response
Displayed to the user for this to work
we'll need multiple children nodes each having as its condition in Occasion value like
anniversary Funeral ETc each having an appropriate response
Alternatively we can take advantage of the factor responses themselves can have conditions attached
I know that can have multiple responses that are only processed if their own condition is met
So instead of having multiple children nodes one for each occasion
We could have a single node that provides different responses
Depending on which Occasion value is provided in response to our request for clarification
Children nodes can have a children nodes of their own giving us the ability to create a quite complex dialogue flow
Furthermore we have the ability to jump from one node to another something that can complicate our dialogue flow
But which will be necessary at times
In order to accomplish what the chopper needs to do don't worry if this is a bit overwhelming?
We covered a lot of ground to give you a theoretical foundation
When we create our chat bot in the next module for become much more familiar with how we use parent children nodes
conditions and responses in order to Define a
convincing conversation flow for our chat bot
