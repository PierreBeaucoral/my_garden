---
{"dg-publish":true,"permalink":"/miscellaneous-thoughts/"}
---

## About AI 

I’m currently attending an AI conference geared toward engineers and researchers, and today one of the hardware vendors gave a live demo of their latest GPU setup’s ability to generate deepfakes in real time. Watching a “realistic” face swap unfold seamlessly on stage was impressive from a pure performance standpoint—but it also hit me like a jolt of cold water.

On one hand, it’s exciting: faster inference means new possibilities for creative AI, medical imaging, and complex simulations. But on the other hand, the very same throughput that makes harmless applications slick can be used maliciously. A handful of lines of code and a powerful board can conjure an almost indistinguishable video of anyone saying—or doing—anything.

As a geek, I respect the ingenuity involved: optimizing models down to the metal, pushing hardware limits, and shaving milliseconds off frame-by-frame processing. But as a researcher and as a member of a broader society that isn’t always prepared for the dark side of innovation, I can’t ignore the risks. Deepfakes are already circulating in political contexts, fueling disinformation campaigns. Tomorrow, we’ll see them used to manipulate financial markets, smear reputations, or perpetuate fraud in ways we haven’t yet imagined.

Today’s demo made me think hard about the responsibility we bear: to design safeguards, to build detection tools that keep pace, and to advocate for transparent, accountable deployment. If these hardware breakthroughs simply usher in a new wave of undetectable fakes—without proper regulation or ethics baked in—we’ll lose the public’s trust in digital media faster than we can say “real-time rendering.”

So yes, I’m thrilled by the technical strides on display here—every drop in latency and surge in throughput is a testament to human ingenuity. But I’m equally concerned about how we channel that power. As engineers and researchers, our next challenge isn’t just maximizing performance but ensuring that AI remains a tool for positive progress, not a loophole for deception.

> PS: I am still a huge user of it, for coding it is my go to debugging 

--- 
### **How I Got Hooked on Causality**

I never expected that a course would fundamentally reshape how I think about evidence in economics. But that’s exactly what happened when I took a class from **Martin Huber**. Before that, I understood regression, correlation, and even some applied econometrics—but I hadn’t truly grasped the _difference between correlation and causation_ in a deep, operational sense.

Huber’s course made me pause. It wasn’t just about running regressions; it was about asking sharper questions: **What is the effect of X on Y, really?** And crucially, _how can we be sure_? That line of thinking led me down a rabbit hole—from treatment effects to identification assumptions, and finally to the emerging role of **machine learning (ML)** in causal inference.

This post is a personal reflection on what I’ve learned, why causal thinking matters in economics, and how machine learning can be a powerful ally—_if we use it wisely_.

---

### **What Is Causal Inference?**

>Causal inference asks “what if” questions: What would have happened to someone if they hadn’t received a treatment? This is central to economics, where we care about the _effects_ of policies, institutions, and behaviors—not just their associations.

Since we can't observe counterfactual outcomes directly, economists rely on **identification strategies** to estimate them. Some foundational tools include:

- **Randomized Controlled Trials (RCTs)**
- **Difference-in-Differences (DiD)**
- **Instrumental Variables (IV)**
- **Regression Discontinuity (RD)**
- **Propensity Score Matching (PSM)**

For beginners or practitioners, Angrist & Pischke’s _Mastering ‘Metrics_ is an essential starting point. It doesn’t just explain techniques—it teaches the logic behind them.

---

### **What Makes a Causal Claim Credible?**

To truly infer causality, certain conditions must hold:

1. **Unconfoundedness** – No omitted variable bias, once we condition on observables.
2. **Overlap** – Treated and untreated units must be comparable.
3. **Exogeneity (for IVs)** – The instrument must influence the outcome only through treatment.
4. **Stable Unit Treatment Value Assumption (SUTVA)** – One unit's treatment doesn't affect another’s outcome.

These assumptions are what economists obsess over—not because we're perfectionists, but because without them, causal claims become wishful thinking.

### **Where Machine Learning Fits In**

Machine learning wasn’t built for causal inference. It was designed to **predict** well, not to uncover _why_ something happens. That said, ML can enhance causal work when applied with care.

#### **Controlling for Many Covariates**

In high-dimensional settings (e.g., many potential confounders), traditional models break down. ML methods like **LASSO**, **Random Forests**, or **Gradient Boosting** can select relevant variables more effectively than manual methods.

#### **Uncovering Treatment Effect Heterogeneity**

Not everyone responds to a treatment in the same way. ML models like **Causal Forests** ([Wager & Athey, 2018](https://arxiv.org/abs/1510.04342)) or **meta-learners** (T-, S-, and X-learners) can estimate **individualized treatment effects**, telling us who benefits most.

#### **Double Machine Learning (DML)**

Proposed by [Chernozhukov et al. (2018)](https://academic.oup.com/ectj/article-abstract/21/1/C1/5056401?redirectedFrom=fulltext), DML is a framework that uses ML to control for confounding, but preserves valid statistical inference by using orthogonalization and sample splitting. It combines flexibility with the structure economists demand.

#### **Improving Propensity Score Estimation**

Propensity scores estimate the likelihood of treatment given covariates. ML can generate more accurate scores, leading to better balancing between treated and control groups.

---

### **The Lesson I Took Away**

Martin Huber’s course didn’t just teach me methods. It "resettled" my instincts as an economist. Today, I don’t look at an estimate and ask only, _“Is it significant?”_—I ask, _“Is it causal?”_ and _“Is the identification strategy solid?”_

Machine learning is a tool—_not a shortcut_. It’s most useful when integrated into a framework built on clear assumptions and theory. Used correctly, ML helps us move faster and see deeper patterns. But it must always serve the **causal question**, not override it.

---

### **Where to Learn More**

If this perspective resonates with you, here are some great resources that helped me on my journey:

- **Martin Huber’s Research & Teaching**: University of Lucerne Profile
- **Angrist & Pischke** – _Mastering ‘Metrics_
- **Chernozhukov et al. (2018)** – Double Machine Learning:  
     [Chernozhukov et al. (2018)](https://academic.oup.com/ectj/article-abstract/21/1/C1/5056401?redirectedFrom=fulltext)
- **Wager & Athey (2018)** :  
    [Wager & Athey, 2018](https://arxiv.org/abs/1510.04342)
- **EconML (Microsoft)** – [https://github.com/microsoft/EconML](https://github.com/microsoft/EconML)
- **DoubleML (Python package)** – [https://github.com/DoubleML/doubleml-for-py](https://docs.doubleml.org/stable/index.html)

---

### **Conclusion**

Causal inference is hard. But it’s what makes economics useful. With the right mindset and tools—traditional or machine-learned—we can ask better questions and give better answers. It’s not about what’s new and shiny; it’s about what’s _credible_.

And that’s the biggest thing I’ve taken from this journey: never confuse _predictive power_ for _causal insight_. Always be skeptical—but curious.
