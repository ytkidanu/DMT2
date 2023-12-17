![image](https://github.com/ytkidanu/DMT2/assets/123510145/1183fcb3-afb9-4fdb-8830-9c310cdf75d2)# DEFINING INPUT AND OUTPUT dfkugjgs

<img width="742" alt="Screen Shot 2023-12-16 at 7 51 03 PM" src="https://github.com/ytkidanu/DMT2/assets/123510145/f059a74a-0fd1-434e-bc77-c8431507a13d">

### INPUT:
Inputs are the things we compute on. An **Alphabet** is a finite set of characters. **Strings** are built up from an **Alphabet** 

Notation: 
**Σ (\Sigma in LaTeX)**

Examples:\
Σ={0,1}\
Σ={𝑎,𝑏,𝑐,𝑑,…,𝑧}\
Σ={0,1,2,…,9}

If:
Σ={0,1,𝑎,𝑏,𝑐}

Valid Strings:\
00abc10\
cccccc\
a11

We can define structure of a string in various ways. 

Examples:\
**_Σ^𝑛_** = The set of all length n strings over alphabet Σ\
{0,1}^3


The set of 3-bit strings.\
{0,1}^3={(𝑥_0,𝑥_1,𝑥_2  )
:𝑥_0,𝑥_1,𝑥_2∈{0,1}}\  
{0,1}^3={000,001,010,011,100,101,110,111}

So our alphabet id (0,1) and our n is 3, so we are trying to find every possible combination of 0 and 1 that is 3 in length

Pop Quiz: If |Σ|=𝑚, then |Σ^𝑛 |=? 
    
    m^n . In our previous example, m = 2 and n=3. m^3 =8, and we also found 8 possible combinations
    
**" * "** - operator refers to a string of any length, including 0. \
Σ^∗ = The set of all strings over alphabet Σ of any length (including 0)

{0,1}^∗
{0,1}^∗={(𝑥_0,𝑥_1,…,𝑥_(𝑛−1)  )  :𝑛∈"ℕ, " 𝑥_0,…,𝑥_(𝑛−1)∈{0,1}}  
{0,1}^∗={””, 0, 1, 00, 01, 10, 11, 000, 001,…}


<img width="310" alt="Screen Shot 2023-12-16 at 7 50 19 PM" src="https://github.com/ytkidanu/DMT2/assets/123510145/6f4792b7-8ae9-4ec6-968f-b3c8fb8b10e1">

---
### Defining Computation

Definition of computation is based on functions; A function 𝑓 is computable under a computing model if:
 

That model allows for an implementation (way of filling in the black box) such that,
For any input 𝑥∈𝐷 (string representing an element from the domain of 𝑓)
The implementation “produces” the correct output

	all inputs must be a part of 𝑓 and the inplenetation has to be correct
    
_Function_: a “mapping” from input to output (𝑓:𝐷→𝐶)

Function 𝑓 maps elements from the set 𝐷 to an element from the set 𝐶\
𝐷: the domain of 𝑓\
𝐶: the co-domain of 𝑓\
Range/image of 𝑓: {𝑓(𝑑):𝑑∈𝐷}\
The elements of 𝐶 that are “mapped to” by something

	The Codomain is the set of all possible values which can come out as a result, but the range is the set of values that actually comes out.

_Finite_ function: a function with a finite domain

	𝑓:𝐷→𝐶 is a finite function if 𝐷 is finite. Otherwise it’s an infinite function
   
**Injective Functions**\
<img width="98" alt="image" src="https://github.com/ytkidanu/DMT2/assets/123510145/1f2e29ba-9370-4c6a-8612-2f3468a30ebc">

One-to-one (injective)\
𝑥≠𝑦⇒𝑓(𝑥)≠𝑓(𝑦)\
Different inputs yield different outputs\
_No two inputs share an output_

	
    a function that maps distinct elements of its domain to distinct elements of its codomain. Formally, it is stated as, if f(x) = f(y) implies x=y, then f is one-to-one mapped, or f is 1-1

**Surjective (onto) Functions**\
<img width="792" alt="image" src="https://github.com/ytkidanu/DMT2/assets/123510145/1b131086-ec1e-4ff2-85a9-68e07b97a712">

∀𝑐∈𝐶, ∃𝑑∈𝐷 :𝑓(𝑑)=𝑐

Everything in 𝐶 is the output of something in 𝑑\
Everything in Co-Domain “receives” something
	
     function f such that, for every element y of the function's codomain, there exists at least one element x in the domain. 


**One-to-one Correspondence (bijective)**\
<img width="336" alt="image" src="https://github.com/ytkidanu/DMT2/assets/123510145/eab43a96-46e0-428f-ac8f-89509c45765c">

Both injective and surjective\
Everything in 𝐶 is mapped to by a unique element in 𝐷\
All elements from domain and co-domain are perfectly “partnered”

Because Onto( surjective):\
Everything in Co-Domain “receives” something

Because 1-1:\
Nothing in Co-Domain “receives” two things

**Conclusion:
Things in the Domain _exactly_ “partner” with things in Co-Domain**

<img width="98" alt="image" src="https://github.com/ytkidanu/DMT2/assets/123510145/b712e569-0ab0-45d0-8c28-f5e5443249d0">

### Overview of Computation!

**Input / Output are Strings and a
Computing Machine is something that implements a set of functions that we care about.**

