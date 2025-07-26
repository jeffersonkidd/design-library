
#  🎨 Jefferson Kidd- "*Personal Design System*" 

[Link #1](https://jeffersonkidd.github.io/design-library/)  |  [Link #2](https://jeffersonkidd.github.io/design-library/) | [Link #3](https://jeffersonkidd.github.io/design-library/) | [Link #4](https://jeffersonkidd.github.io/design-library/) |  [Link #5](https://://jeffersonkidd.github.io/design-library/)

### ⚡️ API design library (beta)

Live site:  [ jeffersonkidd.design](https://jeffersonkidd.com/design/index.html)  
Repo: [jeffersonkidd/design-library]()


## 
- Hosted on GitHub Pages.    
- Made with reusable web components.      
- Access to:  🪙 [Design tokens](https://jeffersonkidd.github.io/design-library/css/tokens.html) , 🧰  [Components](https://jeffersonkidd.github.io/design-library/components.html) ,  📄  [Pages](https://jeffersonkidd.github.io/design-library/components.html) , 

###  🩻 File System

```
|root
|------
|------
 
``` 
⚡️ Starting with a minimal, essential set of design token primitives sets the foundation for a scalable and consistent design system without overengineering it. Here's a lean starter pack that's flexible enough for real-world use but simple enough not to slow you down.

# 🧱 Essential Minimum Design Token Primitives

### 1.) Color

Define base colors used throughout your system. These should be abstracted from their usage.

``` json
"color": {
  "base": {
    "white": "#ffffff",
    "black": "#000000"
  },
  "gray": {
    "50": "#f9f9f9",
    "100": "#f0f0f0",
    "900": "#1a1a1a"
  },
  "primary": {
    "500": "#3b82f6"
  },
  "error": {
    "500": "#ef4444"
  }
} 
```

💡 *Start small (e.g., grayscale, primary, semantic). Add hues/tones later.*

### 2. Typography

Define the core type properties individually so they can be recombined later.  

``` json
"font": {
  "family": {
    "sans": "'Inter', sans-serif"
  },
  "size": {
    "xs": "0.75rem",
    "sm": "0.875rem",
    "base": "1rem",
    "lg": "1.125rem",
    "xl": "1.25rem"
  },
  "weight": {
    "regular": "400",
    "medium": "500",
    "bold": "700"
  },
  "lineHeight": {
    "tight": "1.1",
    "normal": "1.5",
    "relaxed": "1.625"
  }
}
```

### 3. Spacing
Used for padding, margin, gap, etc. Stick to a consistent scale (4px is common).

```json
"spacing": {
  "0": "0px",
  "1": "4px",
  "2": "8px",
  "3": "12px",
  "4": "16px",
  "5": "20px",
  "6": "24px",
  "8": "32px"
}
```

### 4. Border Radius
Keep a small scale unless you’re building a very stylized system.

``` json
"radius": {
  "none": "0px",
  "sm": "4px",
  "md": "8px",
  "lg": "16px",
  "full": "9999px"
} 
```

### 5. Shadow (Optional but useful)  
Even just one or two helps bring life to components.

``` json
"shadow": {
  "sm": "0 1px 2px rgba(0, 0, 0, 0.05)",
  "md": "0 4px 6px rgba(0, 0, 0, 0.1)"
}
```

### 6. Opacity
Especially handy for overlays and disabled states.
``` json
"opacity": {
  "0": "0",
  "50": "0.5",
  "100": "1"
}
```

## ✅ Summary: Just These to Start

| Token Group           | What to Define                    | 
|:----------------------|:----------------------------------|
| color                 | base, gray scale, brand, semantic |
| font.family           | one or two to start               |
| font.size             | 4-6 sizes                         |
| font.weight           | 3-4 weights                       |
| lineHeight            | tight, normal, relaxed.           |  
| spacing               | 0 to 32px scale                   | 
| radius                | sm, md, lg, full                  |  
| shadow                | sm, md (optional)                 |  
| opacity               | 0, 50, 100.                       |    