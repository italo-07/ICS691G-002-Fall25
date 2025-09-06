# [Formally Verified Cloud-Scale Authorization](https://assets.amazon.science/bb/40/22ac44f84f6d8eb625ac9666a00f/formally-verified-cloud-scale-authorization.pdf)
> ICSE 2025

## Summary
This paper describes a real-world example of implementing a production service 
at scale, AWS's authentication engine, using [Dafny](https://github.com/dafny-lang/dafny), 
a formally verified language. 

A formally verified language can generate traditional code that is formally 
guaranteed to execute exactly as described, using proofs and theorem provers 
to generate proofs of correctness. The AWS authv1 engine was written in Java and 
the would be maintainers of the authv2 engine are traditional Java developers,
which introduced the additional constraint that the `dafny` compiler must 
generate idiomatic Java code such that a Java developer could still understand 
the code. 

This is a significant development in the field of formal methods as it demonstrates 
the development and deployment of critical services can be done with a formally 
verified language at scale and with minimal friction with non-formally trained 
developers. 
