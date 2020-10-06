# Information-in-Language
This is a fun little experiment where we are trying to understand the information carried in sentences! We attempt to measure the information content and vagueness of true/false statements in language by modeling them with a minimum complexity neural net. For more information, see the tutorial in 'Perceptron Networks' where the process of modeling and finding the complexity of the addition of two integers is explained.

The sigmoid function classifer used in the neural nets is a fundamental result from the most basic systems studied in statistical mechanics, and neural nets can theoretically model any continuous function. As a result, we believe neural networks can be used to define a new fundamental unit of information in the context of statements and language. In addition, by examining the the accuracy of the network with different complexities, we can begin to quantify vagueness in language and perhaps even search for more efficient representations of language!

We also strive to link together multiple statements to understand how much extra complexity is necessary to model a statememnt after verification of a previous statement vs allowing that statement to stand alone or training a single neural net to model both statememnts simultaneously. For example, we can start by finding out how much complexity is required to model the addition of two integers between -50 and 50: `a + b == c`. Then, we can model the statememnt `a == c` given that the previous statement is true. We can compare this complexity to that which is required to model `a == c` without the previous statement and the complexity of modeling the logical combination of both statements, `a + b == c and a == c` or `a + b == c or a == c` .  

Our initial toy models come from mathematics. We chose these statements since they are precise and we can easily generate training and validation datasets for them. We are starting with some proof of concept models using perceptron neural networks but will migrate to recurrent architecture to better represent statements that may not have a pre-determined length.

This project could help us understand the most efficient underlying structures for neural representations of language and compare them to the way our brain is structured. It could also elucidate how growing up around different languages might change the way a person assigns meaning to phrases and perhaps even help pave the way for scientists to use different languages and invent their own languages as general and evolving tools to represent different types of information. A very long term goal would be for people to have the ability to not only change what the say when they are trying to communicate something, but also change the language representation they are using based on the context in which they are communicating.  

This paper provides a theoretical basis for the information complexity of neural networks - http://math.bu.edu/people/mkon/nn30.pdf

We will be building on the work on neural complexity from this paper - https://people.cs.umass.edu/~binds/papers/1997_Siegelmann_JNeurocomp.pdf
