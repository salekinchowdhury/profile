---
layout: single
title: "VerilogA Day 01: Resistor"
date: 2024-10-24
author: "Shirazush Salekin Chowdhury"
permalink: /blogs/VerilogA_Day01_Resistor/
excerpt: "In this post, we'll dive into Verilog-A modeling for resistors and explore some basic circuits."
---

## Verilog-A Modeling for Resistors

In this post, we'll explore how to model resistors using Verilog-A. The first step is to understand the syntax.

### Basic Resistor Example

Here is the Verilog-A code for a simple resistor:

```verilog
module resistor(p, n);
   electrical p, n;
   parameter real r = 1k;
   analog V(p, n) <+ r * I(p, n);
endmodule
