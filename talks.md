---
layout: page
title: Talks
permalink: /talks/
---

<style>
.talk-entry {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 0.2rem;
}
.talk-title {
  font-size: 1.1rem;
  font-weight: 600;
}
.talk-date {
  font-size: 0.95rem;
  color: #555;
  white-space: nowrap;
}
.talk-details {
  margin: 0 0 1.2rem 0;
}
</style>

<!-- ================= TALK 1: VTSA 2025 (LATEST) ================= -->

<div class="talk-entry">
  <div class="talk-title">Reduction for Structured Concurrent Programs</div>
  <div class="talk-date">Sept 2025</div>
</div>

<div class="talk-details">
  <strong>
    <a href="https://resources.mpi-inf.mpg.de/departments/rg1/conferences/vtsa25/" target="_blank">
      Summer School on Verification Technology, Systems & Applications (VTSA) 2025
    </a>
  </strong><br>
  University of Liège, Belgium<br><br>

  <strong>Abstract:</strong><br>
  Commutativity reasoning based on Lipton's movers is a powerful technique for verification of concurrent
  programs. The idea is to define a program transformation that preserves a subset of the initial set
  of interleavings, which is sound modulo reorderings of commutative actions. Scaling commutativity
  reasoning to routinely used features in software systems, such as procedures and dynamic thread
  creation, remains a significant challenge.<br><br>

  In this work, we introduce a novel reduction technique for structured concurrent programs that unifies
  two key advances. First, we present a reduction strategy that soundly replaces thread forking and
  joining with sequential composition. Second, we generalize Lipton’s reduction to support atomic
  sections containing (potentially recursive) procedure calls. Crucially, these two foundational
  strategies can be composed arbitrarily, greatly expanding the scope and flexibility of reduction-based
  reasoning.<br><br>

  We implemented this technique in Civl and demonstrated its effectiveness on a number of challenging
  case studies, including a snapshot object, a fault-tolerant and linearizable register, the FLASH cache
  coherence protocol, and a non-trivial variant of Two-Phase Commit.

  I demonstrate this technique using an implementation of a concurrent snapshot object, which aims to
  return a consistent view of memory despite concurrent updates.
</div>

<hr>

<!-- ================= TALK 2: VDS 2025 ================= -->

<div class="talk-entry">
  <div class="talk-title">Commutativity Based Refinement Proofs Using Civl</div>
  <div class="talk-date">May 2025</div>
</div>

<div class="talk-details">
  <strong>
    <a href="https://netys.net/wds2025/VDS25.html" target="_blank">
      Workshop on Verification of Distributed Systems (VDS) 2025
    </a>
  </strong><br>
  Rabat, Morocco<br><br>

  <strong>Abstract:</strong><br>
  Civl is a static verifier for concurrent programs based on the idea of layered refinement.
  A program at a lower layer (such as a concrete, low-level implementation) refines a program at a
  higher layer (such as a high-level specification) in such a way that proving correctness of the
  higher layer implies proving correctness of the lower layer.
  One form of refinement is reducing the space of possible executions of a concurrent program.
  This can be achieved by exploiting the commutativity of statements, defined as movers in Lipton's
  reduction. A statement is a left (right) mover if it can be commuted to the left (right) of every
  other statement executed by a different thread, without altering the outcome of the execution.
  I describe a new refinement proof rule based on commutativity and use it to prove correctness of a
  snapshot algorithm. The goal of the algorithm is to return a snapshot of the entire memory, despite
  concurrent updates to different locations.
</div>

<hr>
