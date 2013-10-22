---
layout: post
category : introduction
title: "Through the pipeline"
tagline: "<br />Experimenting with alternative concurrency models"
tags : [sumary]
---
{% include JB/setup %}


## Inroduction


Hello everybody,

Here, I&rsquo;ll post some thoughts about what I have been researching in my academic life and some random stuff in my head. I&rsquo;ll try to be clear in the development of my ideas. Also, you may find some grammar errors since english is not my native language, so please be patient with me.

Throughout my posts, I&rsquo;ll talk about concurrence and parallelism.
Concurrence is a property that occurs when more than one process run simultaneously, potentially interacting with each other and competing for resources.
Parallelism is a property of systems that can execute more than one process *at the same time*. 

In my thesis, I discussed about the staged event-driven concurrency model and how it can be tweaked to decouple decisions about the logic of your applications from decisions about the execution environment.

[Leda](http://leda.co) was implemented as a result of my research, and, in this blog, I&rsquo;ll cover some aspects of its architecture and execution dynamics.


### Possible future posts

1. **Leda overview and examples**

   A post with a little tutorial about the features of Leda in some use cases.

   Stages, instances, states, processing latency, asynchronous execution, cooperative task manager.

   Communication, output ports, event type, event queues, communication latency, communication throughput.

   Agglomeration, communication patterns, processing latency, and resource sharing.

   Mapping, separate local resources in the localhost, running on the Amazon EC2.


1. **Asynchronous execution and the power of pipelines**

   Multicore/many core  architectures, accelerators, NUMA, and networked environments. Heterogeneous environments.

   Application graph, Local communication, remote communication.

   Asynchronous execution, context switching, stack ripping, cohort execution.
   
   C interface, Lua bytecode, JIT runtime, FFI interface.


1. **Managing states to avoid the thread hell**
      
   Ready (blocking) queue, thread pool, process controller, scheduler API, types of controllers, customizing controllers 

1. **Comunication issues**

   Lock free queues, Rings, cache issues, references (single reference/multiple readers multiple writers/immultable references), resource sharing (device, file and socket descriptors, memory references, data serialization, copy on write), events, 

1. **Future considerations**

   Things to improve or rethink and possible future research topics.

I hope I see you in the future!

Tiago Salmito
