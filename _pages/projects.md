---
layout: page
title: projects
permalink: /projects/
description: A partial list of projects I have worked on.
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---

## TorchDynamo

I started the [TorchDynamo] project, which is now part of [PyTorch 2.0].
TorchDynamo is a Python-level JIT compiler designed to make unmodified
PyTorch programs faster. TorchDynamo hooks into the frame evaluation API
in CPython (PEP 523) to dynamically modify Python bytecode right before it
is executed. It rewrites Python bytecode in order to extract sequences of
PyTorch operations into an FX Graph which is then just-in-time compiled with
a customizable backend. It creates this FX Graph through bytecode analysis
and is designed to mix Python execution with compiled backends to get the
best of both worlds: usability and performance.

[TorchDynamo]: https://pytorch.org/docs/master/dynamo/
[PyTorch]: https://github.com/pytorch/pytorch/
[PyTorch 2.0]: https://pytorch.org/get-started/pytorch-2.0/

## TorchInductor

I started the [TorchInductor] project, which is now part of [PyTorch 2.0].
TorchInductor is a new compiler backend for PyTorch.  TorchInductor took
inspiration from how PyTorch users were writing high performance custom kernels:
increasingly using the [Triton] language.  We also wanted a compiler backend that
used similar abstractions to PyTorch eager, and was general purpose enough
to support the wide breadth of features in PyTorch.  TorchInductor uses a
pythonic define-by-run loop level IR to automatically map PyTorch models into
generated Triton code on GPUs and C++/OpenMP on CPUs.  TorchInductor’s core
loop level IR contains only ~50 operators, and it is implemented in Python,
making it easily hackable and extensible.

[TorchInductor]: https://dev-discuss.pytorch.org/t/torchinductor-a-pytorch-native-compiler-with-define-by-run-ir-and-symbolic-shapes/747
[Triton]: https://github.com/openai/triton

## GoDaddy Domain Appraisals

While at GoDaddy, I created a system that uses neural networks to predict the
resale price of a domain name in the aftermarket.  GoDaddy Domain Appraisals
(GoValue) is available to millions of GoDaddy customers and provides estimated
values to help both buyers and sellers more effectively price domain names.
GoValue is 1.25x better at predicting past domain name sale prices than
human experts.  You can [try it yourself], [learn how it works], or listen
to me [talk about it on a podcast].

[try it yourself]: https://www.godaddy.com/domain-value-appraisal
[learn how it works]: https://www.godaddy.com/engineering/2019/07/26/domain-name-valuation/
[talk about it on a podcast]: https://blogs.nvidia.com/blog/2018/03/08/ai-podcast-godaddy-ai-to-domains/
[research paper]: https://arxiv.org/abs/1806.11222

## Google Native Client

While interning at Google in 2010, I added support for sandboxing
self-modifying code to Native Client (part of Google Chrome) to support
dynamic language runtimes and JIT compilers. Native Client is a sandbox
for running untrusted machine code in the web browser.  We
[published this work in PLDI](http://groups.csail.mit.edu/commit/papers/2011/ansel-pldi11-nacljit.pdf).

## OpenTuner

[OpenTuner] is an open-source framework building domain-specific
multi-objective program autotuners.  OpenTuner supports customizable
configuration representations, an extensible technique representation
to allow for domain-specific techniques, and an easy to use interface for
communicating with the tuned program.  I was the primary author and original
creator of this project.

## PetaBricks
[PetaBricks] is a language and compiler where algorithmic choices are
exposed explicitly to create programs that define a search space of possible
algorithms.  The PetaBricks compiler then uses empirical autotuning to search
over these algorithms for an optimal version.  I was the primary author and
original creator of this project.


## Kendo
[Kendo] is a library that allows multithreaded programs,
that would normally produce non-deterministic output, to execute
deterministically by enforcing a dynamically computed and efficient
ordering of lock acquisitions.  The primary author of this work is
[Marek Olszewski](https://www.linkedin.com/in/marekolszewski/).


## DMTCP
[DMTCP][DMTCP] (Distributed Multi-Threaded Checkpointing) is a tool to
transparently checkpoint and restart the state of a distributed cluster
computation that communicates through MPI or sockets.  It works on unmodified
binaries at the user level.  I was the first author on the original DMTCP
paper and designed and implemented the distributed component that converted a
single-process checkpointer into a distributed checkpointer. 
I have moved on from this project, but it is continued by
many wonderful researchers, and there are now [100+ refereed
publications](http://dmtcp.sourceforge.net/publications.html) using or
extending DMTCP.

## Algorithmic Trading on LendingClub.com

Starting in 2012 I also did algorithmic trading on the secondary market of
the peer-to-peer lending platform [LendingClub]. I used neural networks to
predict the likelihood of default of specific loans, and then both buy and
sell notes based on those predictions.  LendingClub has since shut down,
but I enjoyed this side project.


[LendingClub]: https://lendingclub.com/
[GitHub Page]: https://github.com/jansel
[ShowDB]: https://github.com/jansel/showdb
[LendingClubChecker]: https://github.com/jansel/lendingclubchecker
[OpenTuner]: http://opentuner.org/
[PetaBricks]: http://projects.csail.mit.edu/petabricks/
[Kendo]: http://projects.csail.mit.edu/kendo/
[DMTCP]: http://dmtcp.sourceforge.net/

