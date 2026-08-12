[← back](../)

# Career notes

*Draft — v1. The factual arc is here; the parts worth actually reading are the ones only I can fill in. Marked below.*

---

Twenty-five years is long enough that the industry I started in and the one I work in now share very little vocabulary. What follows is less a career history than an attempt to name what actually changed at each stage, and what carried over.

## Honeywell — industrial software, and what "production" means

I started in refinery and oil enterprise software: production planning, production analysis, operations management. Dynamic cubes for production modeling, workflow automation for refinery planning. Remote automation products for plants that could not simply be restarted.

That last part is the thing that stuck. In industrial software, the cost of being wrong is not a rolled-back deploy — it is a process unit that has to be brought down. You learn to think about failure modes before features, and to treat "it works on my machine" as roughly meaningless. Everything I later found unremarkable about production discipline, I learned first in a context where the physical world was downstream of the code.

<!-- TODO: Balaji — what actually made you leave? Was there a specific project or a specific ceiling? Any story from the refinery work that still comes to mind? -->

## Microsoft — thirteen years, and the shift to platform

Thirteen years is the longest chapter, and it spans the industry's move to cloud almost exactly. Software engineering lead for Managed Services for Cloud, running multi-tenant solutions across Azure IaaS, PaaS, and O365. Hybrid storage resource providers for Azure Stack, back when it was still Windows Azure Pack. Cloud hydration with System Center DCS — data-driven, multi-tier workload deployment through Azure Resource Manager and SCVMM.

The change in this period was one of altitude. At Honeywell I built applications; at Microsoft I built the substrate other people built applications on. Those are genuinely different disciplines. Platform work means your users are engineers, your failure modes are other teams' outages, and your best design decisions are the ones nobody ever notices. It also means arguing about abstractions for months, because the abstraction is the product.

<!-- TODO: Balaji — thirteen years is a long time. What were the two or three distinct eras inside it? Was the Azure Stack work the peak, or something else? What made you stay that long, and then what made you go? -->

## Google — the consulting altitude, and Document AI

Four years as a solutions architect. Customized Document AI processors for lending document types, and acting as a feedback loop back into product engineering on the document intelligence roadmap. Automated RFP response systems and pipeline analytics. Technical strategy and enablement for GSI partners across Data Analytics and AI/ML.

This was the first stage where the work was primarily *outward-facing*. Not building the platform, not building on it, but sitting between the two — translating what customers actually needed into something the product team could act on, and translating the product's real capabilities into something a customer could plan around. It is a genuinely different skill from engineering, and I underestimated it before doing it.

It was also my first sustained exposure to ML systems in production rather than in demos, and specifically to the gap between a model that performs well on a benchmark and a processor that survives contact with real lending documents.

<!-- TODO: Balaji — the Document AI work: what was the hardest customer problem? And what did you learn about ML in production that surprised you? Also: what pulled you toward Onix? -->

## Onix — building again, and the patents

AI/ML architect since 2023. Rapid prototypes carried into production agentic workflows. Vision language models for legacy system interaction — getting a model to operate software that has no API. Fine-tuned small language models for domain-specific work. Agentic orchestration with ADK, LangGraph, and custom frameworks built on Airflow-inspired DAGs.

The three patents come from this period and the cloud migration work around it. The thread running through all of them is the same observation: the individual capabilities existed, but nobody had automated the *judgment between* them. Migration assessment tools could inventory an estate but not decide the wave plan. Scanners could find vulnerabilities but not predict what would break if you fixed them. In both cases the missing piece was the reasoning step in the middle, and in both cases that turned out to be patentable because nobody had built it as one chain.

That framing — look for the human judgment sitting between two automated steps — is the most portable thing I have learned. It is also, not coincidentally, what agentic systems are for.

<!-- TODO: Balaji — the patent origin stories. Who had the idea first? What did the first working version look like? Also worth saying: what does the agentic work look like day to day, and what do you think is overhyped about it? -->

## What carried over

Looking back, the through-line is not technology — none of the Honeywell stack survives in what I do now. It is the habit of treating the unglamorous middle as where the real problem lives. Production discipline from industrial software, abstraction design from platform work, translation from consulting, and now the automation of judgment itself.

<!-- TODO: Balaji — does this framing ring true, or is it too neat? Happy to make this messier and more honest if the real arc was less linear. -->

---

<sub>Last updated August 2026. This is a working draft.</sub>
