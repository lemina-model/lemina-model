# **Hello, Lemina\!**

© Copyright 2024 Rex Young. All Rights Reserved.

![contact](lemina-contact.jpg)

Part 1 — Programming's Evolving Path

Part 2 — Lemina Programming Model

Part 3 — Lemina Programming Model For Business Applications

Part 4 — Lemina Business Application Development

# **Part 1 — Programming's Evolving Path**

Computer programming is a fascinating technique deeply ingrained in the CPU's operation. It shares common developmental threads with machine-operating techniques like car driving. Both programming and driving have evolved along a similar path to achieve operational efficiency on parallel development tracks. This human-centered evolution of programming, a journey we can all relate to, is at the heart of our discussion.

At the dawn of every newly invented machine, users had to adapt to its limitations. The first modern car, the Benz Patent-Motorwagen No. 1, built in 1885 by Karl Benz, forced people to use a centered steering crank instead of a steering wheel and a left-handed gas-and-brake handle instead of pedals to drive.

Over time, a wave of human-centered features emerged in car driving to align the car's operations with our natural reactions. For instance, General Motors introduced an automatic transmission in its Oldsmobiles in 1924, and Chrysler pioneered power steering in 1951\.

These features changed how cars operate, catering to drivers' desires for more intuitive and relatable driving machines. Other human-centered additions included cruise control, which allows the driver to set a constant speed without keeping their foot on the gas pedal, and anti-lock braking systems, which prevent the wheels from locking up during braking, improving the driver's control over the car through critical moments.

Today, car driving is approaching the end of its evolution. With merely an address, self-driving cars can take their passengers to their destination without further human input.

As early automobiles began with simple mechanics, early programming began with machine code. Each machine code represents a CPU operation, which could be one of the following:

* Arithmetic operations (such as additions, subtractions, multiplications, and divisions) of two words (such as numbers within limited ranges)  
* Bitwise operations on one or two words  
* Jumping to another address in the memory and executing stored machine code from there  
* Comparing two words and conditionally jumping based on the comparison result

A word is the size of CPU registers and memory units. The Intel CPU 8088 used by the first IBM personal computer released in 1981 was 8 bits, which could hold a number ranging from 0 to 255 (or from \-128 to 127 with a sign). If a number larger than 255 was needed in a program, the programmer had to write more machine code to use multiple words to achieve it. Unfortunately, programmers could not easily enlarge the word size for the CPUs of the time because physical circuits had to be laid on the chip to support every bit of the CPU's combined internal registers and memory units. Longer words required more circuits on the chip. As a result, personal computers have been equipped with 64-bit CPUs since 2000, such as the Intel Pentium 4 processor and the present-day version, the Intel i9.

Most non-IT people who observe modern computing devices, such as smartphones, gaming devices, Internet applications, cloud computing infrastructures, and now AI-enabled programs, cannot believe that CPUs are this raw on a fundamental programming level. The unpleasantness of working with "dumb" machine code drove programmers to innovate waves of new human-centered features in modern programming.

The first wave introduced high-level programming languages, such as FORTRAN (invented by IBM in 1957 as the first high-level language), COBOL, and BASIC. These languages allowed programmers to use user-friendly elements like English keywords, data types, variables, arithmetic expressions, and procedures (or functions).

A program written in a high-level programming language cannot be understood and executed directly by the CPU, so it has to be translated into machine code. Thus, a high-level programming language is always equipped with a before-time compiler (which translates the entire program into machine code before execution) or a real-time interpreter (which translates the program line-by-line on the fly during execution) for the machine code translation.

This innovation led to two key benefits that would shape the future of programming. First, the compiler automated repetitive work for programmers, leading to a significant leap in efficiency. Before this innovation, programmers had to write extra machine code to utilize a number exceeding the size that the CPU could handle. With the new high-level languages, the compiler's job was to support new data types and variables, leaving human coders with extra time for more demanding tasks. The second key benefit was that these procedures allowed programmers to group repeated and relevant parts of code for reuse, removing redundant coding labor from the process and further enhancing the workflows of human programmers.

The second wave introduced object-oriented programming (OOP, backed by the object model), a term coined by Alan Kay in 1967\. An object is a programming element that encapsulates relevant and private state (data) and behavior (code) to which no outside access is allowed. Other objects or non-object codes can only operate the object through its predefined interfaces or "methods," which are procedures or functions owned and encapsulated by objects. OOP programming languages are also considered high-level and equipped with compilers or interpreters. Eventually, OOP programs were translated into machine code, allowing a range of users that was impossible before this innovative new process.

The innovations brought by the first two waves have fundamentally improved programming. Most of today's programming languages are high-level and object-based (object-based is more broad than object-oriented). Unlike high-level languages, which automate repeated work for programmers, objects address increasing code complexity by introducing a new building block for constructing programs. Objects profoundly impact programming because this building block is like a new "life element" in programs. It's as functionally significant to programmers as the first appearance of the division or specialization of labor in Adam Smith's The Wealth of Nations was for economists and business managers.

The emergence of the object concept and model has allowed programmers to evolve from designing each step of a computational task (e.g., high-level codes or low-level CPU operations) to organizing a group of specialized objects that contain relevant data and behaviors. Thus, programming itself has evolved into a new twofold technique: programmers design detailed steps to form specialized objects and then organize them to create programs.

People who pay attention to lists of most popular programming languages every year know that OOP will still be mainstream in 2024\. Does this mean programming has stopped evolving for the last 60 years since the late 1960s? Surprisingly, we have not made any meaningful breakthroughs in general-purpose programming since the OO revolution.

Despite this, the IT industry has not been hibernated for 60 years. Instead, it has expanded its territory into every corner of people's lives, shaping our daily experiences and interactions. It's new battles take place over these places:

* Participation in programming and computing has expanded from a niche population in academia, research, and scientific communities to a giant IT industry.  
* Computers have expanded from mainframes to personal computers, handheld devices (e.g., POS scanners), smartphones, and anything with a CPU that can run programs.  
* Programming and computing environments have expanded from processors with a single CPU to multi-CPU (aka multi-core) processors, networked computers (e.g., programs running on a company's network or cloud), and the Internet, which connects everything (with a CPU) and everyone (via a device and a program) 24/7.

This shift implies several things. First, there were two eras—the former focused on invention and the latter on applying programming techniques in broader domains. Secondly, the meaning of programming has changed from programming a simple computer to programming many multi-core and networked computers (essentially, "programming the Internet").

Let us use automobiles as an analogy once more. The programming industry has gone from inventing the car to seeing what a single car can do for people. Now, it controls the actions of multiple vehicles from a coordinated business objective.

Therefore, we need to reevaluate the evolving path of programming and recalibrate its direction by examining two fronts: whether OOP is sufficient for programming the Internet and what (other than OOP) has kept us moving forward to more complex, efficient applications.

Programming the Internet requires techniques for concurrent and distributed programming. Although modern OOP languages have added more user-friendly features to support multi-threading, the object model behind OOP lacks a mechanism for concurrency. Efforts were made in the past, such as Carl Hewitt's Actor model in 1973 and Greg Lavender and Douglas Schmidt's Active object pattern in 1996, but mainstream programmers have yet to accept them.

The object model also lacks a mechanism for distributed programming. Similarly, efforts such as the Common Object Request Broker Architecture (CORBA), Distributed Component Object Model (DCOM), and Java Remote Method Invocation (RMI) were made but have yet to be widely utilized. As a result, hardware and software architectures, frameworks, and patterns—such as middleware and microservices with RESTful APIs as interfaces—have kept us moving forward with programming the Internet.

Based on these observations about the potential bottlenecks in programming the Internet in 2024 and beyond, it's clear that we need a unified programming model that can handle concurrency, intra-process programming (e.g., at the level of programming language), and inter-process programming (e.g., at the level of many programs running on many computers). The model should be human-centered, meaning intuitive and instinctive to people. We already have the steering crank; the goal is to invent the steering wheel.

# **Part 2 — Lemina Programming Model**

In Part 1, we discussed the status of programming and where it is going now. This knowledge helps us determine whether a new programming technique is on the evolutionary path and assists us in designing new ones. When creating a unified programming model, I analyzed the essential behaviors and mechanisms behind the current programming techniques and compared them to how people interact to perform social and business functions. Then, I borrowed models and concepts in human social behavior to create a programming model reflecting these principles. The result was the Lemina programming model.

In a fundamental sense, a CPU executes a program by executing one statement (or line of code) at a time. To illustrate the program's execution to non-IT people, we can use the train, track, and sleeper analogy. A train represents a CPU, a track represents a program, and a sleeper represents machine code or a line of code. A train running through sleepers under the track represents a CPU executing code in the program.

In the early days of programming, even in the late 1940s, a computer might not support the concept of subroutine or procedure. For example, Manchester Baby (the first electronic stored-program computer built at the University of Manchester in 1948\) only supported eight instructions, not including one that calls a subroutine. These rudimentary programs can be viewed as one-dimensional (1D) in structure because all their code in a program lays linearly as a one-dimensional line, as all sleepers are under the main track.

Programs using procedures can be viewed as two-dimensional (2D) since each has a track parallel to the main track, lying in a two-dimensional area. The train runs down the main track, teleports to the procedure's track, and continues to run when it encounters a call procedure sleeper on the main track. The train then stores the position next to the call procedure sleeper on the main track to the stack so that it can teleport to where it left off when it finishes the procedure's track. We use "teleport" to describe the move when a CPU "jumps" instantly to the beginning address of another track, though there's no analogous function in an actual train.

Now, let us add objects to the picture. An object in the program can be viewed as several tracks (the methods owned by the object), with private data enclosed by a fence. However, programs with objects are still 2D programs.

Multi-core CPUs bring multiple trains to execute the same program simultaneously, a requirement for most modern programs. Having a train for each procedure track expedites lengthy calculations since having more hands on deck will speed up the entire program. Another typical example of needing multi-core CPUs is when programs run as servers that support many simultaneous clients.

Having multiple trains in a program adds a new dimension. We can view programs with multi-threading at runtime as "3D programs." However, this also leads to new programming challenges. When one train does everything, the train knows and has all the information. But how do multiple trains interact when they perform functions simultaneously? Should the main train wait or continue while the procedure train is running? If the main train doesn't wait and the procedure train has new results to report, how can it receive them mid-process?

In programming, these interactions are called synchronous and asynchronous procedure invocations. On the one hand, a caller can obtain a callee's results for sync invocation because it waits on the spot. However, for async invocation, the caller immediately moves forward. Thus, it's difficult for the caller to obtain the callee's results because there should be a new arrangement in another time and space for the results to change hands. Popular solutions for getting async results include Future, Promise, and Callback with Closure. These solutions work as expected, but their styles are more tech-oriented and less intuitive than many modern programmers would prefer.

In Part 1, we considered objects a new life element in the programming world. Objects have addressed the structural aspect of the issues caused by code complexity but have yet to address the behavior aspect of the problems caused by concurrence (on the same or different computers). In other words, objects are revolutionary but still half-baked, requiring improvements to behave more like independent life elements in the modern programming world.

The analyses boil down to one direction for solutions: a unified, human-centered design for handling sync and async procedure invocations in and across programs (and computers).

I started to find this direction by examining the similarities between 3D programs and human societies. People live on the earth's surface, which can be viewed as a 2D space. Within that space, everyone carries out their own decisions and actions with their bodies, which can be viewed as the third dimension, the dimension of thinking and action. Thus, both programs and societies similarly define the 3D context. Recognizing this, I examined how people interact in societies to perform social and business activities. I became convinced that the real-world postal service model can be an infrastructure for 3D programs in a new unified programming model.

Thus, I borrowed models and concepts from real-world postal services to create the new lemina programming model, which introduces two programming elements: lemina (postal) services and leminas. Real-world postal services send mail to registered recipients on behalf of anonymous senders. Lemina services behave similarly by delivering messages to registered recipients on an anonymous senders' behalf, where senders could be any code, including leminas.

I intentionally chose lemina, a personified name, over a traditional name in programming, like an object or actor, for several reasons:

* To pay tribute to real-world models and concepts  
* To indicate that the lemina model is a human-centered design  
* To emphasize that leminas are not objects or actors but could be implemented by objects, actors, or even procedures as long as they comply with the lemina model.

The lemina model aims to replace procedure invocation with message passing. Procedure invocation is deeply rooted in the mindset that one thread of execution (e.g., a train) performs actions on both the caller and callee sides, while the mentality of message passing is between two independent entities (e.g., humans or programming elements). Procedure in this context also means functions, methods, subprograms, subroutines, etc. These terms are interchangeable in this discussion.

Procedure invocation is a low-level, techy mechanism of how the CPU works. We cannot replace them with the lemina model, which is a higher abstraction. "Replacing" means that the procedure invocation overreached unsuitable places in programming. Therefore, we replace it in these situations with the lemina model.

The procedure invocation works this way: caller → procedure. The lemina model inserts a middleman between the caller and procedure: caller → outbox → lemina service → inbox → lemina, where lemina represents a procedure.

The lemina model requires a lemina service to provide a public outbox for every user and a private inbox for each lemina, as the outbox and inbox are part of the lemina service. The outbox and inbox are named after the sender's and lemina's perspectives, respectively. Thus, the original procedure invocation is replaced by two separate invocations: one between the caller and the lemina service (via outbox) and the other between the lemina service and lemina (via inbox).

For programming the Internet, the lemina model works through networked lemina services: caller → outbox → source lemina service → {networked lemina services} → target lemina service → inbox → lemina. Thus, the caller, lemina, and the programming style remain unchanged among different configurations of lemina services.

In summary, the invocation model (which is supported by high-level, object-oriented languages for intra-process programming):

* Caller → procedure

Is successfully converted to the lemina model (for intra-process and inter-process programming):

* Caller → outbox → {lemina service(s)} → inbox → lemina

It can be further abstracted as a one-way message-passing model where one message passing between the sender and lemina comprises two invocations: one is between the caller and outbox, and the other is between the inbox and lemina:

* Sender → {lemina service(s)} → lemina

The lemina model utilizes four foundational mechanisms to achieve the design goals mentioned above:

* Textual ID  
* Reply-to  
* Localization  
* Namespace

## **Textual ID**

In the real world, recipients registered with postal services use their addresses for delivery in the place of their real names. Addresses are associated with houses (more precisely, the lots on which homes are built), so addresses are deliverable where names are not.

In contrast, no difference exists between names and addresses in the digital world. Thus, lemina ID, name, and address are interchangeable terms in the lemina model.

The lemina model defines lemina IDs as textual. Textual ID is the cornerstone of the lemina model, enabling or improving several key factors:

* referenceability  
* reachability  
* human-style reply-to mechanism

**Referenceability** enables all people, not limited to those with IT knowledge, to use lemina names directly in their thought processes. People can talk about lemina names, pass through lemina names to others via phone, design business processes with lemina names, etc.

**Reachability** enables successful message delivery to leminas, whether in the same program or over the Internet. Notably, messages should also be textual to be delivered across different programming languages, computers, networks, etc. Textual content is not a technical requirement for cross-internet delivery but is compatible with all existing protocols and infrastructures.

**The human-style reply-to mechanism** is for async messages (e.g., two-way messages that return results). People perform async interactions by asking someone to do work and leaving a reply-to address for the person to return the results. Textual ID ensures the reachability of the reply-to messages.

A lemina could represent or be implemented by a procedure, multiple procedures, an object with methods, or even multiple objects. In the case of representing multiple entities, further internal addressing is needed to target a particular entity. The lemina model further defines an **attention name mechanism** for lemina internal addressing, inspired by real-world addressing on an envelope with attention. The attention names are separated from the lemina name by a pound sign "\#," for example, "Alice\#place-order," "Alice\#cancel-order," and "shipping-team\#ship-order." On that note, lemina names should be case-insensitive to avoid being prone to human usage errors.

## **Reply-to**

The lemina model's core function is one-way message passing. A sender can send a message by name using outbox. The syntax below is for illustration purposes, as outbox details will be implementation-dependent:

* outbox.send("Alice\#place-order", \<message\>)

Notably, outbox messages are one-way. From the sender's point of view, they act in the send-and-forget style.

Our early analysis concluded that performing async invocation is easy while getting results is difficult. The lemina model introduces the reply-to mechanism to replace current technical solutions such as Future, Promise, and Callback with Closure.

The reply-to mechanism adds a reply-to address to the outgoing message so that the lemina (or its parent lemina service) wraps its results in a new message sent to the reply-to address.

* outbox.send("send-to: Alice\#place-order", "reply-to: shipping-team\#ship-order", \<message\>)

Remember that lemina ID, lemina name, and lemina address are interchangeable terms that refer to the same thing. Therefore, users should treat the send-to and reply-to labels above as comments that are not part of the definition of the lemina model.

This way, the 'shipping-team' lemina will receive the results at the attention 'ship-order.' But what if a programmer has legacy code or wants to obtain the results in place? Put another way, how can you serve a sync message on a lemina?

The lemina model doesn't support any sync function at its core, so the burden is placed on the shoulder of the outbox by design. The outbox will take a sync invocation like this:

* \<results\> outbox.await("Alice\#place-order", \<message\>)

The outbox's implementation can achieve the await() by using two one-way messages. For example, an outbox receiving an await() call can internally create a new lemina, register it with its parent lemina service, add the new lemina name to the message, and eventually convert it to a reply-to message. When the new lemina receives a return message, the outbox then passes the results in the return message back to the waiting caller.

## **Localization**

The lemina model's core component is the lemina service: caller → outbox → lemina service → inbox → lemina. Implementing the lemina service also covers the outbox and inbox because they are part of the lemina service as defined by the lemina model.

Modern programmers have hundreds of languages available, each of which may implement the lemina service. Additionally, programmers may have different designs within the same language. Since the total number of implementations is nearly limitless, the lemina model cannot provide a one-size-fits-all design or definition for every possibility. Here is where the locality comes in.

Locality refers to the principle that programmers can implement lemina services however they prefer, provided the results are within the lemina model's core principle. This principle can be summarized: if a caller has a lemina name and access to an outbox, then the caller can send the lemina a one-way message. Of course, the compatibility of individual messages can lead to new challenges. Let us use a real-world example. You can write someone a letter in English if you know the person's address, but the recipient may only understand French. That won't be the postal service's fault since the sender should know the recipient. The same is true for lemina.

For example, let us explore two different designs for implementing a lemina service using the same programming language, Java, to illustrate how locality helps everyone participate in the lemina world to solve existing and emergent programming challenges.

There is a legacy class, 'Sales,' with methods like 'placeOrder,' 'cancelOrder,' etc.

Let us take the example of designing two lemina services in Java, one for sync invocation and the other for async invocation, to illustrate these methods.

The former will demonstrate that the lemina model can maintain the legacy program in the same style; the latter will prove that the lemina model can convert legacy code to concurrency.

**Design for sync invocation**

The lemina service offers an outbox as usual but doesn't provide inboxes for leminas because the lemina service and leminas work privately and locally. The lemina service internally uses a map to store all mappings between lemina names and Java object instances (namely, leminas).

Legacy code:

* sales.placeOrder(\<parameters\>)

Converted lemina style for sync invocations:

* outbox.call("sales\#placeOrder", \<parameters\>)

After receiving this call via the outbox, the lemina service lets the caller's thread continue executing the following internal logic:

* Retrieve the sales instance from the mapping by the name "sales."  
* Retrieve the method instance on the sales instance using the Java reflection feature based on the attention "placeOrder" as the method name.  
* Invoke the method sales.placeOrder(\<parameters\>) with parameters.

Thus, the caller's thread executes all implementation logic, and the overall invocation remains synchronous.

**Design for async invocation**

The lemina service offers an outbox for the public and a private inbox for each lemina. A lemina's mapping will include the lemina name, inbox, and a Java object instance.

Legacy code:

* sales.placeOrder(\<parameters\>)

Converted lemina style for async invocations (minus the results to make the example simpler):

* outbox.call("sales\#placeOrder", \<parameters\>)

In this implementation, the caller's thread retrieves the mapping by the lemina name, puts parameters in the inbox, and returns immediately, allowing the caller to complete an async invocation.

Notably, the lemina service uses a thread from its internal thread pool and loops the inbox for this lemina. For every loop, the service thread retrieves a set of parameters in the order of their arrivals and executes the Java object sales.placeOrder(\<parameters\>) until the inbox is empty.

**Design for a combination of both sync and async**

We can further merge two implementations into one by localizing the method names of the outbox:

* outbox.syncCall("sales\#placeOrder", \<parameters\>)  
* outbox.asyncCall("sales\#placeOrder", \<parameters\>)

## **Namespace**

A lemina service can work alone, and it can also work with other lemina services through a connection called networked lemina services. The lemina model doesn't define any network topology or structure for networked lemina services because the model doesn't want to promote a one-size-fits-all design. However, networked lemina services create a potential challenge when a caller wants to call or message a lemina with the same name as other leminas registered with different lemina services.

Therefore, the lemina model defines a concept of "namespace" to address these duplicate name issues. A namespace is a scope:

* Consisting of one or more networked lemina services  
* In which a specific lemina name structure or pattern is used  
* Where all lemina names have the same reachability through any lemina service in the scope

**Example 1**: One namespace for a single lemina service that contains the names 'Alice' and 'Bob.'

A caller can reach all names registered with the lemina service:

* outbox.send("Alice", \<message\>)  
* outbox.send("Bob", \<message\>)

**Example 2**: Three namespaces for the networked lemina services' s1' and 's2' where s1 contains 'Alice' and 'Bob' and s2 contains 'Charlie' and 'David.'

In this example, there are three namespaces:

* namespace s1 contains lemina service s1 and leminas Alice and Bob  
* namespace s2 contains lemina service s2 and leminas Charlie and David  
* namespace s1s2 contains lemina service s1 and s2 and leminas Alice, Bob, Charlie, and David

The lemina service s1 understands namespace s1 and s1s2 but needs help understanding namespace s2.

* s1.outbox.send("Alice", \<message\>) → it works  
* s1.outbox.send("Bob", \<message\>) → it works  
* s1.outbox.send("Charlie", \<message\>) → it doesn't work  
* s1.outbox.send("s2/David", \<message\>) → it works

The lemina service s1 is part of namespace s1s2, so it understands the name pattern 's2/David.'

**Example 3**: One namespace for the networked lemina services' s1' and 's2' where s1 contains names 'Alice' and 'Bob' and s2 contains names 'Charlie' and 'David.' Unlike in Example 2, lemina services s1 and s2 decide to share a single namespace, which means they will share names and ensure no duplicate names when registering a new lemina on either side.

In this example, a caller can reach all leminas by their native lemina names via either lemina service s1 or s2. There is no name pattern, as there is only one layer between lemina services and leminas.

**Example 4**: A global namespace

Everyone is familiar with the Internet, but only some people understand it from a network perspective. The same network protocols that create the Internet could be used to power more Internet instances. Other Internet instances utilize the same network protocols on a small scale, often designed for specific organizations, such as a business's employee intranet.

Similarly, we can use these network protocols and technologies to build a global instance of the lemina namespace where everyone can participate. The advantage of this approach is that we don't have to start from the ground up. We can use domain names as the top layer in the lemina name structure. For example, Amazon may publish a lemina name for the public to use:

* lemina://amazon.com/account/shopping-cart\#add-item

Again, we can name the global lemina namespace a personified name: Lemina World. Thus, 'Hello, Lemina\!' and 'Lemina World' are inspired by the 'Hello, World' program.

# **Part 3 — Lemina Programming Model For Business Applications**

"Business applications" refers to enterprise applications or software solutions for information systems. They include those that can be used across multiple industries, such as content management or accounting systems, and those that only apply to certain types of companies, such as loan management or banking systems. These systems differ in application but share an ability to automate and improve the business process in their respective industries.

COBOL, designed in 1959, was the first programming language for business applications and a "common business-oriented language," as its name suggests. Since COBOL, many high-level programming languages have been used by businesses to build applications and improve their industry-specific workflows.

Today, modern business applications are internet-based, structured in two tiers (e.g., a frontend and a backend), and usually built by popular OO languages like Java and JavaScript. These traits define the programming languages most commonly used by businesses as well as the skills most frequently desired in job postings for software engineers, including:

* An ability to write programs in popular object-oriented programming languages such as Java and JavaScript (Angular JS for the frontend and Node JS for the backend)  
* An ability to design applications that comply with the microservices architecture with RESTful API  
* An ability to deploy applications to one of the major cloud service providers (e.g., AWS, Azure, Google Cloud, etc.)

Parts 1 and 2 illustrated how programming evolved from the framework of a single computer to a network of computers and finally to modern Internet applications. In the past, high-level programming languages and the object model (OOP) were sufficient to accomplish basic and advanced programming tasks. However, in the age of Internet programming, the lemina model offers a solution to the deficiencies in using current programming languages to create applications at the Internet scale.

Each stage of programming evolution improves programming knowledge and functionality without completely replacing the tried-and-true methods. High-level programming languages automate repetitive work on top of machine code. The object model creates a new form of code unit (as significant as the first cells coming to life to begin the life evolution) with internal logic implemented by high-level programming languages. In other words, all OO languages are high-level languages. The lemina model builds on this evolutionary process by teaching objects to socialize and work together to form societies of objects, which is what we call the "lemina way" of building programs.

Part 2 also demonstrated that by taking advantage of localization, one of the four core mechanisms of the lemina model, we could implement a lemina postal service that is backward compatible with OOP languages. Therefore, the lemina model in the backward compatible mode can be used to build business applications like other OO languages.

However, backward compatibility is only part of the full context of the lemina model's potential. Its real power comes from the mechanisms that make the model leap over the object model on programming's evolutionary path. With the lemina model, businesses can personify leminas as employees or roles and apply their organizing skills seamlessly to leminas and employees in the early planning and design phases.

A lemina has a textual name and a list of attention names. We name leminas with human or role names and use the naming convention of verb \+ noun for its attention names to more clearly represent employees or roles in business processes. At the same time, an actual employee or role also appears as a name and a list of tasks in the business process. Thus, leminas and employees established a relationship of one-on-one mapping in the business process context.

Businesses organize their activities as business processes and use tools such as BPMN (Business Process Model and Notation) or UML (Unified Modeling Language) to design and describe business processes.

UML has two behavior diagrams: the activity diagram and the use case diagram. The activity diagram contains activities and condition checks but doesn't specify who will perform them. In this case, the business process owner or manager should refine the activity diagram to a lemina activity diagram by denoting the number of leminas involved and marking each activity to its owning lemina. Conversely, leminas can directly replace the actors in the use case diagram.

BPMN only has one pool diagram, which is similar to UML's activity diagram but with two enhancements. First, a pool uses multiple lanes to represent employees or roles who will perform the activities. Second, BPMN uses gateways to represent condition checks on splitting and merging. Thus, leminas can directly replace lanes in the pool.

So far, we have reviewed how the lemina model can be used as an OO language to build business applications and model high-level business behaviors. In the rest of Part 3, we will focus on modeling business data in the lemina way.

Let us start with a pool, which represents a business process. A pool may have one or more lanes, each representing an employee or role. Since we use a lemina to implement a lane, all activities in the lane will become the lemina's internal attention names.

Thus, the lemina will need two types of information to perform the activities. The first is the information activities required for the lemina to coordinate themselves, including overall status, each activity's status, partial results, etc. We can call this kind of information administrative data, and it can be at different scopes, including lane, pool, and cross-pool diagrams.

The second is information regarding the targets to which the activities apply actions. For businesses providing services, the targets could be shopping carts or bank accounts. For companies manufacturing goods, the targets could be data generated by goods or manufacturing processes. Usually, this type of information goes beyond business processes and belongs to the company's central business domain.

The admin data is usually private to its scope and has a one-on-one relationship with it. On the other hand, a business process is generally independent of the domain data and has a one-to-many relationship: a business process or an activity may operate on multiple domain data. For example, a worker must update the assembly line inventory for the ten parts (minus one for each) and the toy (plus one) when the worker assembles a toy with ten parts on an assembly line. At the same time, other business processes may use the same domain data. Hence, at a more extensive scope, it is a many-to-many relationship between business processes and domain data.

There are hundreds, if not thousands, of industries worldwide. Companies have their ways of doing business, even within the same industry. For example, one bank offers a checking account that doesn't charge a monthly fee, while another may waive the fee if the account's daily balance is over $500. This situation makes designing standard data models or structures for each industry impossible since every industry and business would require new parameters for program functions to learn.

However, we still need a commonality when discussing and working with data because the only association between the reality of the business's operations and the functionality of its computers is the organization of its data. When things happen in the real world, computers learn them through data generated by or for the events. Similarly, when computers (programmed by people, of course) want to impact the world, they create data to let people react (e.g., passively, for example, a report) or drive devices (e.g., actively, for example, an industrial robot) to perform physical actions.

I created two data concepts, Account and Event, to allow us to reference relevant data before complete data structures became available while modeling business process behaviors.

"Account" is an overloaded term with many meanings. When it is joined with another noun in front of it in a noun-noun collocation, such as a bank account, a customer account, an email account, a Google account, etc., the Merriam-Webster dictionary defines it in two ways:

* Entry 3-a-(1) — A formal business arrangement providing for regular dealings or services (such as banking, advertising, or store credit) and involving the establishment and maintenance of an account  
* Entry 3-b — An arrangement in which a person uses the Internet or email services of a particular company

The arrangements defined in the two entries are the same as both refer to an arrangement between an account provider and holder, while the holder could be a subject (e.g., a person, a thing, etc.) or concern.

A lemina account is such an arrangement since it is abstract until it is associated with a subject, which could be an entity in the business domain, such as a bank account or an inventory account, or a representation of a business process's admin data, such as a place-order process account.

More specifically, a lemina account's arrangement refers to a group of relevant data items regarding a subject or concern. These data items will change on lemina events throughout the account's lifespan.

Abstract lemina accounts and events provide identification information. An account contains two fields:

* Account type or name  
* Account instance ID or number

An event contains four fields, two of which point to the parent account instance:

* Account type  
* Account instance ID  
* Event type  
* Event instance ID

A good analogy is using paper to record an account's data structure by writing the header section with identifications before we have details. This piece of paper serves as a placeholder to provide referenceability. Now, this account can participate in our thought processes and help us model business process behaviors.

This account-centered approach also aligns business and IT people in breaking down data structures while modeling data. Thus, business people can participate in data structure design as well.

Before closing Part 3, let us assemble a picture of how lemina models business applications.

First, we use BPMN or UML to model business process behaviors and refine them by replacing BPMN lanes or UML actors with leminas (it is also possible to model the behaviors directly with leminas). In this portion, leminas perform activities and condition checks in the business processes.

Once the process is established, we identify accounts and events. For identified accounts and events, we can start with the primary identification information (e.g., type and ID) and refine the data structure throughout the modeling and designing process.

For each account, we can assign a lemina and equip the lemina with the knowledge or business logic required to apply changes to the account based on the received events.

Thus, we have a group of leminas that perform activities and another group of leminas that perform bookkeeping against accounts. As mentioned earlier, these leminas interact in a many-to-many relationship. A behavior lemina may coordinate several account leminas to complete one activity; for example, after the toy assembling activity, the behavior lemina needs to update inventory for the toy and the other ten parts, which are eleven account instances if they all belong to the same account type.

By coordinating, lemina groups can model business applications more efficiently than past programming methods. However, the development process for business applications comes with unique challenges that we will address in Part 4\.

# **Part 4 — Lemina Business Application Development**

The lemina programming model can model business applications in three steps.

Step 1 is to create lemina accounts for data structures of business processes and domain subjects. A lemina account is a placeholder and container of data items related to a particular business concern or arrangement, such as a checking account, customer account, business process admin account, etc. Usually, we start to identify and realize data items late during the business requirement elicitation and analysis phases. Therefore, we need placeholders for reference before data items come to life.

An account has a type name, and an instance of that type will have an instance ID. Some accounts may contain constants. For example, an account instance with the type name' business holidays' and instance ID '2024' includes all business-recognized holidays in 2024 for receiving payments, which would remain the same.

However, most accounts will change throughout their life spans, and lemina accounts cannot change without a trace. Lemina events are designed to trigger changes against account instances and carry all necessary data to complete the account changes. Similarly, a lemina event has the concepts of type and instance. An event instance specifies an account type name, an account instance ID, an event type name, and an event instance ID. A significant difference between accounts and events is that events are historical records that cannot change after they have happened, while accounts can.

Step 2 is to utilize lemina's flexibility to represent various entities in different contexts. The native context is a lemina postal service in which a lemina is a recipient uniquely identified by its name. In this context, a lemina represents an individual. In a slightly extended context, a lemina represents an organization as a lemina further supports internal addressing by specifying attention.

Outside the postal service, a lemina can represent an individual in a business context. Businesses hire people based on skills relevant to their positions (such as taking an order or canceling an order) rather than irrelevant skills (such as fishing or hunting). In such a context, an individual is viewed in a computer model as an entity identified by name with a list of skills, behaviors, or actions. Thus, leminas can represent individuals in business when skills are associated with attention.

Let's switch to a third context where leminas can represent lemina accounts. More precisely, a lemina represents an individual with the knowledge and skills to apply all events to the associated account. When we associate the lemina with the account and the lemina's skills with the account's events, we effectively use the lemina to represent the lemina account.

Please note that a lemina represents a type of account. When applying a specific event, the lemina will retrieve the account instance specified by the event and operate on the account instance. It is the typical way to use leminas to model accounts, but there could be other ways. Remember, the lemina model opens the door to how people behave and socialize by using societal patterns.

Step 3 is to reveal the big picture of a business application model. A business application, or any software application, consists of behaviors and data. Business behaviors are usually modeled as business processes, each containing a set of business activities. The details of behaviors are laid out in each activity as business logic. Together with a set of domain data structures, all the details provide a raw view of the business application.

Step 1 refines the above raw view by introducing lemina accounts and events for business processes and domain subjects. Thus, business logic is transported into events. For example, placing an order is an activity in a business process that is then converted into an event against the business process admin account representing the business process. This event knows the business logic for charging the customer against the customer's payment account and reducing the inventory against the product's inventory account. Then, this event will issue two more events against the domain accounts: the customer's payment account and the product's inventory account. Similarly, the two domain events know the business logic for updating their accounts accordingly.

Step 2 further refines the updated model from Step 1 using leminas to represent business process admin and business domain accounts. As a result of these two steps, the lemina model can produce a general business application model comprising a set of leminas representing business process admin accounts and a separate set of leminas representing business domain accounts. Notably, all business logic is associated with events, so all accounts are central to the lemina model's view.

A general model enables a general model implementation, which provides at least two sets of essential functions. The first set displays and examines lemina account and event contents by browsing and searching account types, account instances of a selected account type, and events of a selected account instance.

The second set accepts one or more consecutive events and applies them to the specified account instance by executing their logic (remember, business logic is associated with events). As business logic is invisible, examining its correctness involves comparing the before-and-after contents of the account instances it impacted. Thus, the model implementation can support manual verification and automated testing.

The lemina method for business application development creates an environment that can streamline any new addition or update (including data items, business logic, business process flows, test cases, etc.). In the real world, there are already development environments for software engineers called CICD, which stands for Continuous Integration and Continuous Deployment. However, the lemina development environment further covers requirement management with its unique process automation and streamlining features.

The lemina method employs three techniques to achieve its goals. The first technique is an all-in-one document, which includes everything from requirements, data structures, business logic, and source code that implements the business logic. Ideally, it should be written using markdown syntax, which is text-based (helpful in displaying Pull Request diffs) and straightforward enough for anyone familiar with standard office software to learn in just a few days. An all-in-one document represents and describes a lemina account type or event type with multiple sections:

* A form that visually represents data items   
  * Mainly for people's consumption (e.g., US Tax Return Form 1040\)  
  * To display data contents on the screen  
* A JSON structure that represents data items   
  * Mainly for computer consumption (e.g., data types in code)  
  * JSON is also friendly to people (most business analysts understand JSON)  
* Detailed explanation for every data item (e.g., Form 1040 Instructions)

If it is an account type, it has extra sections:

* A list of event types owned by this account type

If it is an event type, it has extra sections:

* An account type owning this event type  
* Detailed business logic, including nature language and pseudocode, for how to apply changes to the specified account instance  
* A code file name that contains the actual source code for the business logic (unfortunately, code will be in a separate file until an IDE can extract code from an all-in-one document)

The second technique is a Git repository from a vendor such as GitHub or GitLab. The Git repository stores all-in-one documents for all lemina accounts and events. Thus, we manage the requirement changes like code changes through PR (Pull Request).

The third technique is a customized build tool (e.g., Maven or Gradle) that pulls code files from all-in-one documents and creates a model implementation. A base model implementation should be developed before the first all-in-one document exists.

With these techniques, the lemina method provides some immediate benefits. Firstly, since all information is stored in one Git repository, all users remain aware of the full context of the business application. For a business application to be developed simultaneously by dozens or hundreds of people, users must understand what they are doing, what other users are doing, and why everyone is collectively performing specific actions at specific times. This situational awareness of the application's functions and goals improves overall efficiency, increases the odds of project success, and reduces the risks of project failures and delays.

Secondly, the Git Pull Request (PR) mechanism prevents conflicts by overlapping across teams as a last resort when a PR contains all related data items, business logic, and source code changes. Usually, the first defense to avoid such conflicts is to designate well-arranged features or areas for each team to work on. However, teams will get closer when the progress goes into the late stages due to different reasons:

* The nature of the application may need to have precise edges among its features.  
* The deadline is approaching, so more teams are working in the same area.  
* Some teams are idling and would benefit from joining the project.  
* Teams step on each other's toes accidentally.

The PR mechanism doesn't prevent conflicts from happening beforehand but prevents them from being committed. Fixing such conflicts earlier saves the business money and mitigates the risk of liabilities.

Finally, a unit of work (e.g., a PR by a team in a sprint) will contain work regarding requirement elicitation or adjustment, design, coding, and testing, which covers the unit of work's entire life cycle. As a result, the unit of work is more independent and forms a feedback loop. This situation perfectly demonstrates the agile principles.

Inspired by the term CVT (continuously variable transmission), I call the fine granularity of agility offered by the lemina method CVA (A for agility).

The lemina development method for business applications delivers benefits in process efficiency and performance management. Yet, the lemina method aims to bring enterprises additional benefits at the strategy level. It can be summed up as letting business people complete the full development of their applications up to functional reference implementations without needing IT people (or keeping a minimum). A functional reference implementation refers to the model implementation equipped with features for all functional requirements but no features for nonfunctional requirements, which *will* be left to the IT people.

Here is a brief explanation of how everything we mentioned above makes this possible using the lemina development method.

**Use forms to represent data structures.**

The use of forms bridges the gap between business and IT mindsets. Before computers were invented, people performed business activities with universally understood forms. It is natural for business people to analyze business processes and activities and use forms to represent data needed for those processes and activities.

On the other hand, forms and JSONs have the same expressiveness regarding data and data structure, so they can easily be converted.

**Create small and well-defined contexts for implementation.**

Business logic is associated with activities in the business processes, activities are associated with events, and events are associated with attention in leminas. So, lemina attention is the context and unit of code that handles an event and implements the event's business logic.

Lemina attention is a well-defined context that includes at least the event instance, the specified account instance, and other account instances that may be involved according to business logic.

Programming business logic in a clearly defined context is straightforward, even for non-IT people. Computer programming has been taught in colleges for all majors since the 1990s, so it is safe to claim that most business analysts, who are specialized business people, know how to program in this situation.

**Utilize functional reference implementations.**

The ideal development environment should provide a base model implementation and a customized build tool before development starts. Thus, once it has been reviewed, approved, and merged, every PR containing changes for requirements, data items, business logic, and source code will be built and deployed into the running model implementation for manual verification and automated testing. The model implementation becomes a functional reference implementation when it is equipped with business features and functions.

Adam Smith opens The Wealth of Nations with these words: "The greatest improvement in the productive powers of labour … seem to have been the effects of the division of labour." In the programming world, the original model of the lone programmer creating the building blocks of applications and networks has given way to teams of people with various experience levels coding smaller programs within the broader context of the project. Today, IT teams take the work of business people and wire it together into final production applications, adding features for nonfunctional requirements like performance, security, usability, reliability, and scalability.

While IT teams won't touch the function reference implementation, they will assemble data structures and code from the Git repo to create a production implementation with nonfunctional features. The lemina method expects two implementations to run parallel through their life spans to ensure business people have a dedicated implementation they can reference for verification or continuous development, even as their operations scale in size and objective. Further division or specialization of labor is the next step on the programming evolutionary path, requiring a consolidated solution like the line model to integrate the business reference implementation with IT finalization for the next generation of Internet applications.


© Copyright 2024 Rex Young. All Rights Reserved.
