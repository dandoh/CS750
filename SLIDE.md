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
    - Components separate
    - How to reason with multidimensional variables?

---

# Computing derivatives

- Implicit derivative
<div>
	<img src="images/df.svg" alt="" style="">
</div>
    - Infinitesimal change
    - Directional derivatives?


- Differential form (1-form)
<div>
	<img src="images/df.svg" alt="" style="">
</div>
<div>
	<img src="images/directional_derivative.svg" alt="" style="">
</div>


---

<div style="margin-top: 130px">
    <h1>
    Vector, covector, the exterior derivative and Hashed Expression
    </h1>
    <div class="horizontal-line"></div>
    <div class="flex-row" style="justify-content: flex-end; margin-right: 30px"> 
        <ul class="table-content">
            <li>Motivation</li>
            <li class="table-content-selected">Vector & covector</li>
            <li>The exterior derivative</li>
            <li>Hashed Expression</li>
        </ul>
    </div>
</div>

---

# Vector

- Element of a vector space
<div>
    <img src="images/vector_space.svg" alt="" style="">
</div>

- Basis
<div>
    <img src="images/basis.svg" alt="" style="">
</div>

- Vector components
<div>
    <img src="images/vector_components.svg" alt="" style="">
</div>
    

---

# Vector
- Vector components
<div>
    <img src="images/vector_components_column.svg" alt="" style="">
</div>


--
<div class="flex-row" style="justify-content: center">
	<img src="images/vector_draw.svg" alt="" style="">
</div>

---

# Covector
- Linear functional on vectors
<div>
    <img src="images/alpha_VS.svg" alt="" style="">
</div>
<div>
    <img src="images/linear_covector.svg" alt="" style="">
</div>
- Examples
<div>
    <img src="images/example_covectors.svg" alt="" style="">
</div>

---

# Covector
- Function
- Levels set
<div class="flex-row" style="justify-content: center;">
	<img src="images/covector_draw.svg" alt="" style="">
</div>


---

# Covector 

- Apply to a vector
<div class="flex-row" style="justify-content: center;">
	<img src="images/compute_function.svg" alt="" style="">
</div>
- The changing of value following the vector


---

# Covector
- The dual space
<div>
    <img src="images/dual_vector_space.svg" alt="" style="">
</div>
- Basis
    <div>
        <img src="images/covector_basis.svg" alt="" style="">
    </div>
    <div>
        <img src="images/covector_basis_prop.svg" alt="" style="">
    </div>
- Covector components
    <div>
        <img src="images/covector_components.svg" alt="" style="">
    </div>

---

# Covector 
- Covector components
<div>
    <img src="images/covector_components.svg" alt="" style="">
</div>
<div>
	<img src="images/covector_component_visual.svg" alt="" style="width: 100%">
</div>
- As row
<div>
	<img src="images/covector_row.svg" alt="" style="">
</div>

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
            <li class="table-content-selected">The exterior derivative</li>
            <li>Hashed Expression</li>
        </ul>
    </div>
</div>
    









