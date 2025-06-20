# User Guide: Interactive Peano Axioms & Addition Visualizer

## Overview

This interactive web application provides a visual and hands-on approach to understanding the Peano axioms and mathematical addition. It demonstrates how natural numbers are constructed and how addition is formally defined in mathematics.

## Getting Started

The application consists of two main sections accessible via tabs at the top:
- **2.1 The Peano Axioms** - Foundation of natural numbers
- **2.2 Addition** - Building addition from basic definitions

## Section 1: The Peano Axioms

### Purpose
Learn how natural numbers are formally constructed using five fundamental axioms.

### Controls

#### Axiom 2.1: 0 ∈ ℕ (Create 0)
- **Action**: Click once to create the number 0
- **Effect**: Initializes the number system and displays a 1×1 grid
- **Note**: This button becomes disabled after first use

#### Axiom 2.2: n++ ∈ ℕ (Successor Function)
- **Action**: 
  1. Click to activate (button turns blue)
  2. Click any number in the grid to create its successor
- **Effect**: Expands the grid to include the next natural number
- **Example**: Clicking 2 creates 3, expanding from 3×3 to 4×4 grid
- **Limit**: Can create numbers up to 9

#### Axiom 2.3: 0 ≠ n++ (Zero is not a successor)
- **Action**: Toggle on/off
- **Effect**: 
  - Shows inequalities between 0 and all positive numbers
  - Displays random fading symbols as visual feedback
- **Demonstrates**: Zero is fundamentally different from all other natural numbers

#### Reflexivity: n = n (Everything equals itself)
- **Action**: Toggle on/off
- **Effect**: Highlights the diagonal showing each number equals itself
- **Visual**: Diagonal cells turn light blue

#### Axiom 2.4: m≠n ⇒ m++≠n++ (Successor preserves inequality)
- **Action**: Toggle on/off
- **Effect**: 
  - Animates the propagation of inequalities
  - Shows how differences between numbers are preserved under succession
- **Animation**: Inequalities appear diagonal by diagonal over 2 seconds

### Tips for Section 1
- Start with Axiom 2.1 to create 0
- Use Axiom 2.2 to build several numbers (try 0→1→2→3)
- Toggle Axiom 2.3 to see how 0 is special
- Enable Reflexivity to see the equality diagonal
- Finally, enable Axiom 2.4 to see inequality propagation

## Section 2: Addition

### Purpose
Understand how addition is formally defined using recursive definitions and prove basic properties.

### Initial Setup
The section displays a 10×10 grid with:
- **Rows**: Left operand (0-9)
- **Columns**: Right operand (0-9)
- **Cells**: Will show addition results when definitions are activated

### Controls

#### Definition 2.2.1a: 0 + m = m
- **Action**: Toggle on/off
- **Effect**: 
  - Fills the top row (0 + m = m)
  - Shows that adding zero to any number gives that number
- **Animation**: Cells fill from left to right
- **Required**: Must be enabled before Definition 2.2.1b

#### Definition 2.2.1b: (n++) + m = (n+m)++
- **Action**: Toggle on/off (only available when 2.2.1a is active)
- **Effect**: 
  - Fills remaining rows using the recursive definition
  - Each row builds on the previous row by adding 1
- **Animation**: Rows fill progressively over 2 seconds
- **Demonstrates**: How addition extends from the base case

#### Lemma 2.2.2: n + 0 = n (Hidden until unlocked)
- **Unlock Condition**: 
  1. Enable both definitions above
  2. Click cell "0 + 0 = 0"
  3. Click the left operand (0) three times consecutively
- **Effect**: Proves that adding 0 to any number gives that number
- **Animation**: Transformation display and column highlighting

### Interactive Proof Mode

When both definitions are enabled, clicking any cell enters **Proof Mode**:

#### What You See
- A highlighted box appears between controls and grid
- Five large buttons display the selected equation (e.g., "3 + 2 = 5")
- Only the left operand is clickable

#### How to Use
1. **Click a cell** (e.g., "3 + 2 = 5") to enter proof mode
2. **Click the left operand** (the "3" button) to apply Definition 2.2.1b
3. **Observe the effects**:
   - Red "++" symbols fade upward from both operand and result buttons
   - Definition 2.2.1b glows green briefly
   - Equation updates (e.g., "3 + 2 = 5" becomes "4 + 2 = 6")

#### Unlocking Lemma 2.2.2
1. Click "0 + 0 = 0" to enter proof mode
2. Click the "0" button three times in a row
3. Watch the unlock animation showing the mathematical reasoning
4. See the n + 0 column shake with smoke effects

### Tips for Section 2
- Always start with Definition 2.2.1a
- Enable Definition 2.2.1b to see the full addition table
- Try proof mode with different equations to understand the recursive nature
- Unlock the lemma by working with "0 + 0" to see the special property
- Pay attention to the visual feedback showing mathematical relationships

## Troubleshooting

**Grid not appearing**: Make sure to click Axiom 2.1 first in the Peano section

**Definition 2.2.1b disabled**: Enable Definition 2.2.1a first

**Proof mode not working**: Ensure both definitions in Section 2 are enabled

**Lemma not unlocking**: Start from "0 + 0 = 0" and click the left "0" exactly three times

**Animations not smooth**: Wait for current animations to complete before triggering new ones

## Educational Value

This tool demonstrates:
- **Constructive Mathematics**: How complex concepts build from simple axioms
- **Formal Definitions**: The precise mathematical meaning of "addition"
- **Proof Techniques**: How mathematical properties are established
- **Visual Learning**: Abstract concepts made concrete through interaction

## Best Practices

1. **Follow the logical order**: Start with basic axioms before advanced concepts
2. **Experiment freely**: The tool is designed for exploration
3. **Watch the animations**: They illustrate important mathematical relationships
4. **Connect concepts**: Notice how Section 2 builds on Section 1's foundation
5. **Take your time**: Let each concept sink in before moving to the next

---

*This tool was designed to make abstract mathematical concepts accessible through interactive visualization and hands-on exploration.*