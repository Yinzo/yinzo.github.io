---
title: "Note for <Thesis - Behavior of Machine Learning Algorithms in Adversarial Environments.pdf>(1)"
date: 2016-02-04T16:55:00+08:00
draft: false
toc: false
images:
tags: 
  - untagged
---
# Note for "Thesis - Behavior of Machine Learning Algorithms in Adversarial Environments.pdf"(1)

<div class="read-more clearfix">
<span class="date">2016/2/4 16:55 下午</span>
<span>posted in&nbsp;</span>
<span class="posted-in"><a href="Adversary%20Learning.html">Adversary Learning</a></span>
<span class="comments">
</span>
</div>
<h2 id="toc_0">1.1 Motivation and Methodology</h2>

<h4 id="toc_1">Learning approach is well-suited to the scenario when:</h4>

1.   The process is too complex to designed for human operator
2.   Requirement of dynamical development

<span id="more"></span><!-- more -->

<h4 id="toc_2">An intelligent adversary can:</h4>

*   Alter his approach based on knowledge of the learner’s shortcomings
*   Mislead it by cleverly crafting data to corrupt 
*   Deceive the learning process

<h4 id="toc_3">Potential dangers posed to a learning system:</h4>

*   An attacker can exploit the nature of a machine learning system to mis-train it and cause it to fail

<h4 id="toc_4">The questions raised by author:</h4>

*   What techniques can a patient adversary use to mis-train or evade a learning system?
*   How can system designers assess the vulnerability of their system to vigilantly incorporate trustworthy learning methods?

<h4 id="toc_5">An algorithm’s performance depends on:</h4>

*   The constraints placed on the adversary
*   The job the algorithm is tasked with performing

This raises two fundamental questions:

*   How can we evaluate a learner’s performance in adversarial environment?
*   How to design or select a learner which can be satisfied for its performance in particular environment?

<h3 id="toc_6">Example 1.1</h3>

<h4 id="toc_7">How spammer corrupt the learning mechanism:</h4>

1.   use information about the email distribution to construct clever attack spam messages
2.   will cause the spam filter to misclassify the user’s desired messages as spam.
3.   to cause the filter to become so unreliable

<h3 id="toc_8">Example 1.2</h3>

<h4 id="toc_9">The ANTIDOTE’s feature:</h4>

*   Better resistance within the poisoned environment
*   But Less effective on non-poisoned environment

<h3 id="toc_10">Example 1.3</h3>

<h4 id="toc_11">The means to evade the filter:</h4>

*   obfuscating words indicative of spam to human-recognizable misspellings; e.g., “Viagra” to“V1@gra” or “Cialis” to “Gia|is”
*   using clever HTML to make the content difficult to parse 
*   adding words or text from other sources unrelated to the spam
*   embedding images that contains the spam message.

<h2 id="toc_12">1.2 Guidelines from Computer Security</h2>

<h4 id="toc_13">Author’s principles:</h4>

*   Proactively Analysis
*   Kerckhoffs’ Principle
*   Conservative Design
*   Threat Modeling

<h3 id="toc_14">Proactive Analysis:</h3>

Proactively find the vulnerabilities of learning system before the it is deployed or widely used.

<h3 id="toc_15">Kerckhoffs' Principle:</h3>

Do not let a system’s security rely on secrets. If the secrets are exposed, the system is immediately compromised.

So apply this principle into machine learning, we should assume the adversary is aware of the learning algorithm and can obtain some data used to train the model.

<h3 id="toc_16">Conservative Design:</h3>

When access the security of a system, we should avoid to put limit on adversary’s behavior. We should assume that the adversary has the broadest possible powers.

Conversely, though the adversary too powerfully may lead to an inappropriate assessment on the system.

<h3 id="toc_17">Threat Modeling:</h3>

A completely secure system is infeasible. So author qualified the systems with _degree of security_ -—the level of security expected against an adversary based on a _threat model_ with a certain set of:

*   objectives 
*   capabilities
*   incentives

<h4 id="toc_18">To construct a threat model for a particular learning system:</h4>

1.   Quantifies the security setting and objectives of that system, to develop criteria to measure success and quantify the level of security offered.
2.   Formalizing the risks and objectives, to identify potential limitations of the system and potential attacks.
3.   Identifies potential adversarial goals, resources and limitations.

<h4 id="toc_19">To evaluating a system:</h4>

1.   Determining classed of attacks on the system.
2.   Evaluating the resilience of the system against those attacks
3.   Strengthening the system against those classes of attacks.

<h2 id="toc_20">1.3 Historical Roadmap</h2>

Some experience of author when developing this thesis, seems irrelevant to the mainstream.

<h2 id="toc_21">1.4 Dissertation Organization</h2>

As the title, no useful informations.