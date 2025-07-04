# 🧠 Julia IR Codegen Pipeline

This folder contains key modules related to the **Intermediate Representation (IR)** and **code generation** pipeline in Julia. These scripts represent different stages in how Julia code is transformed, optimized, and lowered into executable instructions.

Whether you're studying Julia's compiler internals or contributing to language-level improvements, this directory offers insight into how high-level Julia code becomes performant machine code.


---

## 📁 Folder Contents

| File Name       | Description |
|-----------------|-------------|
| `domtree.jl`     | Constructs and manages the **Dominator Tree** of the IR graph, essential for control-flow analysis and SSA (Static Single Assignment) form generation. |
| `driver.jl`      | Coordinates code generation processes; contains wrappers or entry points for various codegen stages. |
| `inlining.jl`    | Implements the logic for **function inlining**, optimizing runtime performance by embedding function bodies directly. |
| `ir.jl`          | Defines the **Intermediate Representation** structure, including expressions, operations, and abstract IR nodes. |
| `legacy.jl`      | Holds deprecated or legacy implementations that are retained for backward compatibility or comparison. |
| `passes.jl`      | Houses **optimization passes** such as constant folding, dead-code elimination, and purity-based transformations. |
| `queries.jl`     | Performs queries on the IR, such as checking for exception safety, purity, or memory allocation behavior. |
| `show.jl`        | Provides functionality to pretty-print or visualize the IR tree; used by developers for debugging and introspection. |
| `slot2ssa.jl`    | Converts **slot-based representation** into **SSA form** (Static Single Assignment), aiding optimization and analysis. |
| `verify.jl`      | Validates the correctness of the IR post-transformation (e.g., SSA invariants, GC root safety). Useful in compiler debugging and development testing. |

---

## 🚀 Why This Matters

Understanding or modifying these modules can help with:

- 📈 Improving Julia’s runtime performance
- 🛠️ Customizing compiler optimization behavior
- 🧪 Experimenting with new language features or IR transformations
- 📚 Learning how modern compilers are structured and how high-level code becomes efficient machine instructions

---

## 🧑‍💻 Who Should Use This?

- 🔍 Compiler developers  
- 🎓 Students studying systems programming or language design  
- 🧠 Contributors to the Julia language  
- 📊 Researchers in performance optimization  

---

## 📄 License

This folder follows the same license as the Julia project: [MIT License](https://opensource.org/licenses/MIT)

---

> ✨ *Exploring how Julia thinks — one IR node at a time.*

