```
╭────────────────────────────────────────────────────────────────╮
│  ∇ · F = ∂Fₓ/∂x + ∂Fᵧ/∂y + ∂Fᵤ/∂z                            │
│                                                                 │
│  ╔═╗╔═╗╔═╗╔╦╗╔═╗╔╦╗╦═╗╦ ╦  ╦ ╦╔═╗╔═╗╦╔═╔═╗                    │
│  ║ ╦║╣ ║ ║║║║║╣  ║ ╠╦╝╚╦╝  ╠═╣╠═╣║  ╠╩╗╚═╗                    │
│  ╚═╝╚═╝╚═╝╩ ╩╚═╝ ╩ ╩╚═ ╩   ╩ ╩╩ ╩╚═╝╩ ╩╚═╝                    │
╰────────────────────────────────────────────────────────────────╯
```

## Hi, I'm John

**Computational Geometry & Algorithmic 3D Tool Developer**

*Camera-centric sketch-based modeling | Conformal geometry | Spectral methods*

I build tools where **mathematical specification IS the execution**.
The algebra IS the geometry. The tree IS the program.

---

### The Approach

> **Camera-Centric Sketch-Based 3D Modeling**
>
> 2D input → Camera projection → Geometric inference → Resolution-independent output

Traditional modeling manipulates vertices directly. My systems interpret **2D strokes as constraints on 3D form**—projecting through the camera plane to infer depth, curvature, and surface.

```
Traditional:    Sketch → Trace → Extrude → Edit vertices
This System:    Sketch → Project → Solve → Generate
```

---

### Mathematical Foundations

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│  ∇ Gradient    ∇· Divergence    ∇× Curl    Δ Laplacian       │
│                                                                │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐           │
│  │   AFFINE    │◄─│  CONFORMAL  │─►│  SPECTRAL   │           │
│  │   GL(4,ℝ)   │  │   PSL(2,ℂ)  │  │   L²(ℝ³)    │           │
│  └─────────────┘  └─────────────┘  └─────────────┘           │
│                                                                │
│  Möbius:  f(z) = (az+b)/(cz+d)   Circles → Circles           │
│  Fourier: f̂(k) = ∫ f(x) e^(-2πik·x) dx                       │
│  Curvature: κ = dθ/ds                                         │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

### Active Research

| Project | Description |
|---------|-------------|
| [**Geometric Synthesis Framework**](https://github.com/JohnnyNeoman/Math/tree/master/maya-math) | Mathematical compiler: Lift → Operate → Collapse |
| **Skeletal Singleton Tree (SST)** | Functional L-system separating state from mutation |
| **Neural Sketch Field** | FNO-based surface anticipation from boundary curves |
| **Curvature-Aware Octree** | Riemannian metric hierarchy for spectral subdivision |

---

### Spectral Octree & Manifold Navigation

Extending classical octree indexing into **learned Riemannian manifolds**:

```
Level 0: Euclidean       ‖x − y‖₂
Level 1: Mahalanobis     (x−y)ᵀΣ⁻¹(x−y)
Level 2: Riemannian      Geodesic distance with g(x)
Level 3: Fisher-Rao      Information geometry on shape distributions
Level 4: Learned         d_L(x,y) = ‖Φ_θ(x) − Φ_θ(y)‖_{g(θ)}
```

Subdivision follows **spectral energy density** E = Σ αᵢ²λᵢ — refining where geometry is rich, staying coarse where smooth.

---

### Listen to the Framework

[**Executive Summary Audio (5 min)**](https://github.com/JohnnyNeoman/Math/raw/master/maya-math/media/executive_summary_narration.mp3)

---

### Technical Stack

**Geometry:** Computational geometry, conformal maps, spectral methods, Frenet-Serret frames

**3D Platforms:** Maya (MEL/Python), Blender, Unreal Engine 5

**Mathematics:** Linear algebra, differential geometry, Riemannian manifolds, L-systems

**ML Integration:** Fourier Neural Operators, geometric deep learning, spectral regularization

---

### The Legacy: 2,308 MEL Procedures

Analyzed and organized:
- **Circle/tangent geometry** — 234 procedures (conformal PSL(2,ℂ))
- **Linear algebra** — 240 procedures (affine GL(4,ℝ))
- **Camera projection** — 218 procedures (sketch-to-3D mapping)
- **Array batch processing** — 565 procedures (data infrastructure)

[**Explore the Math Repository →**](https://github.com/JohnnyNeoman/Math)

---

> *"The octree isn't just a spatial index—it's a discretization of a distance function.*
> *Every node boundary is a level set. Swap the metric kernel, and behavior changes accordingly."*
