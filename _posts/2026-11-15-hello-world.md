---
title: "Hello, world"
description: "First post. What this blog is for, and a quick test of how things render."
tags: [meta]
---

I build agents for a living, so this is where I'll write down what I learn doing it: agentic workflows, RAG, evals, guardrails, and the back-end plumbing that keeps all of it running.

> This post doubles as a formatting reference. Edit it into your real first post, or delete it.

## Code

Fenced code blocks get syntax highlighting and a language label:

```python
from langgraph.graph import StateGraph, END

graph = StateGraph(dict)
graph.add_node("review", review_case)
graph.add_conditional_edges("review", route, {"abstain": "human", "done": END})
```

```java
@Path("/rfp")
public class RfpResource {
    @POST
    public Response create(RfpRequest req) {
        queue.send(req);   // async, picked up by an SQS consumer
        return Response.accepted().build();
    }
}
```

Inline code looks like `this`.

## Tables

| approach | latency | quality |
|----------|---------|---------|
| plain retrieval | low | ok |
| retrieval + rerank | medium | better |

### Images

Put images in `assets/img/` and reference them like `![alt text](/assets/img/diagram.png)`.
