# caesar225-langsmith-MAT496
In module 1 video 1, I learnt about the concept of tracing. It is the process of tracking the flow of requests across different services. I also added a few of my own questions in the code.

In module 1 video 2, I learnt about runs, their types and tool calling. Runs are a single execution unit traced by Langsmith. Runs are helpful in debugging as we can trace the intermediate steps and see where we went wrong. Tools are used when the LLM can't answer something by itself. LangSmith will trace each tool call as a separate Tool run. Once again, I added a few of my own questions.

In module 1 video 3, I learnt about the alternative ways to trace, as decorators trace only one function call at a time, and don't capture the entire flow. Context manager gives more control over what exactly is traced and when. It is useful if you want multiple related calls or longer workflows as a single run. API Calls explicitly create and log runs via SDK or API calls. They allow linking multiple runs, or integrating with external systems. I tweaked the code by adding some questions which would not be given in the context.

In module 1 video 4, I learnt about conversational threads. It is how we can continue a conversation with an LLM about a topic with a sequence of related messages. It's like a mini conversation within the overall dialogue. Threads are useful so the LLM application doesn't mix up answers. I tested the limits of its contents.

In module 2 video 1, I learnt about datasets. They are useful as a form of evaluation, so that we can make sure that our changes make our application better. Fundamentally, they are a list of examples. We can add examples manually as well. Examples contain an input and an output, similar to a RAG application. I have tweaked all the examples. 

In module 2 video 2, I learnt about evaluators. They evaluate empirically whether the changes we made actually improved the application or not. They operate on examples from our dataset and run our application over those examples. We can attach multiple evaluators so that we can calculate many different metrics such as accuracy and hallucination. What they do is, they compare the dataset example(the golden example) against the example run from our app. I have compared questions from my dataset and the ones not from my dataset as well.

In module 2 video 3, I learnt about experiments. An experiment can be defined as running our application over a dataset, and then evaluating performance using evaluators. Experiments in Langsmith let us run, monitor, and compare different model runs or configurations. I have used my own dataset. 

In module 2 video 4, I learnt how to analyse the results of my experiment. <img width="1282" height="459" alt="Screenshot 2025-10-04 234041" src="https://github.com/user-attachments/assets/3a67e37e-da1f-4de2-ba74-6e43185b9702" />

In module 3 video 1, I learnt about the playground environment in Langsmith and how it's useful for prompt engineering. We will be dealing with prompt templates, which have template variables which are filled by the user at runtime. They give the user more flexibility as now we can enter different inputs and test them. I changed the dataset used and filled it with my own variables.

In module 3 video 2, I learnt about the prompt hub. Here, we can store prompt templates and reuse them across different applications. It also allows us to save different versions of the same prompt. I created different versions of my own prompt and saw the LLM answer in the language of my choosing.

In module 3 video 3, I learnt how to take what I learnt about the playground and prompt hub and how to iterate on a prompt using them. I created my own updated dataset.I also used Groq instead of ChatGPT and HuggingFace embeddings instead of OpenAI embeddings.

In module 3 video 4, I learnt about prompt canvas, which uses an LLM agent to help us improve our prompts. We can find this inside the playground interface in Langsmith. We can use this to standardize prompts across our organization.
