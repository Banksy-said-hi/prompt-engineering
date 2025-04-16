- **Preference driven refinement**: Within every iteration try to add what you liked & did not like about the answer you were just given

- Exploit the generative nature of LLM s by trying to get multiple answers for the same problem and collect good parts from all 

- Informed Decision Making: support your decision-making process through viewing different perspectvies & approaches, ask the LLM to give you different scenarios and possibilities, clarify what is the cause/root of your projected variation?
  - "Give me three possible emails which totally different tones, and compare and contrast them" 

- For software related solutions, we can ask it to give us multiple solutions and then we can test them and choose the most performant one. Writing effective tests could be leveraged in this scenario. Recognize the objective criteria first!

- You can ask GPT to provide you different analyses on your matter:
  - SWOT: Strenghts, Weaknesses, Opportunities, Threats
  - PESTLE: Political, Economic, Social, Technological, Legal, Environmental
  - SMART: Specific, Measurable, Achievable, Relevant, Time-bound
 
- Breakdown of a great prompt:
  - Intruction: the actual request well explained and clarified
  - Information: providing detailed context and explainig unclear or new parts
  - Patterns/**Examples**: provide something the bot can learn from ( could come from our preferences )
  - Output/Format: providing the wanted structure, it helps guide the thinking of the bot, you can take control of the output format
  - Trigger: You can provide the starting point for the bot, giving some ideas how to start 

- Machine Learning analysis techniques:
  - **Classification**: labeling, putting things into categories, sentimment analysis
      - example: you can copy paste comments of your Linkedinpost and have GPT process and classify them in a table based on their sentiment, summary of comment, and other crucial information which can be tapped into. No need to data cleansing and training model. 
  - Clustering: take our data and try to group it together where common properties can be found, segmenting our market or customers, trying to group them based on attributes, we can identify commonalities 
  - Prediction: Asking the bot predict, here is what you see, based on that, what else can be seen?
  - Recommendation: Based on the available findings, what other possbilities could we have?
  - **In-Context Learning**: AI has the ability to spot the patterns and learn, within the prompt you teach it how to craft the answer, for instance you can provide an exampke and go like "complete the pattern...". come on see if this is the input, this is the output I expect, you can get the AI to fill out the mising info in a dataset, "predict the missing category for this dataset ( probably data drawn from a table )
 
- How many examples are ideal to teach a pattern to an AI?
  - Use lots of examples, as many as you can or AI can accept.
  - More examples, higher accuracy -> more expensive too
  - Providing examples is a tool to get better results from AI
  - You can get the AI to give you some examples, then you choose the good fits and then reiterate over the prompt again

- **Output Formatting**:
  - Placeholder: a place for variables in the response, creating a space to be filled in by AI: "Sina is a <insert adjective> person", if you give a template no instruction is needed, AI realizes itself what needs to be done, we can also specfiy format of the input we expect in placeholder, we can be very specific with the condition inside the < >, you can use a combination of < > to strcuture the response desirably in the needed format.
  - Markdown: cool!
  - Sophisticated Patterns: combining < > placeholders with markdown ( ##Header2, #Header ) to format the response, can result in self-consistency, referencing footnoes can be utilized
    
- Fact-check: always check the response you are given

- Escape Valves: while providing a certain response format, you can use escape valves to tell AI what do to or print when the case it is not applicable/not found/not defined. You are basically telling it do not worry about this now and you can print something as simple as "N/A" instead

- **Retrieval Augmented Generation (RAG)**: What happens if we do not give AI the information it needs to generate our response? How we overcome this problem when enough information is not possessed by the AI to craft our answer? Have AI itself return to the generated response and correct itself via a command in the end that hooks the AI back to the top of response to check something like citations. RAG helps AI go and collect our needed information from external sources.

- Embeddedings: embedding is a wat to convert text into numerical vectors that represents the text in a format that a modl can understand, conversion process, semantics matters.

- Tokenization: breaking down the prompt into its building blocks/words. The purpose of embeddings and tokenization is to find sentences with close meaning. Basically, the meaning of the prompt is represented as a vector to give it dimensions, numerical representation of the text, vectors are a sequence of numbers

- Retrieval with embeddings: 

- Chunks: phrases such as "Potentially Relevant Information" and "Relevant Information" can be used to address the preciseness the provided information for AI.
