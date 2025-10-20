# **LANGTRAJ**

**Diffusion Model and Dataset for Language‑Conditioned Trajectory Simulation**

This repository is the official implementation of **LangTraj: Diffusion Model and Dataset for Language‑Conditioned Trajectory Simulation**.

> **LangTraj: Diffusion Model and Dataset for Language‑Conditioned Trajectory Simulation**

> [Wei‑Jer Chang](https://scholar.google.com/citations?user=tF-OmYgAAAAJ&hl=en)1, [Wei Zhan](https://zhanwei.site/)1, [Masayoshi Tomizuka](https://me.berkeley.edu/people/masayoshi-tomizuka/)1, [Manmohan Chandraker](https://cseweb.ucsd.edu/~mkchan)2,3, [Francesco Pittaluga](https://www.francescopittaluga.com/)2

> 1 University of California, Berkeley · 2 NEC Labs America · 3 University of California, San Diego

Evaluating autonomous vehicles with controllability enables scalable testing in counterfactual or structured settings, enhancing both efficiency and safety. We introduce **LangTraj**, a language‑conditioned scene‑diffusion model that simulates the joint behavior of all agents in traffic scenarios. By conditioning on natural language inputs, LangTraj provides flexible and intuitive control over interactive behaviors, generating nuanced and realistic scenarios. Unlike prior approaches that depend on domain‑specific guidance functions, LangTraj incorporates language conditioning during training, facilitating more intuitive traffic simulation control. We propose a novel closed‑loop training strategy for diffusion models, explicitly tailored to enhance stability and realism during closed‑loop simulation. To support language‑conditioned simulation, we develop **Inter‑Drive**, a large‑scale dataset with diverse and interactive labels for training language‑conditioned diffusion models. Our dataset is built upon a scalable pipeline for annotating agent‑agent interactions and single‑agent behaviors, ensuring rich and varied supervision. Validated on the Waymo Open Motion Dataset, LangTraj demonstrates strong performance in realism, language controllability, and language‑conditioned safety‑critical simulation, establishing a new paradigm for flexible and scalable autonomous vehicle testing.

## **News**

* [2025.07] Paper accepted by ICCV 2025!
* [2025.10.20] Example annotations of Inter‑Drive released.
* [2025.11.07 | ETA] Initial version of Inter‑Drive inference code release.
* [2025.11 | ETA] Inter‑Drive dataset release (delayed due to company IP review).

Please stay tuned for further updates!


