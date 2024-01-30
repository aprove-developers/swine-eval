<head>
    <title>SwInE</title>
    <style>
        p {text-align: justify;}
    </style>
</head>

This is the evaluation of the technique from our paper "Satisfiability Modulo Exponential Integer Arithmetic", which is implemented in our SMT solver SwInE (**S**MT **w**ith **In**teger **E**xponentiation). For more information abot SwInE, we refer to its [website](https://ffrohn.github.io/swine/).

# Downloading SwInE

[Here](https://github.com/ffrohn/swine/releases) you can find the latests releases of SwInE.

# Input Format

SwInE supports an extension of the [SMTLIB-format](https://smtlib.cs.uiowa.edu/) with an additional binary function symbol `exp`, whose arguments have to be of sort `Int`.
By default, the semantics of `exp(s,t)` is s<sup>|t|</sup>.
Alternatively, SwInE supports *partial semantics* where `exp(s,t)` is treated like an uninterpreted function if `t` is negative.

# Using SwInE

Please execute `swine --help` for detailed information on using SwInE.

# Benchmarks

You can find the benchmarks from our evaluation [here](https://github.com/ffrohn/QF_EIA).
Moreover, you can download [our leading example](leading.smt2), and [Example 21](ex21.smt2) from our paper.

# Detailed Results

<a href="results.html">Here</a>, we provide a table with detailed results of our evaluation.
