---
name: neo-brutalist
description: This skill should be used when the user asks to "create a neo-brutalist website", "brutalist design", "anti-design", "raw web design", "chunky bold website", or wants a website with intentionally raw, bold, high-contrast aesthetics. Provides font pairings, color palettes, and Tailwind patterns.
---

# Neo-Brutalist Web Design System

Neo-brutalism rebels against polished digital aesthetics with raw honesty. Websites feel bold, unapologetic, and deliberately imperfect. Hard shadows, thick borders, and aggressive typography create unforgettable experiences.

## Design Principles

- **Raw honesty**: No polish, no pretense—show the structure
- **Hard edges**: No soft shadows or subtle gradients—sharp and bold
- **High contrast**: Black on bright, bright on black—maximum impact
- **Chunky elements**: Thick borders, heavy type, solid shapes
- **Intentional "ugliness"**: Beauty through breaking conventions
- **Function over form**: Elements look like what they do

## Anti-AI Design Rules

Avoid these clichés that soften brutalism into generic design:

- **NO emojis** - Never use emojis anywhere in the design
- **NO subtle gradients** - Use solid colors with hard edges
- **NO purple or violet** - Choose bold primaries or neons
- **NO hero badges** - Brutalism doesn't whisper
- **NO glass morphism** - Too refined and polished
- **NO soft shadows** - Hard, offset shadows only
- **NO thin borders** - 2px minimum, 4px+ preferred
- **NO subtle hover states** - Bold, obvious transformations
- **NO muted pastels** - Saturated, loud colors
- **NO smooth transitions** - Instant or stepped changes

## Font Pairings

### Pairing 1: Industrial Mono
```html
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Space+Grotesk:wght@400;500;700&display=swap" rel="stylesheet">
```
```css
--font-heading: 'Space Mono', monospace;
--font-body: 'Space Grotesk', sans-serif;
```
Monospace headlines for that raw, undesigned feeling. Space Grotesk keeps body readable.

### Pairing 2: Black Impact
```html
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Work+Sans:wght@400;500&display=swap" rel="stylesheet">
```
```css
--font-heading: 'Anton', sans-serif;
--font-body: 'Work Sans', sans-serif;
```
Anton's condensed black weight screams. Use sparingly, maximum impact.

### Pairing 3: Tech Brutalism
```html
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700;800&display=swap" rel="stylesheet">
```
```css
--font-heading: 'JetBrains Mono', monospace;
--font-body: 'JetBrains Mono', monospace;
```
All monospace, all the time. Developer aesthetic turned up to 11.

### Pairing 4: Compressed Power
```html
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=IBM+Plex+Sans:wght@400;500&display=swap" rel="stylesheet">
```
```css
--font-heading: 'Bebas Neue', sans-serif;
--font-body: 'IBM Plex Sans', sans-serif;
```
Bebas Neue's tall, compressed letters. Poster typography for the web.

### Pairing 5: Bold Grotesque
```html
<link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Archivo:wght@400;500&display=swap" rel="stylesheet">
```
```css
--font-heading: 'Archivo Black', sans-serif;
--font-body: 'Archivo', sans-serif;
```
Same family, extreme weight contrast. Archivo Black is unapologetically bold.

## Color Palettes

### Palette 1: Highlighter Yellow
```css
--color-bg: #FFFC00;
--color-surface: #FFFFFF;
--color-text: #000000;
--color-border: #000000;
--color-accent: #000000;
--color-shadow: #000000;
```
```js
colors: {
  yellow: '#FFFC00',
  white: '#FFFFFF',
  black: '#000000'
}
```

### Palette 2: Neon Green
```css
--color-bg: #FFFFFF;
--color-surface: #00FF00;
--color-text: #000000;
--color-border: #000000;
--color-accent: #00FF00;
--color-shadow: #000000;
```
```js
colors: {
  white: '#FFFFFF',
  lime: '#00FF00',
  black: '#000000'
}
```

### Palette 3: Hot Pink
```css
--color-bg: #FF00FF;
--color-surface: #FFFFFF;
--color-text: #000000;
--color-border: #000000;
--color-accent: #FFFFFF;
--color-shadow: #000000;
```
```js
colors: {
  magenta: '#FF00FF',
  white: '#FFFFFF',
  black: '#000000'
}
```

### Palette 4: Inverted
```css
--color-bg: #000000;
--color-surface: #FFFFFF;
--color-text: #FFFFFF;
--color-border: #FFFFFF;
--color-accent: #FF3333;
--color-shadow: #FFFFFF;
```
```js
colors: {
  black: '#000000',
  white: '#FFFFFF',
  red: '#FF3333'
}
```

### Palette 5: Electric Blue
```css
--color-bg: #0066FF;
--color-surface: #FFFFFF;
--color-text: #000000;
--color-border: #000000;
--color-accent: #FFFC00;
--color-shadow: #000000;
```
```js
colors: {
  blue: '#0066FF',
  white: '#FFFFFF',
  black: '#000000',
  yellow: '#FFFC00'
}
```

## Tailwind Patterns

### Layout & Spacing
```html
<!-- Chunky padding -->
<section class="px-4 py-16 md:px-8 lg:px-16 bg-yellow">
  <div class="max-w-6xl mx-auto">
    <!-- Content -->
  </div>
</section>

<!-- Hard-edged container -->
<div class="border-4 border-black p-6 bg-white
            shadow-[8px_8px_0px_0px_#000000]">
```

### Typography Scale
```html
<!-- Massive headline -->
<h1 class="text-6xl md:text-8xl lg:text-9xl font-bold uppercase tracking-tight leading-none">
  BOLD<br/>STATEMENT
</h1>

<!-- Monospace body -->
<p class="font-mono text-lg leading-relaxed">
```

### Buttons
```html
<!-- Primary: hard shadow -->
<button class="px-8 py-4 bg-black text-white font-bold uppercase
               border-4 border-black
               shadow-[4px_4px_0px_0px_#FFFC00]
               hover:shadow-none hover:translate-x-1 hover:translate-y-1
               transition-all duration-100">
  CLICK ME
</button>

<!-- Secondary: outlined with hover fill -->
<button class="px-8 py-4 bg-transparent text-black font-bold uppercase
               border-4 border-black
               hover:bg-black hover:text-white
               transition-colors duration-100">
  LEARN MORE
</button>

<!-- Inverted -->
<button class="px-8 py-4 bg-white text-black font-bold uppercase
               border-4 border-black
               shadow-[4px_4px_0px_0px_#000000]
               hover:shadow-none hover:translate-x-1 hover:translate-y-1
               transition-all duration-100">
  GET STARTED
</button>
```

### Cards & Containers
```html
<!-- Hard shadow card -->
<div class="border-4 border-black bg-white p-6
            shadow-[8px_8px_0px_0px_#000000]">
  <h3 class="text-2xl font-bold uppercase mb-4">TITLE</h3>
  <p class="font-mono">Description text here.</p>
</div>

<!-- Colored card -->
<div class="border-4 border-black bg-lime p-6">
  <h3 class="text-2xl font-bold uppercase mb-4">FEATURE</h3>
  <p>Bold statement about this feature.</p>
</div>

<!-- Stacked effect -->
<div class="relative">
  <div class="absolute inset-0 border-4 border-black bg-yellow translate-x-3 translate-y-3"></div>
  <div class="relative border-4 border-black bg-white p-6">
    Content
  </div>
</div>
```

### Borders & Dividers
```html
<!-- Thick divider -->
<hr class="border-t-4 border-black my-16" />

<!-- Dashed border -->
<div class="border-4 border-dashed border-black p-6">
```

### Navigation
```html
<nav class="flex items-center justify-between px-4 py-4 md:px-8 border-b-4 border-black bg-white">
  <a href="/" class="text-2xl font-bold uppercase">BRAND</a>
  <div class="hidden md:flex items-center gap-6">
    <a href="#" class="font-bold uppercase hover:bg-yellow px-3 py-2 transition-colors">Products</a>
    <a href="#" class="font-bold uppercase hover:bg-yellow px-3 py-2 transition-colors">About</a>
    <button class="px-6 py-3 bg-black text-white font-bold uppercase border-4 border-black">
      CONTACT
    </button>
  </div>
</nav>
```

### Hero Section
```html
<section class="min-h-screen flex items-center bg-yellow px-4 md:px-8 lg:px-16 py-24">
  <div class="max-w-7xl mx-auto w-full">
    <div class="grid lg:grid-cols-2 gap-12 items-center">
      <div>
        <p class="font-mono text-sm mb-4">// WELCOME TO THE FUTURE</p>
        <h1 class="text-6xl md:text-7xl lg:text-8xl font-bold uppercase leading-none mb-8">
          NO<br/>RULES<br/>APPLY
        </h1>
        <p class="font-mono text-lg max-w-md mb-8">
          We break conventions and build something real. No polish. No pretense.
        </p>
        <div class="flex flex-wrap gap-4">
          <button class="px-8 py-4 bg-black text-white font-bold uppercase
                         border-4 border-black shadow-[4px_4px_0px_0px_#FFFFFF]
                         hover:shadow-none hover:translate-x-1 hover:translate-y-1
                         transition-all duration-100">
            GET STARTED
          </button>
          <button class="px-8 py-4 bg-white text-black font-bold uppercase
                         border-4 border-black
                         hover:bg-black hover:text-white transition-colors">
            LEARN MORE
          </button>
        </div>
      </div>
      <div class="border-4 border-black bg-white p-4 shadow-[12px_12px_0px_0px_#000000]">
        <img class="w-full aspect-square object-cover" />
      </div>
    </div>
  </div>
</section>
```

### Feature Grid
```html
<section class="bg-white border-y-4 border-black px-4 md:px-8 py-16">
  <div class="max-w-6xl mx-auto">
    <h2 class="text-5xl md:text-6xl font-bold uppercase mb-12">FEATURES</h2>
    <div class="grid md:grid-cols-3 gap-0 border-4 border-black">
      <div class="p-8 border-r-4 border-b-4 md:border-b-0 border-black">
        <span class="font-mono text-4xl font-bold">01</span>
        <h3 class="text-xl font-bold uppercase mt-4 mb-2">FAST</h3>
        <p class="font-mono text-sm">Lightning quick performance.</p>
      </div>
      <div class="p-8 border-r-4 border-b-4 md:border-b-0 border-black">
        <span class="font-mono text-4xl font-bold">02</span>
        <h3 class="text-xl font-bold uppercase mt-4 mb-2">BOLD</h3>
        <p class="font-mono text-sm">Stand out from the crowd.</p>
      </div>
      <div class="p-8">
        <span class="font-mono text-4xl font-bold">03</span>
        <h3 class="text-xl font-bold uppercase mt-4 mb-2">RAW</h3>
        <p class="font-mono text-sm">Unapologetically honest.</p>
      </div>
    </div>
  </div>
</section>
```

### Marquee/Ticker
```html
<div class="bg-black text-white py-4 border-y-4 border-white overflow-hidden">
  <div class="animate-marquee whitespace-nowrap">
    <span class="font-bold uppercase text-2xl mx-8">BREAKING RULES</span>
    <span class="text-yellow text-2xl">★</span>
    <span class="font-bold uppercase text-2xl mx-8">MAKING WAVES</span>
    <span class="text-yellow text-2xl">★</span>
    <span class="font-bold uppercase text-2xl mx-8">NO LIMITS</span>
    <span class="text-yellow text-2xl">★</span>
  </div>
</div>
```

### Form Elements
```html
<!-- Brutal input -->
<input type="text"
       class="w-full border-4 border-black p-4 font-mono
              focus:outline-none focus:shadow-[4px_4px_0px_0px_#000000]
              placeholder:text-gray-500"
       placeholder="YOUR EMAIL" />

<!-- Brutal checkbox -->
<label class="flex items-center gap-3 cursor-pointer">
  <input type="checkbox" class="w-6 h-6 border-4 border-black accent-yellow" />
  <span class="font-bold uppercase">I AGREE</span>
</label>
```

### Footer
```html
<footer class="bg-black text-white px-4 md:px-8 py-16 border-t-4 border-white">
  <div class="max-w-6xl mx-auto">
    <div class="grid md:grid-cols-4 gap-8 mb-12">
      <div>
        <h4 class="font-bold uppercase text-xl mb-4">BRAND</h4>
        <p class="font-mono text-sm text-gray-400">Breaking the internet since 2024.</p>
      </div>
      <div>
        <h4 class="font-bold uppercase mb-4">LINKS</h4>
        <ul class="space-y-2 font-mono text-sm">
          <li><a href="#" class="hover:text-yellow transition-colors">→ Products</a></li>
          <li><a href="#" class="hover:text-yellow transition-colors">→ About</a></li>
          <li><a href="#" class="hover:text-yellow transition-colors">→ Contact</a></li>
        </ul>
      </div>
    </div>
    <div class="border-t-4 border-white/20 pt-8">
      <p class="font-mono text-sm">© 2024 NO RIGHTS RESERVED</p>
    </div>
  </div>
</footer>
```

## Advanced Creative Patterns

### Dramatic Typography
```html
<!-- Massive stacked letters -->
<h1 class="text-[25vw] font-black uppercase leading-[0.75] tracking-tighter">
  RAW<br/>POWER
</h1>

<!-- Outlined + filled contrast -->
<div>
  <span class="block text-[15vw] font-black uppercase text-transparent [-webkit-text-stroke:4px_black]">
    BREAK
  </span>
  <span class="block text-[15vw] font-black uppercase text-black -mt-8">
    FREE
  </span>
</div>

<!-- Rotated text block -->
<div class="relative">
  <span class="absolute -left-20 top-1/2 -translate-y-1/2 -rotate-90 font-mono text-sm tracking-widest">
    SECTION 01
  </span>
  <h2 class="text-6xl font-bold uppercase ml-12">FEATURES</h2>
</div>

<!-- Marquee text effect -->
<div class="overflow-hidden border-y-4 border-black py-4">
  <div class="animate-marquee whitespace-nowrap">
    <span class="text-4xl font-black uppercase mx-8">BOLD</span>
    <span class="text-4xl font-black uppercase mx-8">RAW</span>
    <span class="text-4xl font-black uppercase mx-8">REAL</span>
    <span class="text-4xl font-black uppercase mx-8">LOUD</span>
  </div>
</div>

<!-- Glitch-style offset text -->
<div class="relative">
  <span class="absolute text-[10vw] font-black uppercase text-yellow -translate-x-2 -translate-y-2">
    GLITCH
  </span>
  <span class="absolute text-[10vw] font-black uppercase text-cyan translate-x-2 translate-y-2">
    GLITCH
  </span>
  <span class="relative text-[10vw] font-black uppercase text-black">
    GLITCH
  </span>
</div>
```

### Breaking the Grid
```html
<!-- Diagonal slice -->
<section class="relative min-h-screen">
  <div class="absolute inset-0 bg-yellow"
       style="clip-path: polygon(0 0, 100% 0, 100% 70%, 0 100%);"></div>
  <div class="absolute inset-0 bg-black"
       style="clip-path: polygon(0 70%, 100% 30%, 100% 100%, 0 100%);"></div>
</section>

<!-- Overlapping boxes -->
<div class="relative">
  <div class="bg-yellow border-4 border-black p-12 w-3/4">
    <h2 class="text-4xl font-bold uppercase">BOX ONE</h2>
  </div>
  <div class="bg-white border-4 border-black p-12 w-2/3 -mt-16 ml-auto relative z-10
              shadow-[8px_8px_0px_0px_#000000]">
    <h2 class="text-4xl font-bold uppercase">BOX TWO</h2>
  </div>
</div>

<!-- Scattered/chaotic layout -->
<div class="relative min-h-screen">
  <div class="absolute top-10 left-10 border-4 border-black p-6 bg-white rotate-3
              shadow-[6px_6px_0px_0px_#000000]">
    Item 1
  </div>
  <div class="absolute top-32 right-20 border-4 border-black p-6 bg-lime -rotate-2
              shadow-[6px_6px_0px_0px_#000000]">
    Item 2
  </div>
  <div class="absolute bottom-20 left-1/4 border-4 border-black p-6 bg-yellow rotate-1
              shadow-[6px_6px_0px_0px_#000000]">
    Item 3
  </div>
</div>

<!-- Full-bleed color blocks -->
<div class="grid lg:grid-cols-2">
  <div class="bg-black text-white p-16 min-h-[50vh] flex items-center">
    <h2 class="text-6xl font-bold uppercase">DARK</h2>
  </div>
  <div class="bg-yellow p-16 min-h-[50vh] flex items-center">
    <h2 class="text-6xl font-bold uppercase">LIGHT</h2>
  </div>
</div>
```

### Image Treatments
```html
<!-- Hard border frame -->
<div class="border-8 border-black p-2 bg-black">
  <img class="w-full" />
</div>

<!-- Stacked shadow frames -->
<div class="relative">
  <div class="absolute inset-0 bg-black translate-x-4 translate-y-4"></div>
  <div class="absolute inset-0 bg-yellow translate-x-2 translate-y-2"></div>
  <img class="relative w-full border-4 border-black" />
</div>

<!-- Halftone effect -->
<div class="relative">
  <img class="w-full grayscale contrast-150" />
  <div class="absolute inset-0 mix-blend-multiply opacity-50"
       style="background: radial-gradient(circle, black 1px, transparent 1px);
              background-size: 6px 6px;"></div>
</div>

<!-- Duotone harsh -->
<div class="relative">
  <img class="w-full grayscale" />
  <div class="absolute inset-0 bg-yellow mix-blend-multiply"></div>
</div>

<!-- Torn edge effect -->
<div class="relative">
  <img class="w-full"
       style="clip-path: polygon(0 0, 100% 2%, 98% 100%, 3% 97%);" />
</div>
```

### Hover & Micro-interactions
```html
<!-- Shadow jumps on hover -->
<button class="px-8 py-4 bg-yellow border-4 border-black font-bold uppercase
               shadow-[4px_4px_0px_0px_#000000]
               hover:shadow-[8px_8px_0px_0px_#000000]
               hover:-translate-x-1 hover:-translate-y-1
               transition-all duration-100">
  CLICK ME
</button>

<!-- Color swap -->
<a href="#" class="block p-8 bg-white border-4 border-black
                   hover:bg-black hover:text-white
                   transition-colors duration-100">
  <h3 class="text-2xl font-bold uppercase">SWAP COLORS</h3>
</a>

<!-- Shadow disappears -->
<div class="bg-lime border-4 border-black p-8
            shadow-[8px_8px_0px_0px_#000000]
            hover:shadow-none hover:translate-x-2 hover:translate-y-2
            transition-all duration-100 cursor-pointer">
  <p class="font-bold">PRESS ME</p>
</div>

<!-- Border thickens -->
<div class="border-4 border-black p-8 hover:border-8 transition-all duration-100">
  <p class="font-bold uppercase">THICK BORDER</p>
</div>

<!-- Rotate on hover -->
<div class="border-4 border-black p-8 bg-white
            hover:rotate-3 transition-transform duration-100
            shadow-[4px_4px_0px_0px_#000000]">
  <p class="font-bold uppercase">TILTS</p>
</div>
```

### Texture & Depth
```html
<!-- Newspaper dot pattern -->
<div class="relative">
  <div class="absolute inset-0"
       style="background: radial-gradient(circle, black 1px, transparent 1px);
              background-size: 8px 8px;"></div>
</div>

<!-- Diagonal stripes -->
<div class="relative overflow-hidden">
  <div class="absolute inset-0"
       style="background: repeating-linear-gradient(
         45deg,
         transparent,
         transparent 10px,
         black 10px,
         black 12px
       );"></div>
</div>

<!-- Stacked shadows -->
<div class="relative">
  <div class="absolute inset-0 bg-black translate-x-6 translate-y-6"></div>
  <div class="absolute inset-0 bg-red translate-x-3 translate-y-3"></div>
  <div class="relative bg-white border-4 border-black p-8">
    Triple stack
  </div>
</div>

<!-- Checkerboard -->
<div class="relative">
  <div class="absolute inset-0"
       style="background: repeating-conic-gradient(black 0% 25%, white 0% 50%) 50% / 20px 20px;"></div>
</div>
```

### Advanced Hero Example
```html
<section class="relative min-h-screen bg-yellow overflow-hidden">
  <!-- Diagonal stripe background -->
  <div class="absolute inset-0 opacity-10"
       style="background: repeating-linear-gradient(
         -45deg,
         transparent,
         transparent 20px,
         black 20px,
         black 22px
       );"></div>

  <!-- Scattered decorative elements -->
  <div class="absolute top-20 right-20 w-32 h-32 bg-black rotate-12"></div>
  <div class="absolute bottom-40 left-10 w-20 h-20 border-4 border-black -rotate-6"></div>

  <div class="relative z-10 min-h-screen flex flex-col">
    <!-- Brutal nav -->
    <nav class="flex items-center justify-between px-4 md:px-8 py-4 border-b-4 border-black">
      <span class="text-2xl font-black uppercase">BRAND</span>
      <div class="flex gap-4">
        <a href="#" class="font-bold uppercase hover:bg-black hover:text-yellow px-4 py-2 transition-colors">
          WORK
        </a>
        <a href="#" class="font-bold uppercase hover:bg-black hover:text-yellow px-4 py-2 transition-colors">
          INFO
        </a>
        <button class="px-6 py-2 bg-black text-yellow font-bold uppercase border-4 border-black">
          CONTACT
        </button>
      </div>
    </nav>

    <!-- Hero content -->
    <div class="flex-1 flex items-center px-4 md:px-8 lg:px-16">
      <div class="max-w-7xl mx-auto w-full">
        <!-- Giant headline -->
        <h1 class="text-[18vw] md:text-[15vw] font-black uppercase leading-[0.8] tracking-tighter mb-8">
          NO<br/>
          <span class="text-transparent [-webkit-text-stroke:4px_black]">RULES</span><br/>
          APPLY
        </h1>

        <div class="flex flex-wrap gap-4 mb-12">
          <button class="px-10 py-5 bg-black text-yellow font-black uppercase text-xl
                         border-4 border-black shadow-[6px_6px_0px_0px_#FFFFFF]
                         hover:shadow-none hover:translate-x-1.5 hover:translate-y-1.5
                         transition-all duration-100">
            START NOW
          </button>
          <button class="px-10 py-5 bg-white text-black font-black uppercase text-xl
                         border-4 border-black
                         hover:bg-black hover:text-white transition-colors duration-100">
            SEE WORK
          </button>
        </div>

        <p class="font-mono text-lg max-w-md">
          // WE BUILD DIGITAL EXPERIENCES THAT BREAK CONVENTIONS AND DEMAND ATTENTION.
        </p>
      </div>
    </div>

    <!-- Bottom ticker -->
    <div class="border-t-4 border-black bg-black text-yellow py-3 overflow-hidden">
      <div class="animate-marquee whitespace-nowrap font-bold text-lg">
        <span class="mx-6">DESIGN</span>
        <span class="mx-6">*</span>
        <span class="mx-6">DEVELOP</span>
        <span class="mx-6">*</span>
        <span class="mx-6">DEPLOY</span>
        <span class="mx-6">*</span>
        <span class="mx-6">DISRUPT</span>
        <span class="mx-6">*</span>
      </div>
    </div>
  </div>
</section>
```

## Implementation Notes

1. **Border width**: 4px minimum, consistency is key
2. **Shadows**: Hard offset only (X_Y_0_0), never blurred
3. **Colors**: Maximum 3, high contrast between them
4. **Typography**: Bold weights, uppercase headlines
5. **Hover states**: Dramatic—shadow removal, color inversion
6. **Transitions**: Fast (100ms) or instant, never smooth
7. **Corners**: Choose corner radius based on design context
8. **Spacing**: Consistent, grid-based, intentional gaps
