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
    
---

# Exterior derivative
- Tangent space 
    - Every point in manifold `M` (care <img src="images/rn.svg" alt="" style=""> only)
    - Set of all tangent vectors to the point p
    - Form a vector space with <img src="images/r.svg" alt="" style="">
    - <img src="images/tpm.svg" alt="" style="">
    - <img src="images/isomorphic.svg" alt="" style="">

---
# Exterior derivative
- Tangent space
<div class="flex-row" style="justify-content: center;">
	<img src="images/sphere.svg" alt="" style="">
</div>

---
# Exterior derivative
- Tangent space
<div class="flex-row" style="justify-content: center;">
	<img src="images/r2.svg" alt="" style="">
</div>
    
---
# Exterior derivative
- Exterior derivative
    - Turn *k*-form to *(k+1)*-form
    - *k*-form
    <div>
    <img src="images/k_form1.svg" alt="" style="">
    </div>
    <div>
    <img src="images/k_form2.svg" alt="" style="">
    </div>
    
        

---
# 1-form
- First exterior derivative (*0*-form to *1*-form)
<div>
<img src="images/dop1.svg" alt="" style="">
<img src="images/dop2.svg" alt="" style="">
</div>
      
---
# 1-form
<div class="flex-row" style="justify-content: center; height: 80%">
	<img src="images/lvlsets.svg" alt="" style="">
</div>

---
# 1-form
<div class="flex-row" style="justify-content: center; height: 80%">
	<img src="images/lvlsets2.svg" alt="" style="">
</div>

---
# 1-form
<div class="flex-row" style="justify-content: center; height: 80%">
	<img src="images/zoom_in.svg" alt="" style="">
</div>

---
# 1-form
<div class="flex-row" style="justify-content: center; height: 80%">
	<img src="images/zoom_in2.svg" alt="" style="">
</div>

---
# 1-form
- Basis
<div class="flex-row" style="justify-content: center; height: 80%">
	<img src="images/dx_basis.svg" alt="" style="">
</div>


---
# 1-form
- Basis
<div>
	<img src="images/dxdy.svg" alt="" style="">
</div>
- Component
<div>
    <img src="images/covector_components.svg" alt="" style="">
</div>
- Similarly
<div>
    <img src="images/similardf.svg" alt="" style="">
</div>
<div>
    <img src="images/df.svg" alt="" style="">
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
            <li >The exterior derivative</li>
            <li class="table-content-selected">Hashed Expression</li>
        </ul>
    </div>
</div>

---
# Hashed Expression
- Share common subexpressions
- Type-safety 
- Compute derivatives symbolically
- Simplify and group expressions
- Part of the **Coconut** ecosystem

---
# Types

```haskell
data Expression d et =
    Expression
        { exIndex :: Int 
        , exMap :: ExpressionMap 
        }
    deriving (Show, Eq, Ord, Typeable)

-- d: Zero, One, Two, Three
-- et: R, C, Covector 
```

---
# Types

```haskell
type Internal = (Shape, Node)
-- []        --> scalar
-- [n]       --> 1D with size n
-- [n, m]    --> 2D with size n × m
-- [n, m, p] --> 3D with size n × m × p
type Shape = [Int]

type ExpressionMap = IntMap Internal
```
---
# Types

```haskell
data Node
    = Var String
    | DVar String 
    | Const Double 
    | Sum ET Args 
    | Mul ET Args 
    | Scale ET Arg Arg
    | Div Arg Arg
    ...
```

---
# Share common subexpressions
```haskell
$ x = var "x"
Expression 
    { exIndex = 120
    , exMap = 
        fromList [(120,([],Var "x"))]
    }
```

---
# Share common subexpressions
```haskell
$ x + x
Expression 
    { exIndex = 254577784
    , exMap = fromList 
        [ (120,([],Var "x")),
        , (254577784,([],Sum R [120,120]))
        ]
    }
```

---
# Share common subexpressions
```haskell
$ (x + y) + (x + y)
Expression
    { exIndex = 542494359821144
    , exMap =
          fromList
              [ (120, ([], Var "x"))
              , (121, ([], Var "y"))
              , (256625675, ([], Sum R [120, 121]))
              , (542494359821144, 
                ([], Sum R [256625675, 256625675]))
              ]
    }
```

---
# Type safety
- 2 phantom type argument in `Expression`
    ```haskell
    data Expression d et =
        Expression
            { exIndex :: Int 
            , exMap :: ExpressionMap 
            }
    ```


---

# Type safety
```haskell
-- | Type representation of 
-- elements in the 0D, 1D, 2D, 3D, ... grid
--
data R
    deriving (NumType, ElementType, Addable)

data C
    deriving (NumType, ElementType, Addable)

data Covector
    deriving (ElementType, Addable)
```

---

# Type safety

```haskell
-- | Type representation of dimension
--
data Zero
    deriving (DimensionType)

data One
    deriving (DimensionType)

data Two
    deriving (DimensionType)

data Three
    deriving (DimensionType)
```


---

# Type safety
- We can then govern which operations are allowed on which kind of expressions, and the returned kind of expression
    ```haskell
    (+) :: (Addable et, DimensionType d) 
        => Expression d et 
        -> Expression d et 
        -> Expression d et
    ```
    
---
    
# Type safety
- The exterior derivative
    ```haskell
    exteriorDerivative ::
           (DimensionType d)
        => Set String
        -> Expression d R
        -> Expression d Covector
    ```

---
# Demo
