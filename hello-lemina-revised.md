# Hello, Lemina\! (revised)

© Copyright 2025 Rex Young. All Rights Reserved.

![contact](lemina-contact.jpg)

Part 1 — Programming's Evolving Path  
Part 2 — Lemina Programming Model  
Part 3 — Lemina Programming Model For Business Applications  
Part 4 — Lemina Business Application Development

# Part 1 — Programming's Evolving Path

Computer programming is a fascinating discipline deeply tied to the operations of the CPU. Its development shares parallels with other machine-operating techniques, such as driving a car. Both programming and driving have evolved along similar trajectories, striving for operational efficiency through parallel advancements. This human-centered evolution of programming—a journey relatable to us all—forms the core of our discussion.

When new machines are invented, users initially adapt to their limitations. Take the first modern car, the Benz Patent-Motorwagen No. 1, built by Karl Benz in 1885\. It requires drivers to use a centered steering crank instead of a steering wheel and a left-handed gas-and-brake lever instead of pedals.

Over time, however, a wave of human-centered features emerged in car design to better align operations with natural human reactions. For example, General Motors introduced automatic transmissions in its Oldsmobiles in 1924, and Chrysler pioneered power steering in 1951\. These innovations transformed how cars function, catering to drivers' desires for intuitive and relatable machines. Other human-centered additions followed, such as cruise control, which allows drivers to maintain a constant speed without pressing the gas pedal, and anti-lock braking systems, which prevent wheels from locking during braking, enhancing control in critical moments.

Today, car driving nears the end of its evolutionary journey. With just an address, self-driving cars can deliver passengers to their destinations without further human input.  
Much like early automobiles began with rudimentary mechanics, early programming started with machine code. Each machine code instruction corresponds to a specific CPU operation, such as:

* Arithmetic operations (e.g., addition, subtraction, multiplication, division) on two "words" (numbers within limited ranges)  
* Bitwise operations on one or two words  
* Jumping to another memory address to execute stored machine code  
* Comparing two words and conditionally jumping based on the result

A "word" refers to the size of CPU registers and memory units. The Intel 8088 CPU, used in the first IBM personal computer in 1981, was 8-bit, capable of representing numbers from 0 to 255 (or \-128 to 127 with a sign). If a program required a number exceeding 255, programmers had to write additional machine code to handle multiple words. Expanding word size was not straightforward, as it depended on physical circuits embedded in the chip to support each bit of the CPU's registers and memory. Larger word sizes demanded much more circuits. By 2000, personal computers had adopted 64-bit CPUs, such as the Intel Pentium 4 and today's Intel i9 processors.

To non-IT observers of modern devices—smartphones, gaming consoles, internet applications, cloud computing infrastructures, and AI-enabled programs—it is hard to believe that CPUs operate at such a raw, fundamental level. The tedious nature of working with "dumb" machine code spurred programmers to innovate, introducing waves of human-centered features into modern programming.

The first wave brought high-level programming languages like FORTRAN (developed by IBM in 1957 as the first of its kind), COBOL, and BASIC. These languages introduced user-friendly elements such as English keywords, data types, variables, arithmetic expressions, and procedures (or functions). Unlike machine code, programs written in high-level languages cannot be directly executed by the CPU. They require translation into machine code via a compiler (which translates the entire program beforehand) or an interpreter (which translates line-by-line during execution).

This shift yielded two transformative benefits. First, compilers automate repetitive tasks, boosting efficiency. Previously, programmers manually wrote extra machine code to handle numbers exceeding the CPU's capacity. With high-level languages, compilers managed new data types and variables, freeing coders for more complex challenges. Second, procedures enabled programmers to group reusable code, eliminating redundant effort and streamlining workflows.

The second wave introduced object-oriented programming (OOP), a concept coined by Alan Kay in 1967\. An "object" encapsulates private states (data) and behavior (code), accessible only through predefined interfaces or "methods" (procedures or functions). Like their high-level predecessors, OOP languages rely on compilers or interpreters to translate programs into machine code. This innovation expanded programming's reach, enabling a broader range of applications.

These first two waves fundamentally reshaped programming. Most modern languages are now high-level and object-based (a broader term than object-oriented). While high-level languages automate repetitive tasks, objects tackle growing code complexity by providing a new building block for program construction. Objects are as revolutionary to programming as the division of labor was to economics in Adam Smith's The Wealth of Nations. They allow programmers to shift from designing every computational step to organizing specialized objects with relevant data and behaviors. Programming has thus evolved into a twofold process: crafting detailed steps to create objects and orchestrating them into cohesive programs.

Annual rankings of popular programming languages show that OOP languages will remain dominant in 2024\. Does this suggest that programming has stagnated since the late 1960s? Surprisingly, no breakthroughs in general-purpose programming have emerged since the OOP revolution. Yet, the IT industry has not stood still for 60 years. It has expanded into every facet of life, shaping daily experiences and interactions. This expansion is evident in three key areas:

* **Participation**: Programming and computing have grown from a niche within academia and research to a sprawling IT industry.  
* **Devices**: Computers have evolved from mainframes to personal computers, handheld devices (e.g., POS scanners), smartphones, and any gadget with a CPU capable of running programs.  
* **Platforms**: Programming now spans single-CPU processors to multi-core systems, networked computers (e.g., corporate networks or clouds), and the internet, connecting everything and everyone 24/7.

This shift marks two distinct eras: one focused on invention, the other on applying programming across broader domains. The meaning of programming has also changed—from coding for a single computer to programming multi-core, networked systems, essentially "programming the internet."

Let us return to the automobile analogy. The programming industry has moved from inventing the car to exploring what a single car can do, and now, it is coordinating multiple vehicles for broader objectives. To chart programming's future, we must reassess its trajectory along two fronts: Is OOP sufficient for programming the internet? And what, beyond OOP, has driven progress toward more complex, efficient applications?

Programming the internet demands techniques for concurrent and distributed programming. While modern OOP languages have added features like multi-threading, the object model lacks inherent support for concurrency. Past efforts, such as Carl Hewitt's Actor model (1973) and Greg Lavender and Douglas Schmidt's Active Object pattern (1996), have not gained mainstream traction. Similarly, the object model does not natively support distributed programming. Initiatives like CORBA, DCOM, and Java RMI have seen limited adoption. Instead, hardware and software architectures—such as middleware and microservices with RESTful APIs—have propelled internet programming forward.

These observations highlight potential bottlenecks in programming the Internet in 2024 and beyond. We need a unified, human-centered model that seamlessly handles concurrency, intra-process programming (within a single program), and inter-process programming (across multiple programs and computers). Intuitive and instinctive, this model should be to programming what the steering wheel was to the steering crank—a natural evolution.

# Part 2 — Lemina Programming Model

In Part 1, we explored the current state of programming and its future trajectory. This understanding helps us evaluate whether a new programming technique aligns with its evolutionary path and guides us in designing innovative solutions. To create a unified programming model, the author analyzed the core behaviors and mechanisms of existing programming techniques and compared them to how humans interact in social and business contexts. Drawing inspiration from human social models, the author developed the Lemina programming model—a human-centered approach rooted in these principles.

At its core, a CPU executes a program one statement (or one line of code) at a time. To explain this to non-IT audiences, consider a train analogy: the train represents the CPU, the track represents the program, and each sleeper (the wooden supports beneath the track) represents a line of machine code. The train moving over sleepers mirrors the CPU executing code within a program.

Early programming, such as on the Manchester Baby—the first electronic stored-program computer built in 1948 at the University of Manchester—lacked subroutines or procedures. With only eight basic instructions, its programs were structurally one-dimensional (1D): all code lay linearly along a single track, like sleepers under a central rail.

The introduction of procedures added a second dimension (2D). Each procedure forms a parallel track alongside the main one, spanning a two-dimensional plane. The train runs along the main track, "teleports" to a procedure's track when encountering a call, and stores the next position on the main track in a stack. After completing the procedure, it teleports back to resume execution. Here, "teleport" describes the CPU's instantaneous jump to another memory address, a concept without a direct equivalent in real trains.

Objects extend this analogy further. An object can be envisioned as multiple tracks (its methods) enclosed by a fence protecting private data. Yet, even with objects, programs remain fundamentally 2D.

Multi-core CPUs introduce multiple trains executing the same program simultaneously—a necessity for modern applications. Assigning a train to each procedure track accelerates complex calculations, much like adding more hands to a task. Another everyday use case is server programs supporting numerous concurrent clients.

Multiple trains add a third dimension, making programs with multi-threading at runtime "3D programs." This shift, however, introduces new challenges. A single train has full awareness of the program's state, but how do multiple trains coordinate when executing tasks concurrently? Should the main train wait for a procedure train to finish or proceed? If it does not wait and the procedure train produces results, how are those results delivered mid-execution?

In programming, these interactions are termed synchronous and asynchronous procedure invocations. Synchronous calls allow the caller to wait and receive results immediately, while asynchronous calls let the caller move forward, complicating result retrieval. Solutions like Future, Promise, and Callback with Closure address this, but their technical nature feels less intuitive than modern programmers might prefer.

In Part 1, we described objects as a "new life element" in programming, tackling structural complexity but not fully addressing behavioral challenges posed by concurrency—whether within a single computer or across multiple systems. Objects, while revolutionary, remain incomplete, needing enhancements to act as genuinely independent entities in today's programming landscape.

This analysis points to a clear solution: a unified, human-centered model for managing synchronous and asynchronous interactions within and across programs and computers.

To find this direction, the author drew parallels between 3D programs and human societies. People operate on Earth's 2D surface, but their decisions and actions—driven by thought and intent—add a third dimension. Similarly, 3D programs combine a 2D code structure with runtime concurrency. Inspired by this, the author examined human social interactions and identified the real-world postal service as a potential foundation for a new programming model.

Thus, the author developed the Lemina programming model, borrowing concepts from postal services to introduce two key elements: lemina services and leminas. In the real world, postal services deliver mail from anonymous senders to registered recipients. Lemina services mirror this by delivering messages from any sender—anonymous code, including leminas—to registered recipients.

The author chose the term "lemina," a personified name, over traditional programming terms like "object" or "actor" for three reasons:

* To honor the real-world inspiration  
* To indicate a human-centered design  
* To emphasize that leminas are distinct from objects or actors, though they can be implemented using objects, actors, or procedures that adhere to the Lemina model.

The Lemina model replaces procedure invocation with message passing. Procedure invocation assumes a single thread of execution (one train) handling both caller and callee, while message passing reflects communication between independent entities—like humans or programming elements. Here, "procedure" encompasses functions, methods, subroutines, and similar constructs used interchangeably.

Procedure invocation is a low-level, CPU-centric mechanism. The Lemina model, a higher abstraction, does not eliminate it but redefines its role where it is ill-suited. In traditional invocation, the flow is *caller → procedure*. The Lemina model introduces a middleman: *caller → outbox → lemina service → inbox → lemina*, where the lemina represents the procedure.

The lemina service provides a public *outbox* for all users and a private *inbox* for each lemina, both integral to its design. These terms reflect the sender's and lemina's perspectives, respectively. It transforms a single procedure call into two distinct steps: one from caller to lemina service (via outbox) and another from lemina service to lemina (via inbox).

For internet-scale programming, networked lemina services extend this: *caller → outbox → source lemina service → {networked lemina services} → target lemina service → inbox → lemina*. The caller and lemina remain unchanged across configurations, ensuring consistency.

In summary, the traditional invocation model (common in high-level, object-oriented languages for intra-process programming):

* *Caller → procedure*

Becomes the Lemina model (for both intra- and inter-process programming):

* *Caller → outbox → {lemina service(s)} → inbox → lemina*

It can be abstracted further as one-way message passing:

* *Sender → {lemina service(s)} → lemina*

The Lemina model relies on four foundational mechanisms to achieve its goals:

* Textual ID  
* Reply-to  
* Localization  
* Namespace

## Textual ID

In the real world, postal recipients use addresses—tied to physical locations—rather than names for delivery. In the digital realm, names and addresses are interchangeable. Thus, in the Lemina model, lemina ID, name, and address refer to the same concept.

Lemina IDs are textual, forming the model's cornerstone and enabling key features:

* **Referenceability**: Textual IDs allow anyone—not just IT experts—to use lemina names intuitively in thought, conversation, or business processes.  
* **Reachability**: Textual IDs ensure messages reach leminas, whether within a program or across the internet. Textual messages enhance compatibility across languages, systems, and networks, aligning with existing protocols.  
* **Human-style reply-to**: For asynchronous (two-way) messages, textual IDs enable a reply-to mechanism akin to leaving a return address in human interactions.

A lemina might represent a single procedure, multiple procedures, an object with methods, or several objects. For multiple entities, internal addressing is needed. The Lemina model introduces an attention name mechanism inspired by real-world envelopes with "Attn:" lines. Attention names follow a lemina name, separated by a pound sign (\#), e.g., "Alice\#place-order," "Alice\#cancel-order," or "shipping-team\#ship-order." Lemina names are case-insensitive to minimize human error.

## Reply-to

The Lemina model's core is one-way message passing. A sender uses the outbox to send a message by name (syntax below is illustrative, as outbox details vary by implementation):

* *outbox.send("Alice\#place-order", \<message\>)*

Messages are one-way, operating in a "send-and-forget" style from the sender's perspective.

As noted earlier, asynchronous invocation excels at sending but struggles with result retrieval. The Lemina model introduces a reply-to mechanism to replace technical solutions like Future, Promise, and Callback with Closure. A reply-to address is included in the message, allowing the lemina (or its service) to send results back:

* *outbox.send("send-to: Alice\#place-order", "reply-to: shipping-team\#ship-order", \<message\>)*

Here, "send-to" and "reply-to" are illustrative labels, not formal syntax, as lemina ID, name, and address are equivalent. The "shipping-team" lemina receives results at "ship-order." For synchronous needs—such as legacy code requiring in-place results—the model avoids native sync support, delegating this to the outbox:

* *\<results\> outbox.await("Alice\#place-order", \<message\>)*

The outbox handles sync calls by creating a temporary lemina, registering it, adding its name as a reply-to address, and passing results back to the caller when received.

## Localization

The lemina service (*caller → outbox → lemina service → inbox → lemina*) is the model's backbone, encompassing outbox and inbox. With countless programming languages and design variations, a universal implementation is impractical. *Localization* allows programmers to implement lemina services freely, provided they adhere to the core principle: a caller with a lemina name and outbox access can send a one-way message.

Message compatibility remains the sender's responsibility, akin to writing a letter in a language the recipient understands. To illustrate this flexibility, consider three distinct Java-based designs for a lemina service handling a legacy "Sales" class with methods like "placeOrder" and "cancelOrder," plus a combined approach:

* **Sync Design**: The lemina service maps lemina names to Java objects, using reflection to invoke methods synchronously on the caller's thread (e.g., *outbox.call("sales\#placeOrder", \<parameters\>)*). It preserves legacy behavior with minimal overhead.  
* **Async Design**: The service maps lemina names to objects and inboxes, queuing parameters for a thread pool to process asynchronously (e.g., *outbox.call("sales\#placeOrder", \<parameters\>)*). It enables concurrent execution across multiple threads.  
* **Combined Design**: This merges sync and async approaches, offering methods like *outbox.syncCall ()* and *outbox.asyncCall ()* to support both paradigms within a single service.  
* **Actor Design**: Similar to the sync and async designs in mapping objects and methods, this approach assigns a single dedicated thread per lemina name. The thread processes queued parameters sequentially, mimicking the Actor model's isolation and order preservation.

Localization ensures flexibility while supporting legacy and concurrent use cases.

## Namespace

Lemina services can operate standalone or networked. The model avoids mandating a network topology, leaving this to implementers. However, networked services risk name collisions. The namespace concept resolves this by defining scopes where lemina names are unique and reachable:

* **Single Namespace**: One service with names like "Alice" and "Bob."  
* **Multiple Namespaces**: Two services (s1: "Alice," "Bob"; s2: "Charlie," "David") form separate namespaces (s1, s2) or a shared one (s1s2) with patterns like "s2/David."  
* **Global Namespace**: Using internet protocols and domain names (e.g., *lemina://amazon.com/account/shopping-cart\#add-item*), dubbed "Lemina World," echoing "Hello, World\!"

# Part 3 — Lemina Programming Model For Business Applications

"Business applications" refer to enterprise software or information system solutions. These include cross-industry tools like content management or accounting systems, as well as industry-specific solutions like loan management or banking systems. Though their applications vary, they share a common goal: automating and enhancing business processes within their respective domains.

COBOL, introduced in 1959 as the "Common Business-Oriented Language," was the first programming language tailored for business applications. Since then, numerous high-level languages have been adopted to develop applications that streamline industry-specific workflows.

Modern business applications are internet-based, typically structured in two tiers (e.g., frontend and backend), and built using popular object-oriented (OO) languages like Java and JavaScript. These characteristics shape the skills most sought after in software engineering job postings, including:

* Proficiency in writing programs using widely-used OO languages such as Java and JavaScript (e.g., AngularJS for frontends, Node.js for backends)  
* Expertise in designing applications that adhere to microservices architecture with RESTful APIs  
* Capability to deploy applications to major cloud platforms (e.g., AWS, Azure, Google Cloud)

Parts 1 and 2 traced programming's evolution from single-computer frameworks to networked systems and, ultimately, internet-scale applications. High-level languages and the object model (OOP) once sufficed for basic and advanced tasks. However, in the era of internet programming, they fall short. The Lemina model addresses these gaps, building on prior advancements to meet the demands of today's interconnected landscape.

Each evolutionary stage enhances programming without discarding proven methods. High-level languages automate repetitive tasks atop machine code. The object model introduces a new code unit—comparable to the emergence of life's first cells—implemented with high-level languages (all OO languages are inherently high-level). The Lemina model extends this progression, enabling objects to "socialize" and collaborate as societies, a paradigm we call the "Lemina way" of building programs.

Part 2 showed how the Lemina model's localization mechanism allows backward-compatible implementations with OO languages. In this mode, it can construct business applications much like traditional OO approaches. However, backward compatibility is just one facet of its potential. The Lemina model's true strength lies in mechanisms that propel it beyond the object model, advancing programming's evolutionary path. Businesses can personify leminas as employees or roles, seamlessly integrating organizational skills into early planning and design phases.

A lemina has a textual name and attention names, styled as verb \+ noun (e.g., "place-order," "cancel-order") to mirror employee tasks or roles in business processes. Similarly, employees or roles are defined by names and task lists. It creates a one-to-one mapping between leminas and human counterparts within a business context.

Businesses structure their operations as processes, often modeled using tools like BPMN (Business Process Model and Notation) or UML (Unified Modeling Language):

* **UML** offers two behavioral diagrams: the activity diagram (showing activities and conditions without specifying performers) and the use case diagram (featuring actors). For activity diagrams, process owners can refine them into lemina activity diagrams by assigning activities to specific leminas. In use case diagrams, leminas can directly replace actors.  
* **BPMN** uses a pool diagram akin to UML's activity diagram but enhanced with lanes (representing employees or roles) and gateways (for conditional branching and merging). Leminas can directly substitute for lanes.

Thus far, we have seen how the Lemina model functions as an OO language for building business applications and models high-level behaviors. The remainder of Part 3 focuses on modeling business data the "Lemina way."

Consider a BPMN pool representing a business process divided into lanes for employees or roles. When a lemina replaces a lane, its activities become the lemina's attention names. In order to perform these activities, the lemina requires two types of data:

1. **Administrative Data** is information for coordination, such as overall status, activity status, or partial results. This data is scoped to lanes, pools, or cross-pool interactions and remains private to its context.  
2. **Domain Data** is information about the targets of activities, like shopping carts or bank accounts for service providers or manufacturing data for goods producers. This data transcends processes and resides in the company's central business domain.

Administrative data is private and has a one-to-one relationship with its scope. Domain data, however, is process-independent and has a one-to-many relationship: a single process or activity may affect multiple domain data instances. For example, assembling a toy from ten parts requires updating inventory data for eleven items (ten parts decremented, one toy incremented). Other processes may also interact with this data, creating a many-to-many relationship at a broader scope.

With thousands of industries worldwide—and varied practices within them—standardizing data models is impractical. One bank might offer fee-free checking accounts, while another waives fees for balances above $500, necessitating unique parameters for each. Yet, data remains the critical link between real-world operations and computer functionality. Events in reality generate data for computers to process, while computers produce data to influence the world—passively (e.g., reports) or actively (e.g., driving industrial robots).

To address this, the author introduces two abstract data concepts—Account and Event—that enable data referencing before complete structures are defined during process modeling. "Account" is a versatile term. In noun-noun collocations (e.g., bank account, customer account), Merriam-Webster offers two relevant definitions:

* *Entry 3-a-(1)*: A formal arrangement for regular dealings or services (e.g., banking) involving account creation and maintenance.  
* *Entry 3-b*: An arrangement for using a company's internet or email services.

Both describe an arrangement between a provider and a holder (a person, entity, or concern). A lemina account follows this pattern, remaining abstract until tied to a subject—such as a business domain entity (e.g., bank account, inventory account) or administrative process data (e.g., a "place-order process account"). It represents a collection of relevant data items about a subject, updated via lemina events throughout its lifecycle.

Lemina accounts and events provide identification placeholders:

* **Account**:  
  * Account type or name  
  * Account instance ID or number  
* **Event**:  
  * Account type  
  * Account instance ID  
  * Event type  
  * Event instance ID

Think of an account as a paper form with a header for identification, awaiting detailed entries. This placeholder ensures referenceability, aiding thought processes and behavior modeling. It also bridges business and IT teams, enabling collaborative data structure design.

Before concluding Part 3, let us synthesize how the Lemina model constructs business applications:

1. **Model Behaviors**: Use BPMN or UML to outline business processes, refining them by replacing lanes or actors with leminas (or modeling directly with leminas). Leminas handles activities and condition checks.  
2. **Identify Data**: Define accounts and events, starting with essential identification (type and ID), and refine data structures iteratively.  
3. **Assign Logic**: Equip each account with a lemina containing the business logic to update it based on events.

It yields two lemina groups: one for process behaviors and another for account bookkeeping. Their many-to-many interactions enhance efficiency. For instance, after assembling a toy, a behavior lemina updates eleven account instances (toy and ten parts), coordinating with multiple account leminas.

Thus, the Lemina model offers a more effective framework for business applications than past methods. However, its development process poses unique challenges, which we will explore in Part 4\.

# Part 4 — Lemina Business Application Development

The Lemina programming model offers a three-step approach to developing business applications.

## Step 1: Create Lemina Accounts for Data Structures

Lemina accounts serve as placeholders and containers for data items tied to specific business concerns or arrangements, such as checking accounts, customer accounts, or business process admin accounts. Typically, data items are identified and detailed late in the requirement elicitation and analysis phases. Lemina accounts provide early reference points before these details emerge.

Each account has a type name and an instance ID. Some accounts, like a "business holidays" account with instance ID "2024," contain static data (e.g., recognized holidays for payment processing in 2024). Most accounts, however, evolve over time. Lemina accounts cannot change without a record; lemina events trigger these updates, carrying the data needed to modify account instances. Like accounts, events have a type and instance, defined by four fields: account type name, account instance ID, event type name, and event instance ID. Unlike accounts, events are immutable historical records.

## Step 2: Leverage Lemina Flexibility Across Contexts

Leminas adapt to various roles depending on context:

* **Native Context (Postal Service)**: Within a lemina postal service, a lemina is a uniquely named recipient, akin to an individual. With attention names for internal addressing, it can represent an organization.  
* **Business Context (Individuals)**: Businesses hire based on relevant skills (e.g., "place-order," "cancel-order") rather than irrelevant ones (e.g., fishing). A lemina, identified by a name and attention-based skills, mirrors an individual in this setting.  
* **Account Context**: A lemina can represent a lemina account by embodying the knowledge and skills to apply events to it. Associating a lemina's attention names with an account's event types effectively ties the lemina to that account type. When processing an event, the lemina retrieves and updates the specified account instance.

This approach—using a lemina to manage an account type—is standard, though the model's societal inspiration allows for alternative implementations.

## Step 3: Construct the Business Application Model

Business applications blend behaviors and data. Behaviors, modeled as business processes with activities, embed business logic. Combined with domain data structures, they form a raw application view.

* **Step 1 Refinement**: Lemina accounts and events replace raw data structures for processes and domain subjects. Business logic then shifts to events. For example, a "place-order" activity becomes an event targeting a process admin account. This event encapsulates the logic to charge a customer's payment account and adjust a product's inventory account, triggering two additional domain events to update those accounts.  
* **Step 2 Refinement**: Leminas represent both process admin and domain accounts, yielding a general model: one lemina set for process admin accounts and another for domain accounts, with all business logic tied to events.

This model supports a general implementation with two key function sets:

1. **Browsing and Inspection**: Tools to view and search account types, instances, and associated events.  
2. **Event Processing**: Mechanisms to apply one or more events to an account instance, executing their logic. Since logic is opaque, correctness is verified by comparing account states before and after execution, enabling manual checks and automated tests.

## The Lemina Development Environment

The Lemina method creates a streamlined environment for adding or updating data items, business logic, process flows, and test cases. While Continuous Integration and Continuous Deployment (CICD) environments exist for software engineers, the Lemina approach extends to requirement management with unique automation and streamlining features.

It employs three techniques:

1. **All-in-One Document**: A single markdown file captures requirements, data structures, business logic, and source code. Markdown's text-based simplicity (ideal for Pull Request diffs) is learnable in days by anyone familiar with office software. Each document describes a lemina account or event type with the following:  
   * Form: A visual data representation (e.g., like a US Tax Form 1040\) for human use and display.  
   * JSON Structure: A machine-readable data format that is also accessible to business analysts.  
   * Data Item Explanation: Detailed human-readable note like the Form 1040 Instructions.  
   * For account types: A list of owned event types.  
   * For event types: The owning account type, detailed business logic (natural language and pseudocode), and a code file name (code remains separate until IDEs can extract it from documents).  
2. **Git Repository**: Hosted on platforms like GitHub or GitLab, it stores all-in-one documents and manages requirement changes via Pull Requests (PRs) like code changes.  
3. **Customized Build Tools**: Like Maven or Gradle, extract code from documents to build a model implementation. A base implementation should precede the first document.

## Benefits of the Lemina Method

* **Context Awareness**: A unified Git repository ensures all users—potentially dozens or hundreds—grasp the application's full context, boosting efficiency and reducing risks of failure or delay.  
* **Conflict Prevention**: PRs containing related data, logic, and code minimize overlaps as a final safeguard. Early defenses include assigning distinct features to teams, though late-stage convergence (e.g., tight deadlines, overlapping work) is mitigated by resolving conflicts before committing, saving costs and risks.  
* **Agile Feedback Loops**: Each PR (e.g., a team's sprint) spans requirement elicitation, design, coding, and testing, fostering independence and aligning with agile principles. Inspired by "continuously variable transmission" (CVT), I term this fine-grained agility CVA (Continuous Variable Agility).

## Strategic Vision: Empowering Business Teams

Beyond efficiency, the Lemina method aims to enable business people to fully develop applications—up to functional reference implementations—with minimal IT involvement. These implementations cover all functional requirements, leaving nonfunctional aspects (e.g., performance, security) to IT teams. Here is how:

* **Forms for Data Structures**: Forms, intuitive to business users from pre-computer eras, represent data naturally. Their equivalence to JSON allows seamless conversion, bridging business and IT perspectives.  
* **Small, Defined Contexts**: Business logic ties to lemina attention names via events, creating precise coding units (e.g., an event, its account, and related accounts). Most business analysts, trained in programming since the 1990s, can code in such contexts.  
* **Functional Reference Implementations**: A pre-built base implementation and build tool integrates PRs into a running model for verification and testing, evolving into a functional reference implementation as features are added.

## The Next Evolutionary Step

Adam Smith begins The Wealth of Nations with: "The greatest improvement in the productive powers of labour … seem to have been the effects of the division of labour." Programming has shifted from lone coders to collaborative teams, with IT finalizing business inputs into production applications and adding nonfunctional features. The Lemina method envisions parallel implementations: a business-led functional reference for verification and development and an IT-led production version with nonfunctional enhancements. This division of labor marks the next step in programming's evolution, requiring a unified model like Lemina to integrate business and IT efforts for future Internet applications.  

© Copyright 2025 Rex Young. All Rights Reserved.
