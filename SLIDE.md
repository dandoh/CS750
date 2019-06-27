layout: true

<img id="logo" src="images/logo.png" alt="McMaster Logo"/>

---

<div style="margin-top: 130px">
    <h1>
    Vector, covector, the exterior derivative and Hashed Expression
    </h1>
    <div class="horizontal-line"></div>
    <div class="flex-row" style="justify-content: flex-end; margin-right: 30px"> 
        <ul class="table-content">
            <li>Motivation</li>
            <li>Vector & covector</li>
            <li>The exterior derivative</li>
            <li>Hashed Expression</li>
        </ul>
    </div>
</div>

---

<div style="margin-top: 130px">
    <h1>
    Vector, covector, the exterior derivative and Hashed Expression
    </h1>
    <div class="horizontal-line"></div>
    <div class="flex-row" style="justify-content: flex-end; margin-right: 30px"> 
        <ul class="table-content">
            <li class="table-content-selected">Motivation</li>
            <li>Vector & covector</li>
            <li>The exterior derivative</li>
            <li>Hashed Expression</li>
        </ul>
    </div>
</div>

---

# Motivation

- Optimization problems
--

- The objective function 
--

<div>
    <img src="images/fxy.svg" alt="" style=""/>
</div>
--

- The gradient 
--

<div>
    <img src="images/dfx.svg" alt="" style=""/>
</div>

--
<div>
    <img src="images/dfy.svg" alt="" style=""/>
</div>

--
<div>
    <img src="images/gradf.svg" alt="" style=""/>
</div>

---

# Motivation
- Many sharing expressions
<div>
	<img src="images/sharing.svg" alt="" style="">
</div>
--

---

# Motivation
- Speedup opportunity
    - Recognize common expressions
    - Schedule evaluation
    
--

<div class="flex-row" style="justify-content: center">
	<img src="images/codegraph.svg" alt="" style="">
</div>

---

# Goals
- Encode expressions
    - Directed acyclic graph (DAG)
- Identify common sub-expressions
    - Hash
- Compute the derivatives (symbolically)

---

# Computing derivatives

- Gradient
<div>
    <img src="images/gradf.svg" alt="" style=""/>
</div>
    - Components separate, inefficient
    - How to interpret with multidimensional variables?

---

# Computing derivatives

- Implicit derivative
<div>
	<img src="images/df.svg" alt="" style="">
</div>
    - Directional derivatives


- Differential form (1-form)
<div>
	<img src="images/df.svg" alt="" style="">
</div>
<div>
	<img src="images/directional_derivative.svg" alt="" style="">
</div>


