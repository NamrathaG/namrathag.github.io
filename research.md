---
layout: page
title: Research
permalink: /research/
---

<style>
.research-entry {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 0.3rem;
}

.research-title {
  font-size: 1.15rem;
  font-weight: 600;
}

.research-date {
  font-size: 0.95rem;
  color: #555;
  white-space: nowrap;
}

.research-details {
  margin: 0 0 1.5rem 0;
}

.research-meta {
  margin-bottom: 0.6rem;
}

.research-abstract {
  margin-top: 0.6rem;
  line-height: 1.6;
}

.research-abstract ul {
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}

.research-links {
  margin-top: 0.8rem;
}

.research-links a {
  margin-right: 16px;
  font-size: 0.95rem;
}
</style>

<div class="research-entry">
  <div class="research-title">Reduction for Structured Concurrent Programs</div>
  <div class="research-date">January 2026</div>
</div>

<div class="research-details">

  <div class="research-meta">
    <em>To appear at ESOP 2026</em><br>
    <strong>Authors:</strong> Namratha Gangamreddypalli, Constantin Enea, Shaz Qadeer
  </div>

  <div class="research-abstract">
    <strong>Abstract.</strong>
    Commutativity reasoning based on Lipton's movers is a powerful technique for verification of concurrent programs.
    The idea is to define a program transformation that preserves a subset of the initial set of interleavings,
    which is sound modulo reorderings of commutative actions.
    Scaling commutativity reasoning to routinely-used features in software systems,
    such as procedures and parallel composition, remains a significant challenge.

    In this work, we introduce a novel reduction technique for structured concurrent programs that unifies two key advances:
    
    <ul>
      <li>We present a reduction strategy that soundly replaces parallel composition with sequential composition.</li>
      <li>We generalize Lipton’s reduction to support atomic sections containing (potentially recursive) procedure calls.</li>
    </ul>

    Crucially, these two foundational strategies can be composed arbitrarily, greatly expanding the scope and flexibility of reduction-based reasoning.
    We implemented this technique in Civl and demonstrated its effectiveness on a number of challenging case studies,
    including a snapshot object, a fault-tolerant and linearizable register, the FLASH cache coherence protocol,
    and a non-trivial variant of Two-Phase Commit.
  </div>

  <div class="research-links">
    <a href="https://arxiv.org/abs/2601.13341">arXiv</a>
    <a href="https://arxiv.org/pdf/2601.13341.pdf">PDF</a>
    <a href="https://doi.org/10.48550/arXiv.2601.13341">DOI</a>
  </div>

</div>