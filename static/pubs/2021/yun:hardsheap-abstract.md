Secure allocators have been extensively studied to mitigate heap
vulnerabilities. They employ safe designs and randomized mechanisms to stop or
mitigate heap exploitation. Despite extensive research efforts, secure
allocators can only be evaluated by with theoretical analysis or pre-defined
data sets, which are insufficient to effectively reflect powerful adversaries in
the real world.

In this paper, we present HardsHeap, an automatic tool for evaluating secure
allocators. The key idea of HardsHeap is to use random testing (i.e., fuzzing)
to evaluate secure allocators. To handle the diverse properties of secure
allocators, HardsHeap supports an extensible framework, making it easy to write
a validation logic for each property. Moreover, HardsHeap employs sampling-based
testing, which enables us to evaluate a probabilistic mechanism prevalent in
secure allocators. To eliminate redundancy in findings from HardsHeap, we devise
a new technique called Statistical Significance Delta Debugging (SSDD), which
extends the existing delta debugging for stochastically reproducible test cases.

We evaluated HardsHeap to 10 secure allocators. Consequently, we found 56
interesting test cases, including several unsecure yet underestimated behaviors
for handling large objects in secure allocators. Moreover, we discovered 10
implementation bugs. One of the bugs is integer overflow in secure allocators,
making them even more invulnerable than ordinary allocators. Our evaluation also
shows that SSDD successfully reduces test cases by 37.2% on average without a
loss of reproducibility.
