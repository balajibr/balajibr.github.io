[← back](../)

# Career notes

*Draft, v2. The factual arc is here. The parts worth actually reading are the ones only I can fill in, marked below.*

---

Twenty-seven years, 1999 to now. Long enough that the industry I started in and the one I work in today share very little vocabulary.

Writing this down, I noticed two threads I had not consciously connected before. One is making complicated information findable. The other is automating the judgment that sits between two steps that are already automated. Almost everything below is one or the other.

## Wipro, 1999 to 2001: structured documents

I started on DynaWeb, Enigma's distributed content management and e-publishing system. We were tailoring it for Bombardier Aerospace, and the job was getting them off paper. What came out the other side were Interactive Electronic Technical Manuals for the CRJ and Q400 fleets: maintenance manuals, wiring manuals, illustrated parts catalogs.

Underneath it was structured SGML, held to aviation industry data standards. It served over corporate intranets and extranets, and also shipped on disc, so a mechanic in a hangar with no network could still pull up the manual.

The engineering problem was formatting on the fly. Raw structured data went in, and stylesheets applied presentation dynamically depending on which browser was asking. In 1999 that meant fighting Netscape and Internet Explorer at the same time. Long compilation times, unforgiving DTDs, and a document model that had no tolerance for sloppiness, because the documentation described aircraft.

The piece I remember most clearly is the illustrations. We embedded vector graphics, catalogued them, and pushed them into the search index. Someone working on a complex engine assembly could search for a single screw or bolt and zoom straight to it. That was really the point of the whole project. We were building a structure precise enough that any individual component on an aircraft became addressable.

I did not think of it that way at the time. It was a retrieval problem over structured technical data. I would end up back at that same problem twice more.

<!-- TODO: Balaji, two things here. (a) Worth checking the specifics before this goes public: the exact data standards, and how much of the stylesheet and DTD detail is your own memory versus reconstructed after the fact. I deliberately kept the resume version vaguer. (b) What made you move to Honeywell? -->

## Honeywell, 2001 to 2005: what production actually means

Refinery and oil enterprise software. Production planning, production analysis, operations management. Dynamic cubes for production modeling, workflow automation for refinery planning, and remote automation products for plants that could not simply be restarted.

That last part is what stuck. A bug in that world could take a process unit offline and cost a plant hours of production. You learn to think about failure modes before features, and "it works on my machine" stops meaning anything.

Everything I later took for granted about production discipline, I learned here first, in a place where the physical world was downstream of the code.

<!-- TODO: Balaji, was there a specific project or a specific ceiling that ended this chapter? Any story from the refinery work that still comes to mind? -->

## Microsoft, 2005 to 2018: the shift to platform

Thirteen years, and they line up almost exactly with the industry's move to cloud.

Software engineering lead for Managed Services for Cloud, running multi-tenant solutions across Azure IaaS, PaaS, and O365. Hybrid storage resource providers for Azure Stack, back when it was still called Windows Azure Pack. Cloud hydration with System Center DCS, doing data-driven multi-tier workload deployment through Azure Resource Manager and SCVMM.

The change here was altitude. At Honeywell I built applications. At Microsoft I built the thing other people built applications on. Those are different jobs. In platform work your users are engineers, your failure modes are other teams' outages, and your best decisions are the ones nobody ever notices. You also spend months arguing about abstractions, because the abstraction is the product.

<!-- TODO: Balaji, thirteen years is a long time. What were the two or three distinct eras inside it? Was Azure Stack the peak, or something else? What kept you there, and then what ended it? -->

## Google, 2018 to 2023: consulting, and documents again

Five years as a solutions architect. Customized Document AI processors for lending document types, and acting as a feedback loop back into product engineering on the document intelligence roadmap. Automated RFP response systems and pipeline analytics. Technical strategy and enablement for GSI partners across Data Analytics and AI/ML.

Two things were new. The first was that the work faced outward. I sat between the product team and the customer, translating what customers actually needed into something the product team could act on, and translating what the product could actually do into something a customer could plan around. I underestimated how different that is from engineering until I had to do it.

The second was the return to documents. Twenty years after the aircraft manuals I was back to pulling structure out of technical documents so a machine could act on it. The difference is that the structure now had to be inferred by a model instead of enforced by a DTD. In 1999 the discipline was upstream: authors wrote to a schema and the system could rely on it. With lending documents there is no schema and no compliance, just whatever the originator happened to send. Most of the gap between a model that scores well on a benchmark and a processor that survives real documents comes down to that.

<!-- TODO: Balaji, hardest Document AI customer problem? And what pulled you toward Onix? -->

## Onix, 2023 to now: building again, and the patents

AI/ML architect. Rapid prototypes carried through into production agentic workflows. Vision language models for legacy system interaction, which mostly means getting a model to operate software that has no API. Fine-tuned small language models for domain work. Agentic orchestration with ADK, LangGraph, and custom frameworks built on Airflow-inspired DAGs.

The retrieval thread shows up here as knowledge catalogs: getting enterprise data into a shape an autonomous system can reason over. Same problem as the parts catalog, three technology generations later. The thing being indexed changed. So did the consumer, from a mechanic to a model. The question stayed put: how do you make a large, messy, structured corpus addressable by something that has to act on it?

The three patents come out of this period and the cloud migration work around it. They share one observation. The individual capabilities all existed already, but nobody had automated the judgment in between them. Migration assessment tools could inventory an estate but could not decide the wave plan. Scanners could find vulnerabilities but could not predict what would break if you fixed them. Both times the missing piece was the reasoning step in the middle, and both times it turned out to be patentable because nobody had built it as one chain.

That habit, looking for the human judgment sitting between two automated steps, is the most portable thing I have picked up. It is also more or less what agentic systems are for.

<!-- TODO: Balaji, the patent origin stories. Who had the idea first? What did the first working version look like? Also worth saying: what does the agentic work look like day to day, and what do you think is overhyped about it? -->

## What carried over

None of the Wipro stack survives in what I do now. Neither does the Honeywell one. What survives is narrower and more useful than any technology.

Production discipline from industrial software, where a bug had the physical world downstream of it. Abstraction design from platform work, where the abstraction is the product. Translation from consulting.

And underneath all of it, one long argument with the same problem. How do you make a complicated body of information addressable by something that needs to act on it, whether that something is a mechanic holding a wrench or an agent holding a tool call.

<!-- TODO: Balaji, does this framing ring true or is it too neat? The retrieval thread connecting Wipro to Document AI to knowledge catalogs is my read, not something you told me. Say so if it is a stretch and I will drop it. Happy to make this messier if the real path was less linear. -->

---

<sub>Last updated August 2026. Working draft.</sub>
