# caesar225-langsmith-MAT496
In module 1 video 1, I learnt about the concept of tracing. It is the process of tracking the flow of requests across different services. I also added a few of my own questions in the code.

In module 1 video 2, I learnt about runs, their types and tool calling. Runs are a single execution unit traced by Langsmith. Runs are helpful in debugging as we can trace the intermediate steps and see where we went wrong. Tools are used when the LLM can't answer something by itself. LangSmith will trace each tool call as a separate Tool run.

In module 1 video 3, I learnt about the alternative ways to trace, as decorators trace only one function call at a time, and don't capture the entire flow. Context manager gives more control over what exactly is traced and when. It is useful if you want tmultiple related calls or longer workflows as a single run. API Calls explicitly create and log runs via SDK or API calls. They allow linking multiple runs, or integrating with external systems.



