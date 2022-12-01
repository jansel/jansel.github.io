---
layout: about
title: about
permalink: /
subtitle:

profile:
  align: right
  image: jasonansel4.jpg
  image_circular: false # crops the image to make it circular
  address:

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

I am currently working on [PyTorch] at Meta where I started the [TorchDynamo]
and [TorchInductor] projects, both of which are foundational parts of
[PyTorch 2.0].  TorchDynamo is a Python-level JIT compiler designed to
make unmodified PyTorch programs faster. TorchDynamo hooks into the frame
evaluation API in CPython (PEP 523) to dynamically modify Python bytecode
right before it is executed.  TorchInductor is a new compier backend for
TorchDynamo that maps arbitrary PyTorch programs to [Triton] or C++/OpenMP.

Before Meta, I was at GoDaddy helping build a deep learning platform
for predicting small business behavior and personalizing experiences across
the company.  I also created [GoDaddy Domain Appraisals], which uses neural
networks to predict the resale value of a domain name better than a human
expert.  I joined GoDaddy in 2013 as part of the [acquisition] of the startup
[Locu], which I joined in 2011 while I was simultaneously getting my Ph.D. at
[MIT][MIT] [CSAIL].

I did my Ph.D. dissertation in the [Commit] group lead by  [Saman Amarasinghe].
I started the [OpenTuner] project, an extensible framework for program
autotuning.  I also created the [PetaBricks] programming language, a language
that incorporates algorithmic choices to allow an integrated autotuner to
explore search spaces of program implementations.  As an undergraduate, I did
research with [Gene Cooperman] and helped create [DMTCP], a user-level
distributed checkpoint/restart system.


[GoDaddy Domain Appraisals]: https://www.godaddy.com/engineering/2019/07/26/domain-name-valuation/
[acquisition]: http://allthingsd.com/20130819/godaddy-acquires-merchant-finder-startup-locu-for-70-million/
[CSAIL]: http://www.csail.mit.edu/
[DMTCP]: http://dmtcp.sourceforge.net/
[Gene Cooperman]: http://www.ccs.neu.edu/home/gene/
[Locu]: http://locu.com/
[MIT]: http://www.mit.edu/
[OpenTuner]: http://opentuner.org/
[PetaBricks]: http://projects.csail.mit.edu/petabricks/
[Commit]: http://groups.csail.mit.edu/commit/
[Saman Amarasinghe]: http://people.csail.mit.edu/saman/
[PyTorch]: https://github.com/pytorch/pytorch/
[TorchDynamo]: https://pytorch.org/docs/master/dynamo/
[TorchInductor]:https://dev-discuss.pytorch.org/t/torchinductor-a-pytorch-native-compiler-with-define-by-run-ir-and-symbolic-shapes/747
[Triton]: https://github.com/openai/triton
[PyTorch 2.0]: https://pytorch.org/get-started/pytorch-2.0/
